# Optional - 参数可选值（类似枚举）

以下语句指定了参数 `a` 的值必须是 `3`，`6`，`9` 中的一个。

```rust
param a: 10 [3, 6, 9];
```

也可以为每个参数指定一个标题，用于在客户端中给用户更清晰的参数说明。

```rust
param a: 10 ["短": 3, "中": 6, "长": 9];
```