# inputactions-kwin-config

My config for 3-finger gestures using InputActions for KWin. It essentially acts like the default 3-finger gestures do on Windows.

## Installation/Setup

1. Install [taj-ny/InputActions](https://github.com/taj-ny/InputActions). Instructions for KWin [here](https://wiki.inputactions.org/main/getting-started/installation/kwin.html).
2. Download `config.yaml` and plop it in `$HOME/.config/inputactions`.
3. Enable InputActions per the documentation.
4. Profit.

## Gestures

### Alt+Tab (Swipe Left/Right)

Swipe left or right with 3 fingers. Hold your fingers on the trackpad until you have found the window you want. Swiping right cycles forward through the switcher; left cycles backwards. You can happily switch directions during your stroke, and the switcher will act accordingly. The switcher will close as soon as you lift your fingers.

This gesture holds down Alt while hitting Tab or Shift+Tab to shift through the switcher, and releases Alt at the end of the stroke.

### Show/Hide Overview (Swipe Up)

Show the overview by swiping up with 3 fingers. Swipe down to close the overview. Or, you can swipe up again. Either works.

### Show Desktop (Swipe Down)

Swipe down with 3 fingers to show the desktop. Swipe down again to show your windows.

**NOTE:** Swiping up while showing the desktop will open the overview rather than restoring your windows. InputActions does not expose a variable that detects when "Show Desktop" is active, and I have not found a reliable way to detect this otherwise. InputActions also lacks the ability to set custom variables during runtime. There is probably a way to do this using a shell command, but I've honestly been too lazy to figure it out.

## Issues

If anyone has improvements or suggestions to improve this config, feel free to open an issue or submit a pull request.
