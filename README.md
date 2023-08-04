# 7zip Auto Extract
A way to automatically extract zipped files by double clicking.
# The Process
1. Obviously you need 7zip installed.
2. Open RegEdit (Win+R, type regedit and press enter).
3. Navigate to Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Classes\Applications\7zFM.exe\shell\
4. There should be a folder with the default command (mine is called "Extract"). Inside that folder, click on "command".
5. On the right pane, double click the "(Default)" key. I would recommend making a backup of the default command just in case you ever want to go back.
6. Replace the Value Data with this command. "C:\Program Files\7-Zip\Extract_Open.bat" "%1"
7. You can close RegEdit. Open File Explorer.
8. Navigate to "C:\Program Files\7-Zip\".
9. Download Extract_Open.bat from this repo and put it in the folder you navigated to in step 8. You are done, enjoy!
