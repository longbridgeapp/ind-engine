# String - 字符串

字符串插值主要用于拼接字符串

以下语句 `a` 的输出结果为 `"abc30def"`

```rust
a := "Hello";
b := "world";

message: a + ", " + b;
// Hello, world

out: `abcdef{10 + 20}`;
// abcdef30
```

大括号内左右空格将被忽略。

```rust
a: `abc{        10 + 20    }def`;
// abcdef30
```
