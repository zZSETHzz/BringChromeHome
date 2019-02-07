# BringChromeHome
The original Chrome OS installer

This project is slowly being merged into Project Croissant (https://github.com/imperador/chromefy)

You can find us at the Telegram Group:
https://t.me/chromeosforpc
   > Please, ask your questions at the group and don't PM the admins. :)
   
You can also follow us on Twitter: https://twitter.com/CroissantDev

## Observations

  - You must have somewhat closely matching hardware to the ChromeOS install chosen later.
    > You will need TPM 2.0 for all TPM 2.0 Chrome installs.
    > you will need a closely matching CPU. No support for AMD currently
    > GPU support is extremely limited and as such onboard are the only recommended display adapters to use.
  - You need a Chromium installation running
    > We strongly recommend using [ArnoldTheBats Chromium](https://chromium.arnoldthebat.co.uk/index.php?dir=special&order=modified&sort=desc) Stable builds.
    > Just deploy the img to a USB Stick, [Rufus](https://rufus.ie/en_IE.html) and similar programs will do the work.
  - You have to be logged in (because if you don't, the initial setup won't work).
  - We are not responsible for any damage made to your computer by you or by your dog.
  - Updating
    > Auto updates do not work however running the install script again will check for if a newer build is available and offer the option to update. If no update is available it offers the option to clean install the same build.
---

# Install

Boot into Chromium OS and open the developer console

> CTL + ALT + F2


you may need to alternate ALT and F2 while holding CTRL.

Here you will need to type the command:

> sudo su

Then you will need to follow the prompts for username and password. Username= chronos Password=*leaveblank*

Type the following command

> bash <(curl -s -L https://bit.ly/2MTr9Tn)

you will now be given the options to select a build of Chrome OS, each build is for a different Chromebook/Chromebox and so hardware varies with each choice. Find a complete list with numbers here!

Pick the build of Chrome OS you would like to install by typing the corresponding number and pressing enter. 

The script will then begin to download and install Chrome OS for you, this will take about 2 minutes on a 120Mb internet connection.

Once the script has finished running you are ready to reboot.

(You will know if the script has finished running as you won't be able to exit the developer console by pressing

> CTRL + ALT + F1

Reboot and you will now have Chrome OS installed!!!


If Chrome OS then does NOT boot, try the newer version, Project Croissant (https://github.com/imperador/chromefy)


## NOTE 1:

 Be aware that booting Chrome OS will produce a message regarding malformed ID's. This is simply from a health check upon boot, simply close this and continue using Chrome OS. This poses no risk or issues. METHOD TO BYPASS IS UNDER INSTRUCTIONS.


## NOTE 2:

Once Chrome OS has been installed and you have logged in you may receive an error stating that your account has been used on a higher build number than the current install, all this means is that your user profile has been loaded from the chromium OS install from earlier and as chromium OS uses a newer source code, Chrome OS thinks you have downgraded, to fix this simply go into settings -> advanced settings -> power wash, let this run for about two minutes and you will be good to go. YOU WILL LOSE ALL DATA WHEN DOING THIS!
