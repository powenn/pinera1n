# pinera1n
<a href="https://www.pine64.org/pinephone/" >
  <img src="https://www.pine64.org/wp-content/uploads/2020/05/PinePhone-3.jpg" height="320"/>
</a>

## Jailbreak method with Linux phone 

This is a great way to make checkra1n portable, since it runs on PinePhone. You can use the latest GUI release of checkra1n, and you can operate it with the phone's touchscreen! It's called pinera1n because it was tested on PinePhone, which was inexpensive and very useful! Using `apt-get` or `pacman` on your Linux distribution will work. Recently, the default OS on PinePhone has become Manjaro, so you won't need to flash a new OS to use this on your PinePhone. However, I've also tested Arch and Mobian.

**NOTE:Odysseyra1n also works. In addition, other Linux phones should work,too. This tool is called pinera1n because it first succeeded on a PinePhone. Please contact me on [Twitter](https://twitter.com/powen00hsiao) if your Linux distribution uses a different package handling system than `apt-get` or `pacman`.**

## Demo 

![Demo photo][1]
![Demo photo][2]
![Demo photo][3]

## What's new
`Add quick setup to setup `all dependencies` and `download cheeckra1n` with less commands`

## Hardware you'll need
- [A pinephone](https://www.pine64.org/pinephone/)
- USB-C docking bar with a USB-A to Lightning and USB-C charging port(**Use USB-A to Lightning to connect the iPhone**)
- USB-A to Lightning cable
- USB-C charging supply

## Hardware you might need
- Micro-SD card
- a card reader

## Supported Linux distributions(those that I have tested)
**`apt-get` distributions**
- [latest release of mobian image](https://mobian-project.org)

**`pacman` distributions**
- [latest release of manjaro image](https://wiki.pine64.org/wiki/PinePhone_Software_Releases#Manjaro_ARM)
- [latest release of arch image](https://github.com/dreemurrs-embedded/Pine64-Arch/releases)

## Software you need 
- xterm(for resize terminal size)
- usbmuxd(must need to connect iphone correctly)
- [Latest checkra1n release for linux arm64](https://checkra.in)
-  a terminal program can set scale of terminal window(default program should work)


### Software needed for odysseyra1n support
- curl
- libusbmuxd-tools(libusbmuxd)

## Getting Started
You can select Quick setup or Manually setup
## Quick setup 
If you are flashing a different OS, please follow this [tutorial](https://wiki.pine64.org/wiki/PinePhone_Installation_Instructions).

Use this to setup `all dependencies` and `download cheeckra1n` with two commands

after run these commands,checkra1n will locate at Home and already got permission

- for `apt-get`
```
sudo apt-get update && sudo apt-get -y upgrade && sudo apt-get install curl
```
```
sudo /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/powenn/pinera1n/main/for-apt-get.sh)"
```

- for `pacman`
```
sudo pacman -Syu && sudo pacman -S curl
```
```
sudo /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/powenn/pinera1n/main/for-pacman.sh)"
```

## Manually setup
Please follow these steps carefully so you can use your PinePhone to jailbreak instead of a computer.

### A. Flash os to emmc or sd card 

If you are flashing a different OS, please follow this [tutorial](https://wiki.pine64.org/wiki/PinePhone_Installation_Instructions).

### B. Install dependencies

1. Perform available updates:

**For `apt-get`:**
```
sudo apt-get update
sudo apt-get upgrade
```
**For `pacman`:**
```
sudo pacman -Syu
```
Reboot your device. 

2. Install xterm and usbmuxd.

**For `apt-get`:**
```
sudo apt-get install xterm usbmuxd
```
**For `pacman`**
```
sudo pacman -S xterm usbmuxd
```
3. **If you want to use odysseyra1n,** install curl and libusbmuxd-tools(libusbmuxd)

**For `apt-get`**
```
sudo apt-get install curl libusbmuxd-tools
```
**For `pacman`**
```
sudo pacman -S curl libusbmuxd
```
4. Now, give checkra1n permission to run.
```
cd Downloads
chmod +x checkra1n
```
Exit terminal and re-open it.

5. Set the terminal size and scale, so that we can run checkra1n with GUI. This will make it be more friendly to use.

Set the terminal scale to 50%, then enter this command:
```
resize -s 80 24
```

### C. Run checkra1n 
Connect your iPhone to your PinePhone via the docking bar. Make sure you charge your pinephone via docking bar for a stable connection. If your iPhone asks you to verify access to device, allow it.

Open and run checkra1n with this command:

default downloaded checkra1n loaction should in Downloads 
```
cd Downloads/checkra1n
sudo ./checkra1n
```

If needed, change checkra1n's options (such as allowing untested versions). You should see the start button available. Follow checkra1n's instructions to complete the jaibreak.

If you're not using odysseyra1n yet and want to, keep going.Don't open the checkra1n loader app on your iPhone.

## Odysseyra1n Conversion Instructions

Make sure you've already installed the optional dependencies for odysseyra1n. Then, enter this:
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/coolstar/Odyssey-bootstrap/master/procursus-deploy-linux-macos.sh)"
```

This will require your iPhone's root password (which is `alpine` by default)

Once it finishes, you'll see Sileo on your iPhone, so you can install/update libhooker, RocketBootstrap, etc.

## Advantages of pinera1n
- Portable and friendly to operate with full GUI and touchscreen
- You can still do more than jailbreak your iPhone on the PinePhone
- It's not crazy expensive, and the PinePhone doesn't need to be jailbroken.
- Setup instructions are simple, and it's straightfoward after setup.
- checkra1n officially supports Linux on ARM, so it works better than Android would 
- You can use the latest release of checkra1n on pinephone immediately.
- **odysseyra1n works on pinephone**
- **pinera1n supports multiple Linux distributions**

## Demo video
These are simple videos just showing what it looks like to use it:
### Mobian
<a href="https://www.youtube.com/watch?v=M5mNpY8a2zM">
  <img src="https://img.youtube.com/vi/M5mNpY8a2zM/maxresdefault.jpg" >
</a>

### Manjaro
<a href="https://www.youtube.com/watch?v=0EkEFZlKQUE">
  <img src="https://img.youtube.com/vi/0EkEFZlKQUE/maxresdefault.jpg" >
</a>

## Tutorial video(odysseyra1n on mobian)
This video provides instructions in so that it's easier to follow.

<a href="https://www.youtube.com/watch?v=Ite65xLu4TE">
  <img src="https://img.youtube.com/vi/Ite65xLu4TE/maxresdefault.jpg" >
</a>

## My posts on Twitter 

[checkra1n successed on mobian](https://twitter.com/powen00hsiao/status/1421803816421257227)

[sideload with pinehphne test (using appsync)](https://twitter.com/powen00hsiao/status/1422377286393729028)

[cydia impactor 64bit on pinephone mobian with chroot(but cannot connect to iphone)](https://twitter.com/powen00hsiao/status/1427641693856272385)

[checkra1n successed on arch](https://twitter.com/powen00hsiao/status/1424192009825263620)

[checkra1n successed on manjaro](https://twitter.com/powen00hsiao/status/1424230136518352908)

[odysseyra1n successed on manjaro](https://twitter.com/powen00hsiao/status/1425100540971716613)

## My repo
My repo for jailbreak tweaks is here: [powen00hsiao repo](https://powenn.github.io/powen00hsiao/)

## Introduce pinephone
From wiki :The PinePhone is a smartphone developed by Hong Kong-based computer manufacturer Pine64, intended to allow the user to have full control over the device. Measures to ensure this are: running mainline Linux-based mobile operating systems, assembling the phone with screws, simplifying the disassembly for repairs and upgrades, and providing six kill switches/security switches for components of its hardware.The PinePhone ships with the Manjaro Linux-based operating system using the Plasma Mobile graphic interface, although other distributions can be installed by users.

# CONTACT ME ON [TWITTER](https://twitter.com/powen00hsiao) FOR QUESTIONS!

<a href="https://twitter.com/powen00hsiao">
  <img src="https://pbs.twimg.com/profile_images/1404649867033550848/3m6kzjQa_400x400.jpg" height="320"/>
</a>


[1]:https://github.com/powenn/pinera1n/blob/main/photos/01.png
[2]:https://github.com/powenn/pinera1n/blob/main/photos/02.png
[3]:https://github.com/powenn/pinera1n/blob/main/photos/03.png
