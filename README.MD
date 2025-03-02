# dmenu-record

Screencast on Xorg with FFmpeg with cool options using any dmenu-compatible menu.
I have also included a dictaphone (voice notes) which is almost the exact thing,
but the default variables are different.

## Features

- Sreen recording
    - Active screen
    - Selection
    - Entire workspace (multi-head)
        - Optionally different video tracks for each monitor (y/n)
- Audio
    - Record desktop audio (y/n)
    - Record microphone audio (y/n)
    - If both enabled:
        - Separate audio tracks (y/n)

## Dependencies

- dmenu or anything compatible (examples below)
- ffmpeg
- xrandr
- xdotool
- slop
- pulseaudio (or pipewire-pulse)
- pactl
- a notification daemon

## Examples

```sh
# --print the arguments instead of recording and quit
dmenu-record --print # only for demenu-record

# you can change the default, dmenu, for rofi. Example:
DMENU_RECORD_DMENU="rofi -dmenu -i -window-title" dmenu-record
```
