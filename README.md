# Sapphire-HD-7790-Dual-X-OC GDDR5 1GB UEFI
UEFI support with official vbios
- Create DIY update for another graphics card (This did also work for me before the official update): GOPUpd (https://www.win-raid.com/t892f16-AMD-and-Nvidia-GOP-update-No-requests-DIY.html)

![update](https://user-images.githubusercontent.com/44642574/110971550-4fdbce80-835b-11eb-9b90-8a539106c231.PNG)

# Why
- Open bios, bootmanager, fastboot, WHQL
- For me mainly in order to boot with macOS on Hackintosh
# Disclaimer
In the worst case your GPU is bricked
permanently after following these steps. I am not responsible for any damage. Follow at your own risk! Do not use on any other model!
# Important
Make sure you **have** the **same gpu model**. **READ the WHOLE README** before you do anything!
# Steps
- Download this respository
- Download https://www.techpowerup.com/download/ati-atiflash/
- Open amdvbflashWin.exe with admin (Takes a few seconds until window pop's up)
- Click on the save button and save (Takes again a few seconds, then a success message should show up)
- Save your backup vbios on another other PC or Cloud so you can use another pc to recover if GPU breaks and blind recovery is not working either
- Put your vbios and 253X03H0.UO1 into your atiflash folder
- Edit line 34 to the path to match your atiflash folder in flash_stock.bat and flash_update.bat (do not remove brackets)
- Edit line 35 in flash_stock.bat to match your vbios filename with file ending in name!
- Start the flash_update.bat for GOP firmware update
- Now wait until the flash is complete. It will take a few seconds, do not do anything while flashing!
- Restart your machine to complete the update. Now your gpu should have UEFI support ;D
- (Use recover.bat for blind stock firmware flash: You can launch it with WinR, then type the full path to flash_stock.bat and press enter)
