# example_workspaces

This repository holds some example workspaces to let the user know how to use some modules in Neorg.

## How to use it

Clone this repository: `git clone https://github.com/nvim-neorg/example_workspaces.git`

## Neorg GTD Tutorial

To use the tutorial, create a new workspace in your config, pointing to the gtd directory, and add the workspace to GTD config:

```lua
require("neorg").setup({
  load = {
    ["core.defaults"] = {},
    ["core.norg.dirman"] = {
      config = {
        workspaces = {
          example_gtd = "/path_where_you_cloned/example_workspaces/gtd",
        },
      },
    },
    ["core.gtd.base"] = {
      config = {
        workspace = "example_gtd",
      },
    },
  }
})
```

After that, just enter Neorg, and go to the workspace: `:Neorg workspace example_gtd`
