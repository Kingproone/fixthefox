# Fix The Fox! 🦊

> [!IMPORTANT]
> Use a fork of Firefox that does a lot of privacy/security enhancements out of the box, like [Librewolf](https://librewolf.net/), [Mullvad](https://mullvad.net/en/browser) or [Tor](https://www.torproject.org/download/) for the desktop. [Ironfox](https://gitlab.com/ironfox-oss/IronFox) or [Tor](https://www.torproject.org/download/#android) for Android.

<details>

<summary><b>Clean up the default UI!</b></summary>

This takes 1 minute to do and will give ```6,8%``` plus usable space on screen

| Firefox on second run (on first run the left sidebar is not added), bars take up ```10.55%``` of the screenshot | Cleeeeean, bar takes up ```3,75%``` of the screenshot |
| --- | --- |
| ![default-ff-on-2nd-open](https://github.com/user-attachments/assets/888c82e0-c4b4-4c7f-a7f4-ea251d649276) | ![clean-ff](https://github.com/user-attachments/assets/55ec9588-cae9-4350-9205-7ce9f8b02e42) |

</details>

<details>

<summary><b>Icons for context menus.</b></summary>

https://github.com/black7375/Firefox-UI-Fix

I recommend the Proton style.

</details>

<details>

<summary><b>Picture in picture window doesn't stay above others on kde.</b></summary>

### Plasma [6.5](https://invent.kde.org/plasma/kwin/-/merge_requests/7954)+ & Firefox [141](https://bugzilla.mozilla.org/show_bug.cgi?id=1970372)+

1. Create a shell script in the Plasma autostart env folder, since [PIP is off by default](https://blog.broulik.de/2025/06/pimp-your-clock/):
```
mkdir -p ~/.config/plasma-workspace/env/
echo 'export KWIN_WAYLAND_SUPPORT_XX_PIP_V1=1' > ~/.config/plasma-workspace/env/kwin-pip.sh
chmod +x ~/.config/plasma-workspace/env/kwin-pip.sh
```

2. Log out and back in to apply.

> `widget.wayland.experimental.pip.enabled` is on by default in Firefox 149

#### Legacy fix

copy of [the original reddit thread of the fix.](https://www.reddit.com/r/kde/comments/osjt3p/firefox_wayland_pip_workaround_or_how_i_learned/)

1. Right click an open Picture-in-Picture window. In the context menu, select "More Actions" -> "Configure Special Window Settings...". This will populate most of the window settings for you.

2. Click "Add Property..." and select "Window title". The newly added row's text field should read "Picture-in-Picture". Change the dropdown option from "Unimportant" to "Exact Match". (All PiP windows in Firefox use this title and by making it Exact Match the rule shouldn't affect any other Firefox windows.) 

3. Click "Add Property..." again and this time select "Keep above other windows". The dropdown in the newly added row should be set to "Apply Initially". Select the "Yes" radio button if it isn't already.

4. Click "OK". That's it. No more manually setting Keep Above every time you open a PiP.

5. Restart your browser

</details>

<details>

<summary><b>Remove search icon drop down.</b></summary>

It hides the lock and shield icon to check site info

1. Open ```about:config```

2. Search for: ```browser.urlbar.scotchBonnet.enableOverride```

3. Change from ```true``` to ```false```

[Article with the fix](https://www.askvg.com/tip-enable-upcoming-address-bar-search-ui-in-firefox-right-now-scotch-bonnet-project/)

</details>

<details>

<summary><b>Tablet UI</b></summary>

1. Open ```about:config```
  
2. Search for: ```browser.uidensity```
 
3. Set it to: ```1```

</details>

<details>

<summary><b>Too short bookmark folder selection window</b></summary>

This helps me organize my bookmarks a LOT

1. Make sure you have userChrome.css support enabled:

- Go to ```about:config```
- Search for ```toolkit.legacyUserProfileCustomizations.stylesheets```
- Set it to ```true```

2. The file should be in the correct location:

- Go to ```about:support```
- Find ```Profile Directory``` and click ```Open Directory```
- Create a folder named ```chrome``` if it doesn't exist
- Create/edit ```userChrome.css``` inside the chrome folder

3. Add the following code to the file:
```
#editBMPanel_folderTree {
  height: auto !important;
  min-height: 400px !important; /* Adjust this value as needed */
}
```
4. Restart Firefox

NOTES

- llms were used in figuring this out
- with a cleaned UI, no horizontal taskbar and a 1080p screen ```700px``` works great, ymmv, try and see what works best

| Before | After |
| --- | --- |
| ![before](https://github.com/user-attachments/assets/dbf32601-370c-4d41-a514-0706658aad4b) | ![after](https://github.com/user-attachments/assets/44fe18a1-2d1a-441b-826a-7a913b9c7016) |

</details>

<!---Placeholder section to copy--->

<details>

<summary><b>placeholder</b></summary>

</details>
