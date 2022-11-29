# Variable - 变量

以下语句表示计算 `1` 和 变量 `b` 的和。

```rust
b := 8;
a := 1 + b;
// a 的值现在为 9
```

## 赋值语句

赋值语句用于为指标内的一个临时变量赋值，如果该变量已经存在，则覆盖它原有的值。

> NOTE: 不能为参数赋值。

以下语句为变量 `a` 赋值为 `10 + 20` 的计算结果。

```rust
a := 10 + 20;
// a 的值现在为 30
```