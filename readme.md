# bluetoothctl + dmenu = :heart:

If you work in software, your work/life situation is probably a lot like mine right now. You wake up, do your morning things, sit down at your desk and awaken your machine, start some music, and work for 6 to 13 hours. Then you put that machine to sleep, grab a different machine and go into a different room with it, start some different music, and do your thing there until you pass out on the couch. Such is the extent of pandemic life most days.

The crucial thing here is the music. The moving from one room to another. You're probably using your bluetooth speakers a lot. You're probably sick of typing sequences like `bluetoothct<tab> <enter> connec<tab> <enter> 48<tab> <enter> exit <enter>` countless times a day.

So here's a little script of dubious utility to save you from all that. It's currently called `bluetooth` because you should never type this command. That would be counter to the spirit of this whole endeavor. Instead, put it somewhere your window manager can execute it and add two bindings, like:

    # For dis/connecting with bluetooth devices.
    bindsym $mod+b exec {path/to/}bluetooth connect
    bindsym $mod+Shift+b exec {path/to/}bluetooth disconnect

Also, ensure your system has `notify-send` and `dmenu` (or equivalent). Also, `ruby`.

With this installed, when you move the couch for the evening, you can just type something like `$mod+b kilbur<enter>` and get on with it. You're welcome.

## But why?

Some of you may be asking: Why would you ever want to do any of this when you could just use the bluetooth applet in the panel? And I'd answer: I guess we have less in common than I thought.
