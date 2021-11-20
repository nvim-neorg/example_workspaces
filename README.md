# example_workspaces

## How to use this:

Clone this repository.
`git clone https://github.com/nvim-neorg/example_workspaces.git`

In your neorg config:
```lua
require("neorg").setup({
    ["core.norg.dirman"] = {
      config = {
        workspaces = {
          example_gtd = "~/example_workspaces/gtd",
        },
      },
    },
    ["core.gtd.base"] = {
      config = {
        workspace = "example_gtd",
      },
    },
})
```
