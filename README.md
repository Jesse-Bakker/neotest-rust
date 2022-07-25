# neotest-rust

[Neotest](https://github.com/rcarriga/neotest) adapter for Rust, using
[cargo-nextest](https://nexte.st/).

Requires [nvim-treesitter](https://github.com/nvim-treesitter/nvim-treesitter)
and the parser for Rust.

```lua
require("neotest").setup({
  adapters = {
    require("neotest-rust")
  }
})
```

Supports standard library tests, [`rstest`](https://github.com/la10736/rstest),
Tokio's `[#tokio::test]`, and more. Does not support `rstest`'s parametrized
tests.
