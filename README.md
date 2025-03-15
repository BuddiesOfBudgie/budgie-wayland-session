# Budgie Wayland session

This project contains various scripts and data files used by the Buddies of Budgie team to facilitate **testing** Budgie Desktop against a wide range of Wayland compositors.

### Important

**None** of the compositors referenced in this repository should be viewed as endorsed by the team for use with Budgie Desktop. Budgie Desktop may not function fully or at all with any compositors referenced in this repository.

You will receive **no** assistance nor issue resolution for any compositor that is not considered to be supported by the team. In the event a compositor is viewed by the team as suitable for use with Budgie Desktop, any files related to it shall be moved to budgie-desktop itself.

## Layout

### desktop/

This contains various session files and any supplemental files used to get Budgie Desktop to _potentially_ function or run with a range of compositors, for example:

- [KWin] (`kwin_wayland`)
- [Magpie v1] ("v1" development branch)
- [Miriway]

**Requirements:**

- [Budgie Desktop]
- When using [Magpie v1], v1 branch is required.
- When using [KWin], KWin 6.0.0 or newer is required.
- When using [Miriway], Miriway 24.10 or newer is required.

### initial-setup/

This contains any files used to test Anaconda Initial Setup with magpie ("v1" development branch) in kiosk mode. Do **not** build or use this unless you are intentionally performing magpie v1 testing with Anacoda Initial Setup specifically.

**Requirements:**

- [Magpie v1]
- [Anaconda Initial Setup] 0.3.99 or newer.

### sddm/

This contains any files used to test SDDM with magpie ("v1" development branch). Do **not** build or use this unless you are intentionally performing magpie v1 testing with SDDM specifically.

**Requirements:**

- [Magpie v1]
- This requires [SDDM] 0.21.0 and [Layer Shell Qt] 6.0.0 or newer. SDDM needs to be built with Qt 6 for both the core and the greeter.

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
