# Get Startted

指标语言与普通编程语言最大的区别是，指标语言是有状态的，每次计算都会影响下一次计算的结果。

下面是例子用于计算成交量的总和，`sum` 函数的第二个参数周期数为 `0` 意味着从第一个值开始：

```rust
sumvol: sum(vol, 0);
```

编译指标得到 `Program` 后，使用 `Program::instantiate` 方式实例化出一个可执行的指标。

现在我们输入第一根 K 线，该周期成交量为 `10`：

```rust
instance.set_candlestick(Candlestick { time: 1, volume: 10, .. });
instance.calculate(StepMode::Step);
```

得到的输出结果是：

```json
{ "sumvol": 10 }
```

然后输入第二根 K 线，该周期成交量为 `5`：

```rust
instance.set_candlestick(Candlestick { time: 2, volume: 5, .. });
instance.calculate(StepMode::Step);
```

得到的输出结果是：

```json
{ "sumvol": 15 }
```
