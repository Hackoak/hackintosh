
# ⚙️ USB Tethering Setup

- Install the `Pacifist` Application.
- Open the `USB/HoRNDIS-9.2.pkg` with the Pacifist Application.
- Extract the kext under the HoRNDIS-9.2 Contents/HoRNDIS-kext Contents/Library/Extensions/HoRNDIS.kext 
- Quit Pacifist.
- I Already done that you can see that Under USB Folder.
- Open Terminal and run the following command. Replace that path with your kext file.

```
sudo cp -R /Path/to/HoRNDIS.kext /Library/Extensions
```
- When `System Extension Updated` Dialog appear, click the `Open Security Preferences`
- Go to Privacy & Security and click Allow/Open Anyway.
- Click on Not now when prompt appears.
- Run the following command
```
sudo kextcache -i/
```

- Restart and enjoy 🎉
