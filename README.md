# tokipona-keyboard
Toki Pona unicode keyboard layout

<div align="center"><img src="https://github.com/alinajafi/tokipona-keyboard/blob/main/sc7%20Toki%20Pona%20layout.jpg" style="width: 80%;"></div>

**Disclaimer:** This is not an application. This is just a keyboard layout for HeliBoard – an open source keyboard application which supports custom layouts. This can be good or bad for you. On the positive side, you can use it simply alongside other keyboard layouts.


The process has two general stages: 

1) Installing the unicode font, 
2) Adding the keybord layout.

<h3>If you can see this character: 󱥢 it means you have already enabled the font and you can skip to stage 2.</h3>

<h1>Stage 1. Installing the unicode font</h1>

The best font that I can guarantee to work with the keyboard layout is <code>nasin-nanpa</code> by jan Itan:

1. Download the UCSUR version of the font: https://github.com/etbcor/nasin-nanpa/releases

3. Use ```zfont``` to install the font on your device – if supported. You can follow instructions [here](https://www.reddit.com/r/tokipona/comments/10bwbur/guide_on_viewing_and_rendering_sitelen_pona_on/).


<h3>If you have a MIUI Xiaomi device</h3>

Some Toki Pona font packages are already submitted by me and will be published soon hopefully. (Not yet on Jan 19th, 2025)

<h3>If you have root access</h3>

You can easily install the font using <code>ADB</code>.

After enabling <code>ADB shell</code>, or using Terminal on the device, type the following cammands to copy the font to the system directory replacing an unused font of yours – here for example the Coptic version:

```su```

```mount -o remount,rw /system```

```cd /sdcard/path/to/folder```

```cp nasin-nanpa*.ttf /system/fonts/NotoSansCoptic-Regular.ttf```

<h1>Stage 2. Adding the keyboard layout</h1>

At first, you need to install [HeliBoard](https://f-droid.org/en/packages/helium314.keyboard/) from F-Droid. It is an open source alternative to GBoard and you can use it for other languages too.

Then, download the [layout file](https://github.com/alinajafi/tokipona-keyboard/blob/main/Toki%20Pona.json) and add it to HeliBord:

1. Go to the app ```settings``` by holding comma (,)

2. Open ```Languages & Layouts``` section

3. At the bottom of the list, enable ```No language (Alphabet)```
  
4. Disable the default ```QWERTY``` and tap on ```+``` to add a layout (pic. left)

5. Tap on ```Add Custom Layout``` (pic. right)
<div align="center">
  <img src="https://github.com/alinajafi/tokipona-keyboard/blob/main/sc1%20No%20Language.jpg" style="width: 45%;">        
  <img src="https://github.com/alinajafi/tokipona-keyboard/blob/main/sc2%20Add%20layout.jpg" style="width: 45%;">
</div>  

6. Select ```Load File``` and select the downloaded layout file (pic. left)

7. Set a name for the layout.  
It will be shown on the space key, so you may want to set it as Toki Pona (pic. right)

<div align="center">
  <img src="https://github.com/alinajafi/tokipona-keyboard/blob/main/sc3%20Load%20file.jpg" style="width: 45%;">        
  <img src="https://github.com/alinajafi/tokipona-keyboard/blob/main/sc4%20Layout%20name.jpg" style="width: 45%;">
</div>  

8. Additionally, on the page from step (4) you had better to change ```popup key order``` and ```hint source``` options.

   For popup keys, disable all sections ecxept ```Layout```.     
   For hint source, disable all sections or optionally leave ```Layout``` enabled – this will hint additional press-and-hold characters.

<div align="center">
  <img src="https://github.com/alinajafi/tokipona-keyboard/blob/main/sc5%20popup%20key%20options.jpg" style="width: 45%;">       
  <img src="https://github.com/alinajafi/tokipona-keyboard/blob/main/sc6%20hint%20source%20options.jpg" style="width: 45%;">
</div>  

</br>
Your layout is ready. Enjoy!
