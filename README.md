# pinera1n

I think this is a great way to make checkra1n portable,runs on pinephone and you can use gui  oringinal latest release of checkra1n,and you can operate it with touchscreen ,It called pinera1n because it's checkra1n on pinephone,it's not a expensive but really useful phone,I had tested checkra1n on mobian,so I suggest user run checkra1n with mobian on pinephone,because it required usbmuxd ,others linux distribution might works with a bit different(if interesd about that ,contact me on twitter),it's the most important thing,without it ,iPhone won't connect correctly with pinephone ,now follow the steps to jailbreak with the awesome phone 

## Demo 
![Demo photo][1]
![Demo photo][2]
![Demo photo][3]

## Things you need(hardware and mobian image)
- [A pinephone](https://www.pine64.org/pinephone/)
- A usb-c docking bar (contain usb-A to lighting and usb-c charging port,must use usb-A to lightning connect iphone)
- usb-A to lightning
- charging supply with usb-c
- micro sd (optional)
- [latest image release of mobian image](https://mobian-project.org)

## Things you need on mobian
- xterm(for resize terminal size)
- usbmuxd(must need to connect iphone correctly)
- [latest checkra1n release for linux arm64](https://checkra.in)
- king's cross(terminal program on mobian)

## Getting  Start

Now following steps to get a friendly easily portable checkra1n ,with this while you lose jailbreak environment,just connect to pinephone,start with friendly gui to rejailbreak,don't need computer 

### Flash mobian to emmc or sd card 

First,you need to flash mobian to pinephone,check this [tutorial](https://wiki.pine64.org/wiki/PinePhone_Installation_Instructions)

### Perpare things will need on mobian

update it first 
```
sudo apt-get update
sudo apt-get upgrade
```
after these reboot

now install xterm and usbmuxd 
```
sudo apt-get install xterm
sudo apt-get install usbmuxd
```
now give checkra1n permission
```
cd Downloads
chmod +x checkra1n
```
exit terminal and re-open it ,now set the terminal size and scale ,so that we can run checkra1n with gui ,it will be more friendly to use 

`set terminal scale to 50 % first(set this with the menu on the right top corner) `
type this in terminal ,make sure W bigger than 80 and H 24
```
resize -s 80 24
```

### Now we can run checkra1n on pinephone 
connect iphone to pinephone through docking bar,make sure charge your pinephone when progress(charge with docking bar,must do this step ,without this connection will be unstable ),if iphone ask you to verify access to device ,select yes

open checkra1n and run it
```
cd Downloads
cd checkra1n
sudo ./checkra1n
```
if you are on untested version or something need to configure ,you can do that with optional,and you should see the start button avaliable,and follow checkra1n to complete jaibreak

## `Advantage of pinera1n`
- portable and friendly to operate with full GUI and touchscreen
- it's a linux phone ,so you can do others thing else,not just a phone for jailbreak
- it's a nice price for this awesome phone,with so much features only need 149 $ for standard pack
- just one command ,and you can get root easily in terminal
- you can underatand well how to do ,because it just need to conncet phone and phone
- with the offical support for linux on arm,it works better than android 
- you can use the latest release of checkra1n on pinephone
- no  complex progress,most of steps on phones

## Demo video
just show how I do it ,might post another video as tutorial video
[demo video](https://www.youtube.com/watch?v=M5mNpY8a2zM)


## My repo
my repo for jailbreak tweaks [powen00hsiao repo](https://powenn.github.io/powen00hsiao/)

## Introduce pinephone
from wiki :The PinePhone is a smartphone developed by Hong Kong-based computer manufacturer Pine64, intended to allow the user to have full control over the device. Measures to ensure this are: running mainline Linux-based mobile operating systems, assembling the phone with screws, simplifying the disassembly for repairs and upgrades, and providing six kill switches/security switches for components of its hardware.The PinePhone ships with the Manjaro Linux-based operating system using the Plasma Mobile graphic interface, although other distributions can be installed by users.

It's a phone with arm architecture,and run different linux distribution,with linux ,you can do  something cool, like make checkra1n being portable with friendly GUI ,this phone is not expensive,for standard pack only 149 $,spent less than most android phone,but you can have GUI to operate checkra1n easily

# IF YOU HAVE ANY QUESTION,CONTACT ME ON [TWITTER](https://twitter.com/powen00hsiao)

[1]:https://github.com/powenn/pinera1n/blob/main/photos/01.png
[2]:https://github.com/powenn/pinera1n/blob/main/photos/02.png
[3]:https://github.com/powenn/pinera1n/blob/main/photos/03.png
