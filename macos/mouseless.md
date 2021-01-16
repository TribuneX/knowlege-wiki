# Mouseless

I started thinking about how I could use my mouseless (there is actually an [app](https://gumroad.com/l/Dwka) called mouseless) and my keyboard more while using my Mac. I was facinated by a guy mastering Vim with his keyboard. So I decided to start looking into how I could avoid using my mouse (actually my trackpad) for most of the task such as switching between windows or browser tabs and especially within apps.

This is an overview of the areas keyboard shortcuts save me a lot of time and effort:

## macOS

### Window Manager

I use [Divvy](https://mizage.com/divvy/) for resizing windows and moving them from one screen to the other.
I use shortcuts to resize windows to fullscreen, to center them in a smaller window and to use two apps side by side (down and up for my vertical screen).

Doing a shortcut twice will send the window to the second screen. I heavily use this feature, which is missing for other window manager (like [rectangle](https://rectangleapp.com))

### App Switching

It took me some years to actually understand the `command+tab` behavior of macOS. I often wondered, why switching to a certain app does not open it. It turns out, `command+tab` does not work for minimized windows. So keep in mind: never minimize an app window! Just keep them as they are and switch to another app by `command+tab`. However, for some apps I often have multiple windows open (e.g. Intellij). Therefore, I need to be able to switch between windows of the same app.
There is a shortcut option called: Move focus to the next window. I use `command+^`for this.
TL:DR: Use `command+tab` for switching between apps and `command+^` to switch between open windows of the same app.

### Safari

In Safari my most commonly task is to open a new tab and search for something. This can be either done by opening a new tab first `command+t`, type the search query and hit enter. Or a shorter way is to use Alfred for this by using the keyword `g` and typing the query. Honestly, I want to always use Alfred for this, but I still find myself opening Safari and using `command+t` still too often!

Going back to the previous page can be achieved by `command+left-arrow`

Another daily used shortcut is `command+w` which closes the current tab and lets me quickly cleanup my open tabs.
Safari supports navigating between tabs, but I use the Alfred worflows [browser tabs](https://github.com/epilande/alfred-browser-tabs) instead, which gives me quick access to all open tabs by name. I use the shortcut `option+tab` for this.

### General

Sent my Mac to sleep can be done via `command+option+eject`. I often close tabs of apps with `command+w`. I also often close the whole app with `command+q`
I think there a many shortcuts yet to be discovered for macOS.

## Apps

### Todoist

Todoist is always available with `command+ä`. I have know idea why I initially have choosen 'ä' for this, 
but it is now part of my muscle memory.

### Intellij

You can be so much faster by learning the shortcuts for all the various actions in Intellij. Especially, the refactoring shortcuts are worth to explore! Listing all the shortcuts I use in this app would be too much work!

### 1Password

One password trigger is set to `option+q`. This is a risky shortcut, since it is really close to `command+q` which would close Safari instead.

## Missing parts

This is the interesting part, which is the actual reason I started this section! Here are the things I am still missing a working shortcut for:

- Right click for all apps: Especially for editing text, a right click shortcut would be really nice.
- Microsoft Teams does not have much shortcuts. So far I can only search for name with `command+f`. Nothing more.