# Budgie Wayland session

This project contains the scripts and data files for setting up the Budgie Desktop
to run in a Wayland environment.

## Requirements

There are a number of runtime requirements for various aspects of this project:

### Desktop

This requires [Budgie Desktop] and [Magpie v1].

Additionally, we make available sessions for Kwin (`kwin_wayland`) and Miriway. These are strictly for development / testing purposes and should not be considered officially supported by Buddies of Budgie. You will receive no assistance nor issue resolution for any compositor other than Magpie V1.

- When using [KWin], KWin 6.0.0 or newer is required.
- When using [Miriway], Miriway 24.10 or newer is required.

### SDDM

This requires [SDDM] 0.21.0 and [Layer Shell Qt] 6.0.0 or newer. SDDM needs to be built
with Qt 6 for both the core and the greeter.

### Anaconda Initial Setup (optional)

If your distribution ships [Anaconda Initial Setup], you need version 0.3.99 or newer.

# Licensing

Copyright © 2024 Neal Gompa.

Copyright © Buddies of Budgie Contributors.

This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.
If a copy of the MPL was not distributed with this file, You can obtain one at
https://mozilla.org/MPL/2.0/.

[Budgie Desktop]: https://github.com/BuddiesOfBudgie/budgie-desktop
[Magpie v1]: https://github.com/BuddiesOfBudgie/magpie/tree/v1
[KWin]: https://invent.kde.org/plasma/kwin
[SDDM]: https://github.com/sddm/sddm
[Layer Shell Qt]: https://invent.kde.org/plasma/layer-shell-qt
[Anaconda Initial Setup]: https://github.com/rhinstaller/initial-setup
[Miriway]: https://github.com/Miriway/Miriway
