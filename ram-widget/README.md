# Ram widget

This widget shows the RAM usage. When clicked another widget appears with more detailed information:

![screenshot](./out.gif)

## Installation

1. Clone this repo under **~/.config/awesome/**

    ```bash
    git clone https://github.com/streetturtle/awesome-wm-widgets.git ~/.config/awesome/
    ```

1. Require ram widget at the beginning of **rc.lua**:

    ```lua
    local ram_widget = require("awesome-wm-widgets.ram-widget.ram-widget")
    ```

1. Add widget to the tasklist:

    ```lua
    s.mytasklist, -- Middle widget
        { -- Right widgets
            layout = wibox.layout.fixed.horizontal,
            ...
            --[[default]]
            ram_widget(),
            ...
    ```
