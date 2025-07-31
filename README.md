# Fix The Fox!

> [!IMPORTANT]
> Use a fork of firefox that does a lot of privacy/security enhancements out of the box, like [librewolf](https://librewolf.net/), [mullvad](https://mullvad.net/en/browser) or [tor](https://www.torproject.org/download/) for the desktop. [Ironfox](https://gitlab.com/ironfox-oss/IronFox) or [tor](https://www.torproject.org/download/#android) for Android.

<details>

<summary>Picture in picture window doesn't stay above others on kde </summary>

1. Right click an open Picture-in-Picture window. In the context menu, select "More Actions" -> "Configure Special Window Settings...".

2. Click "Add Property..." and select "Window title". The newly added row's text field should read "Picture-in-Picture". Change the dropdown option from "Unimportant" to "Exact Match". (All PiP windows in Firefox use this title and by making it Exact Match the rule shouldn't affect any other Firefox windows.) 

3. Click "Add Property..." again and this time select "Keep above other windows". The dropdown in the newly added row should be set to "Apply Initially". Select the "Yes" radio button if it isn't already.

4. Click "OK". That's it. No more manually setting Keep Above every time you open a PiP.

NOTES:

 - a. [The original reddit thread of the fix.](https://www.reddit.com/r/kde/comments/osjt3p/firefox_wayland_pip_workaround_or_how_i_learned/)

 - b. For me the "Keep above other windows" line disappears after setting it and reopening the config window.

</details>
