# Sapphire-HD-7790-Dual-X-OC
UEFI support using custom firmware created with GOPUpd (https://www.win-raid.com/t892f16-AMD-and-Nvidia-GOP-update-No-requests-DIY.html)

![UEFI-Firmware](https://user-images.githubusercontent.com/44642574/110239232-37784800-7f46-11eb-9c00-0ba98150c40f.png)
# Why
- Open bios, bootmanager, fastboot, WHQL
- For me mainly in order to boot with macOS on Hackintosh
# Disclaimer
In the worst case your GPU is bricked permanently after following these steps. I am not responsible for any damage. Follow at your own risk! Do not use on any other model!
# Read this
You may wan't to patch the firmware youself. However since this is currently the newest version i don't see any benefit. Just make sure you have the same model.
# Steps
- Download https://www.techpowerup.com/download/ati-atiflash/
- Open amdvbflashWin.exe with admin (Takes a few seconds until window pop's up)
- Click on the save button and save (Takes again a few seconds, then a success message should show up)
- Save your backup vbios on another other PC or Cloud so you can use another pc to recover if GPU breaks and blind recovery is not working either
- Put your vbios and 113-253OCH-X005_updGOP.rom into your atiflash folder
- Edit line 34 to the path to match your atiflash folder in recover.bat and gop_update.bat (do not remove brackets)
- Edit line 35 in recover.bat to match your vbios name with file ending in name!
- Start the gop_update.bat for GOP firmware update
- Now wait until the flash is complete. It will take a few seconds, do not do anything while flashing!
- Restart your machine to complete the update. Now you should be able to enable WHQL support in your bios ;D
- (Use recover.bat for blind stock firmware flash)!
