KodiLauncher
============

This is just Jacob Johnston's XbmcLauncher updated to launch Kodi.
Please read his blog post on XbmcLauncher here: http://inchoatethoughts.com/launching-xbmc-with-a-windows-media-center-remote

[Download](https://github.com/LenAnderson/KodiLauncher/blob/master/bin/Release/KodiLauncher.exe?raw=true)

Manual Install
--------------
We need to change permissions on the default launcher so we can copy over it:
  1. Go to "C:\Windows\ehome"
  2. In the "ehome" directory, right click "ehshell.exe" and choose "Properties"
  3. Click on the "Security" tab and click on the "Advanced" button at the bottom.
  4. Click on the "Owner" tab and click the "Edit" button.
  5. Select "Administrators" and hit "OK."
  6. Click "OK" in the "Advanced Security Settings for ehshell.exe" dialog.
  7. In the "ehshell.exe Properties" dialog, click on "Administrators" under "Group or user names" and click the "Edit" button.
  8. Select "Administrators" (or add that group if it isn't already there) and check the "Full Control" box in the Allow column.
  9. "OK" out of all the properties and permissions dialogs.
  10. While in "C:\Windows\ehome", copy ehshell.exe and paste it somewhere safe as a backup, in case you ever need to restore.

Now, we can copy the new launcher.
  11. Rename "KodiLauncher.exe" to "ehshell.exe"
  12. Copy and Paste the new "ehshell.exe" into the "C:\Windows\ehome" directory.

Now when you press the start button on your Windows media remote, it will launch Kodi instead.

OPTIONAL: Command Line Arguments
  13. If you want to add command line arguments, place a file named "KodiLaunchArgs.txt" in the "C:\Windows\ehome" directory.
  14. The contents of the text file should be the command line arguments you would like to run with.
