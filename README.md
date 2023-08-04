# ROG-ALLY-Debloat-Optimization-

everything in this guide is YOUR OWN RISK I am not responsible for anything.

Above all, you will need several things:
- a USB flash drive of minimum 16GB
- USB-C hub with 3 USB-A input
- keyboard
- mouse


First, you need to update and install ALL available drivers via MYASUS/ArmoryCrate/WindowsUpdate.
I also recommend installing all the drivers presented on the drivers page for the ROG ALLY below.

https://rog.asus.com/gaming-handhelds/rog-ally/rog-ally-2023/helpdesk_download/


It is imperative to do this because we will Backup all drivers for the following changes.
Once you are ready, create a "drivers" folder in the C: drive at its base.
the path to this folder will be "C: drivers"

We will now use the following command to backup all drivers.
Launch the Windows terminal with administrator rights and paste this line:


dism/online/export-driver/destination:"C:\drivers"

Now let’s create a bootable USB drive
using the windows 11 lean verson "GhostSpectre Superlite SE"

Follow the procedure provided by the creator via this link:

https://ghostclouds.xyz/wp/w11-22h2-22621/

Download version 13, also install Rufus & 7-zip on their respective site.

- https://rufus.ie/en/#
- https://www.7-zip.org

The GhostSpectre Superlite SE iso is compressed to form . U13
You have to extract the iso via 7-zip and put it where you want.
The password is: 22h2u13

Then create a bootable USB drive from the iso with Rufus, leave the default settings.

When the bootable usb drive is ready, paste the folder "c: drivers" to the root of the usb drive.
This will allow us to reinstall them once GhostSpectre Superlite SE is installed.

Before you can start the installation you must disable the following settings in your ROG ALLY Bios:

- Fastboot
- Secureboot

To do this, restart your Ally and hold the volume button - when the animated logo starts at startup.

Here are the two options to disable:


![IMG_5015](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/f5b81703-1cdf-4662-881f-8f75f684116b)
![IMG_5016](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/c186c217-dc9d-413a-8650-b19c8d7a47b5)

save and exit.

Restart in the bios again, You will now be able to choose the bootable usb drive in the boot options visible at the bottom of the screen.

You can follow the instructions in this video for ease when installing the bone:

https://youtu.be/iSoxPFaXBn0?t=510

Choose Superlite SE or Superlite SE + WD if you want to keep Windows Defender.
When the installation is done, congratulations you have made the basis of your new OS!

We now need to import all the essential drivers for the ROG-Ally.
To do this, copy and paste the drivers folder of your usb drive to the root of your C: 
Open Powershell as administrator and paste the following command line:

pnputil /add-driver "C:\drivers\*.inf" /subdirs/install/reboot

Let powershell do its magic and restart your ROG-ALLY


Superlite SE does not have a default browser installed ( bye Edge ) so start Ghost Toolbolx which is on your desktop and install the browser of your choice.
For example for Chrome, press 14 on your keyboard and enter (it is imperative to be connected to the internet for this).
I also recommend doing options 16 and 17.

![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/a2b96bd0-adc7-4959-a444-b4c9ef6b16b6)


You must also activate the Touch Keyboard.
For this do option 20 then 3 and restart.
You can then activate it via windows settings, set them as below.

![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/ba4a934f-22be-42e4-8da3-eec4836693e6)

Then you have to install Armoury Crate. Simply press the button on your Rog Ally to launch it, a window opens, you can download and install it.

Our Base is ready and functional.
I also recommend using Chris’s tool to complete our optimization.

https://github.com/ChrisTitusTech/winutil

Follow its instructions and once the tool is open, check these options in "Tweaks":

![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/cd4f8e3b-3d26-43b0-8bbb-1037360e0358)

click on Run Tweaks, when it’s done, re-launch your Rog-ALLY.

I recommend creating a "Games" folder at the root of your C: drive where you will install all your games and game launcher (Steam,GoG,..) before making the next option.
We will compress our windows installation via Ghost toolbox options. 

So start Ghost Toolbox which is on your desktop and choose option 9 then 1.

![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/a2b96bd0-adc7-4959-a444-b4c9ef6b16b6)
![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/369768ad-6c6b-4109-9d42-a95aca3a510e)

The operation can take more than 10 minutes, do not touch anything during the operation and keep the ROG ally connected.

Restart your ROG ally again once the operation is complete.

If you want this office style:

![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/6e8876bb-f4b6-4afb-a02a-1c12a582b69d)

Right click on your task bar, properties and configure the options like this (I set the resolution to 720P personally):

![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/901fe9ef-31b0-4577-ae70-361e8afda9f9)
![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/96854cc0-b640-48ed-a70d-6afd82c2eec8)
![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/aab06634-b0a8-4e12-aee4-d85d6856c613)

Don’t forget to disable programs at startup if you don’t need them like steam, chrome,...
Creating personalised profiles in Armoury crate is also recommended. Here are my examples:

![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/491f6742-11d1-4bb9-849f-003b1a323cf7)
![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/b629669a-9333-49b8-889c-af4de94c9506)
![image](https://github.com/Oganir/ROG-ALLY-Debloat-Optimization-/assets/141415073/b3ae0018-9848-444b-99f2-da364e1d6cae)

Your ROG is de-optimized and will not be slowed down by Windows.














