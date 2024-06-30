# vim-ai-lolmax

This project is a fork of the [vim-ai](https://github.com/madox2/vim-ai) interface that uses [lolmax](https://github.com/davehughes/lolmax) as a backend to
manage chat and completion profiles. The original project's README is a much better resource for understanding
how to set this up and use it (for now, anyways).

# Setup
+ TODO: configure 'roles', possibly renaming to 'effects' and allowing multiple at once.
+ TODO: configure 'models'. 
+ Roles and models are both identifier strings that are passed to the lolmax backend to control prompt
  composition. 
+ TODO: add info commands to query lolmax backend and list available models and effects

# Telescope extensions
+ `:Telescope vim_ai_lolmax choose_model` opens up a list of available models and their configurations, and selecting
  one updates the model in use (`vim.g.vim_ai_model`)
+ `:Telescope vim_ai_lolmax choose_effects` opens up a list of defined effects from the lolmax server, and selecting
  them will toggle them on or off (someday - this is TBD)
