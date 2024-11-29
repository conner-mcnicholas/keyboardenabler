On a new system, you will also need to create a file: /usr/share/applications/keyboard-on-off.desktop with contents:

[Desktop Entry]
Version=1.0
Type=Application
Name=keyboard-enable-disable
Icon=/home/conner/keyboardenabler/keyboardenabled.png
Exec=bash kbscript.sh
Path=/home/conner/keyboardenabler
NoDisplay=false
Categories=Utility;
StartupNotify=false
Terminal=false
X-Desktop-File-Install-Version=0.26

After that, run:
sudo desktop-file-validate /usr/share/applications/keyboard-on-off.desktop 
sudo desktop-file-install /usr/share/applications/keyboard-on-off.desktop
sudo update-desktop-database /usr/share/applications/

To launch from panel icon, you may need to find the new application within the main launcher, and manually add to favorites.
