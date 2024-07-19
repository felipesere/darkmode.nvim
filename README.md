# darkmode.nvim
Watches a file and switches the theme based on the content

## Setup

With lazy nvim:

```lua
return {
  {
    "felipesere/darkmode.nvim",
    dependencies = {
      "rktjmp/fwatch.nvim",
    },
    opts = {
      on_dark = function()
        vim.opt.background = "dark"
        vim.cmd.colorscheme "catppuccin-frappe"
      end,
      on_light = function()
        vim.opt.background = "light"
        vim.cmd.colorscheme "rosebones"
      end,
    }
  }
}
```
