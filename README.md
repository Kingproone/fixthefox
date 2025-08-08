# Fix The Fox! 🦊

> [!IMPORTANT]
> Use a fork of firefox that does a lot of privacy/security enhancements out of the box, like [Librewolf](https://librewolf.net/), [Mullvad](https://mullvad.net/en/browser) or [Tor](https://www.torproject.org/download/) for the desktop. [Ironfox](https://gitlab.com/ironfox-oss/IronFox) or [Tor](https://www.torproject.org/download/#android) for Android.

<details>

**<summary> Clean up the default UI! </summary>**

This takes 1 minute to do and will give ```6,8%``` plus usable space on screen

| Firefox on second run (on first run the left sidebar is not added), bars take up ```10.55%``` of the screenshot | Cleeeeean, bar takes up ```3,75%``` of the screenshot |
| --- | --- |
| ![default-ff-on-2nd-open](https://github.com/user-attachments/assets/888c82e0-c4b4-4c7f-a7f4-ea251d649276) | ![clean-ff](https://github.com/user-attachments/assets/55ec9588-cae9-4350-9205-7ce9f8b02e42) |

</details>

<details>

**<summary> Icons for context menus. </summary>**

https://github.com/black7375/Firefox-UI-Fix

</details>

<details>

**<summary> Picture in picture window doesn't stay above others on kde. </summary>**

1. Right click an open Picture-in-Picture window. In the context menu, select "More Actions" -> "Configure Special Window Settings...".

2. Click "Add Property..." and select "Window title". The newly added row's text field should read "Picture-in-Picture". Change the dropdown option from "Unimportant" to "Exact Match". (All PiP windows in Firefox use this title and by making it Exact Match the rule shouldn't affect any other Firefox windows.) 

3. Click "Add Property..." again and this time select "Keep above other windows". The dropdown in the newly added row should be set to "Apply Initially". Select the "Yes" radio button if it isn't already.

4. Click "OK". That's it. No more manually setting Keep Above every time you open a PiP.

NOTES:

1. [The original reddit thread of the fix.](https://www.reddit.com/r/kde/comments/osjt3p/firefox_wayland_pip_workaround_or_how_i_learned/)

2. For me the "Keep above other windows" line disappeared after setting it and reopening the config window. After going in and out of PiP a few times and redoing the setup it stuck around.

3. The upcoming fix: [wayland pip protocol support](https://bugzilla.mozilla.org/show_bug.cgi?id=1970372).

</details>

<details>

**<summary> Remove search icon drop down </summary>**

It hides the lock and shield icon to check site info

1. Open ```about:config```

2. Search for: ```browser.urlbar.scotchBonnet.enableOverride```

3. Change from ```true``` to ```false```

[Article with the fix](https://www.askvg.com/tip-enable-upcoming-address-bar-search-ui-in-firefox-right-now-scotch-bonnet-project/)

</details>

<details>

**<summary> Tablet UI </summary>**

1. Open ```about:config```
  
2. Search for: ```browser.uidensity```
 
3. Set it to: ```1```

</details>

<details>

<summary>  </summary>

</details>
