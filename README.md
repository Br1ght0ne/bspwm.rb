# bspwm.rb
Simple bspwm configuration DSL in Ruby.

# Usage
```ruby
require 'bspwm'

your_workspaces = ['I', 'II', 'III']
your_configuration = { click_to_focus: :any, border_width: 2 }
your_window_rules = { firefox: { desktop: 2 } }
your_commands = ['sxhkd &', '$HOME/bin/bootstrap -w bspwm &']

BSPWM.configure do
  monitor your_workspaces
  config your_configuration
  rules your_window_rules
  run your_commands
end
```

# License

This gem is licensed under the MIT license. Pull requests are welcome.
