# localed-x11-sync
A script for controlling X11 system keyboard layouts using the systemd-localed DBus API. This script should run as a service and reflect any configuration done to the systemd-localed in any currently running X11-based desktop environment.

# Reasoning
This script was created for Fedora (primarily spins) to enable the Anaconda installer to control keyboard layout changes in the Live ISO environment. The systemd-localed DBus was chosen for this purpose because Wayland systems lack a centralized keyboard management system and because it's available everywhere in the Fedora.

However, this script can be used outside of Fedora for similar purposes (e.g., SDDM) if needed.

# Sources
This script is based on the work of [alebastr](https://github.com/alebastr), who generously provided the [script used for Sway](https://github.com/alebastr/sway-systemd/blob/dd738a987c3e388070e49d90cf0edbd92977ad7f/src/locale1-xkb-config). A big thanks to him!
