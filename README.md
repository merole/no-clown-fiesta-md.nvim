# No Clown Fiesta

An attempt at a color scheme that does not look like a clown puked up the source code.

I added support for the most basic features of tree sitter. No idea why they werent in there before...

![image](https://gustafrydholm.xyz/images/no-clown-fiesta.png)

## Usage

To enable this colorscheme:

```vim
colorscheme no-clown-fiesta
```

```lua
vim.cmd[[colorscheme no-clown-fiesta]]
```

To override the default settings you need to call setup before enabling the
colorscheme. No-clown-fiesta will use these settings, unless you call setup
and override these.

```lua
require("no-clown-fiesta").setup({
  transparent = false, -- Enable this to disable the bg color
  styles = {
    -- You can set any of the style values specified for `:h nvim_set_hl`
    comments = {},
    keywords = {},
    functions = {},
    variables = {},
    type = { bold = true },
    lsp = { underline = true }
  },
})
```

## Supported Plugins

- Alpha
- Dadbod-ui
- Git
- Hop
- Lazy
- Leap
- Lir
- LSP
- Lualine
- Markdown
- Mason
- Neogit
- NvimCmp
- NvimTree
- StatusLine
- Telescope
- Treesitter
- WhichKey
- Neotest
- Dap UI
