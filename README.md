# tokipona-keyboard
Toki Pona unicode keyboard layout

<div align="center"><img src="https://github.com/alinajafi/tokipona-keyboard/blob/main/screenshots/layout.jpg" style="width: 80%;"></div>  

</br>

**Disclaimer:** This is not an application. This is just a keyboard layout for HeliBoard – an open source keyboard application which supports custom layouts. This can be good or bad for you. On the positive side, you can use it simply alongside other keyboard layouts.


The process has two general stages: 

1) Installing the unicode font, 
2) Adding the keybord layout.

<h1>Stage 1. Installing the unicode font</h1>

The best font that I can guarantee to work with the keyboard layout is <code>nasin-nanpa</code> by jan Itan:

1. Download the UCSUR version of the font: https://github.com/etbcor/nasin-nanpa/releases

   Optionally, you can download alternative fonts combining Sitelen Pona fonts with Latin and Persian [here](https://github.com/alinajafi/tokipona-keyboard/tree/main/fonts).

3. Use ```zfont``` to install the font on your device – if supported. You can follow instructions [here](https://www.reddit.com/r/tokipona/comments/10bwbur/guide_on_viewing_and_rendering_sitelen_pona_on/).


<h3>If you have a MIUI Xiaomi device</h3>

There are some Toki Pona compatible font packages in ```Themes```. Just search for _Toki Pona_ or the font name, such as _nasin nanpa_. You'll find them.

<h3>If you have root access</h3>

You can easily install the font using <code>ADB</code>.

After enabling <code>ADB shell</code>, or using Terminal on the device, type the following cammands to copy the font to the system directory replacing an unused font of yours – here for example the Coptic version:

```su```

```mount -o remount,rw /system```

```cd /sdcard/path/to/folder```

```cp nasin-nanpa*.ttf /system/fonts/NotoSansCoptic-Regular.ttf```

<h1>Stage 2. Adding the keyboard layout</h1>

At first, you need to install [HeliBoard](https://f-droid.org/en/packages/helium314.keyboard/) from F-Droid. It is an open source alternative to GBoard and you can use it for other languages too.

Then, download the [layout](https://github.com/alinajafi/tokipona-keyboard/blob/main/layouts/Toki%20Pona.json) and add it to HeliBordl like this:

1. Go to the app ```settings``` by holding comma (,)

2. Open ```Languages & Layouts``` section

3. At the bottom of the list, enable ```No language (Alphabet)```
  
4. Disable the default ```QWERTY``` and tap on ```+``` to add a layout (pic. left)

5. Tap on ```Add Custom Layout``` (pic. right)
<div align="center">
  <img src="https://github.com/alinajafi/tokipona-keyboard/blob/main/screenshots/1%20No%20Language.jpg" style="width: 45%;">        
  <img src="https://github.com/alinajafi/tokipona-keyboard/blob/main/screenshots/2%20Add%20layout.jpg" style="width: 45%;">
</div>  

6. Select ```Load File``` and select the downloaded layout file (pic. left)

7. Set a name for the layout.  
It will be shown on the space key, so you may want to set it as Toki Pona (pic. right)

<div align="center">
  <img src="https://github.com/alinajafi/tokipona-keyboard/blob/main/screenshots/3%20Load%20file.jpg" style="width: 45%;">        
  <img src="https://github.com/alinajafi/tokipona-keyboard/blob/main/screenshots/4%20Layout%20name.jpg" style="width: 45%;">
</div>  

8. Additionally, on the page from step (4) you had better to change ```popup key order``` and ```hint source``` options.

   For popup keys, disable all sections ecxept ```Layout```.     
   For hint source, disable all sections or optionally leave ```Layout``` enabled – this will hint additional press-and-hold characters.

<div align="center">
  <img src="https://github.com/alinajafi/tokipona-keyboard/blob/main/screenshots/5%20popup%20key%20options.jpg" style="width: 45%;">       
  <img src="https://github.com/alinajafi/tokipona-keyboard/blob/main/screenshots/6%20hint%20source%20options.jpg" style="width: 45%;">
</div>  

</br>
Your layout is ready. Enjoy!

<h1>How does it work?</h1>

For now, other glyphs are accessible with press and hold. You can enable layout hints (step 8).

They are grouped almost alphabetical, i.e. words starting with the same one or two sounds are grouped together.  
Only ```nanpa``` and ```kule``` words are grouped according to their meanings.  

Here’s a color coded layout:

![color coded layout](https://github.com/alinajafi/tokipona-keyboard/blob/main/screenshots/color%20coded.png)

<table>
<tbody>
    <tr>
        <td>󱤂<br />󱤄󱤃󱤅󱤆</td>
        <td>󱤽<br />󱥳󱥮󱤼󱤭󱤄</td>
        <td>󱤰<br />󱦂󱤱󱤲󱦢</td>
        <td>󱤑<br />󱥿󱤐󱤓<br /></td>
        <td>󱥖<br />󱥚󱥙󱥗󱥘</td>
        <td>󱥱<br />󱥰󱥯<br /></td>
        <td>󱤖<br />󱤘󱤙󱤔󱤕󱤗</td>
        <td>󱥩<br />󱥧󱥨<br /></td>
        <td>󱥉<br />󱥋󱥌󱥊󱥈</td>
        <td>󱤡<br />󱦅󱥼󱤦󱤤󱤢</td>
        <td>󱥷<br />󱥳󱥶󱥴󱥵</td>
    </tr>
   <tr>
       <td>󱤀<br />󱤇󱤁󱤈</td>
        <td>󱤾<br />󱤿󱥀󱥸</td>
        <td>󱤴<br />󱦇󱤵󱤳󱥾</td>
        <td>󱥄<br />󱥺󱥆󱥅󱥇</td>
        <td>󱥞<br />󱥜󱥠󱥝󱥟󱥛</td>
        <td>󱤍<br />󱤏󱤌󱤎</td>
        <td>󱤛<br />󱥻󱤚󱥹󱦀</td>
        <td>󱥬<br />󱥾󱥮󱥪󱥫󱥭</td>
        <td>󱥍<br />󱥐󱥎󱥑</td>
        <td>󱤧<br />󱦤󱤩󱤪󱤨</td>
        <td>󱤉<br />󱦃󱤊󱤋</td>
    </tr>
    <tr>
        <td><br /></td>
        <td>󱥁<br />󱥂󱥃󱦆</td>
        <td>󱤶<br />󱥽󱤷󱤸</td>
        <td>󱤺<br />󱤼󱤻󱤹</td>
        <td>󱥡<br />󱥢󱦁</td>
        <td>󱥣<br />󱦦󱥦󱥤󱥥</td>
        <td>󱤜<br />󱦈󱤝󱤟󱤠</td>
        <td>󱤞<br />󱥲󱥏󱤒󱤫󱤣</td>
        <td>󱥔<br />󱥕󱥒󱥓</td>
        <td>󱤬<br />󱤯󱤭󱤮󱤥</td>
        <td><br /></td>
    </tr>
</tbody>
</table>

<h1>Special characters</h1>

<table>
<thead>
    <tr>
        <th>Character</th>
        <th>Unicode</th>
        <th>Position (Press & Hold)</th>
        <th>Shown As</th>
        <th>ShiftKey Status</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td><code>START OF CARTOUCHE</code></td>
        <td>U+F1990</td>
        <td>󱤑 jan</td>
        <td>󱦐</td>
        <td>− Disabled</td>
    </tr>
    <tr>
        <td><code>END OF CARTOUCHE</code></td>
        <td>U+F1991</td>
        <td>󱤑 jan</td>
        <td>󱦑</td>
        <td>− Disabled</td>
    </tr>
    <tr>
        <td><code>MIDDLE DOT</code></td>
        <td>U+F199C</td>
        <td>󱥰 uta</td>
        <td>󱦜</td>
        <td>− Disabled</td>
    </tr>
    <tr>
        <td><code>MIDDLE COLON</code></td>
        <td>U+F199D</td>
        <td>󱥰 uta</td>
        <td>󱦝</td>
        <td>− Disabled</td>
    </tr>
    <tr>
        <td><code>OPENING QUOTATION (te)</code></td>
        <td>U+F199E</td>
        <td>󱥩 tawa</td>
        <td>󱦞</td>
        <td>± Always</td>
    </tr>
    <tr>
        <td><code>CLOSING QUOTATION (to)</code></td>
        <td>U+F199F</td>
        <td>󱥩 tawa</td>
        <td>󱦟</td>
        <td>± Always</td>
    </tr>
    <tr>
        <td><code>COMBINING LONG GLYPH EXTENSION</code></td>
        <td>U+F1999</td>
        <td>󱥡 sona</td>
        <td>　󱦙</td>
        <td>− Disabled</td>
    </tr>
    <tr>
        <td><code>COMBINING CARTOUCHE EXTENSION</code></td>
        <td>U+F1992</td>
        <td>󱥡 sona</td>
        <td>　󱦒</td>
        <td>− Disabled</td>
    </tr>
    <tr>
        <td><code>END OF LONG GLYPH</code></td>
        <td>U+F1998</td>
        <td>󱥡 sona</td>
        <td>x</td>
        <td>− Disabled</td>
    </tr>
    <tr>
        <td><code>SCALING JOINER</code></td>
        <td>U+F1996</td>
        <td>󱤉 e</td>
        <td>󱤌󱦕󱥚</td>
        <td>− Disabled</td>
    </tr>
    <tr>
        <td><code>STACHING JOINER</code></td>
        <td>U+F1995</td>
        <td>󱤉 e</td>
        <td>󱤌󱦖󱤏</td>
        <td>− Disabled</td>
    </tr>
    <tr>
        <td><code>IDEOGRAPHIC SPACE</code></td>
        <td>U+3000</td>
        <td>󱤋 esun</td>
        <td>⇥</td>
        <td>+ Enabled</td>
    </tr>
    <tr>
        <td><code>LONG pi</code></td>
        <td>U+F1993</td>
        <td>󱥎 pilin</td>
        <td>󱦓</td>
        <td>− Disabled</td>
    </tr>
</tbody>
</table>
