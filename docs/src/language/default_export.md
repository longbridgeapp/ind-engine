# Default Export - 默认导出

如果一个指标只需要导出一个值，通常可以省略变量名，指标编译器将为该变量自动命名为 `@default`。

以下语句赋值 `10 + a` 的计算结果到 `@default` 变量，并导出它。

```rust
a := 20;
10 + a
```

> NOTE: 最后一个语句的分号可以省略。
