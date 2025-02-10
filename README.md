[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

# A4T-AFC: [A]nother [4]010 [T]oolhead - [A]nother [F]ilament [C]utter
A toolhead cutter mod from: [![ko-fi](docs/images/Ko-fi_smol.png)](https://ko-fi.com/southash1) [SouthAsh1](https://ko-fi.com/southash1)

[![Join me on Discord](https://discord.com/api/guilds/1029426383614648421/widget.png?style=banner2)](https://discord.gg/armchairengineeringsux)

<img src='docs/images/main_render.png' width=800 />


<br/> 
A filament cutter mod designed around the A4T that is designed by DW-Tas. Focused on keeping the original size as close as possible while still keeping the build relatively simple. <br/><br/>



> [!NOTE] 
> ### Total WIP<br/>
> This mod is still a WIP and some things may change, most changes will be minor. Also the CAD will come out later.<br/>

<br/><br/>

> [!WARNING]
> ### Very Sharp  
> This project requires you to modify very sharp objects. I will cover how to handle these when I get to finishing the instalation instructions very soon. 

<br/>

## Bill of Materials (BOM)
***`*Not including stock A4T hardware`***
| Qty | Item                                          | Notes                        |
| --- | --------------------------------------------- | ----------------------------------------------------------------------------------------- |
| 1   | Bambu Blade                                   | This mod uses a Bambu Labs filament cutter blade that has been stripped of its plastic. <a href="https://us.store.bambulab.com/products/replacement-filament-cutter?_pos=1&_ss=r">Bambu Blade</a>|
| 1   | 0.5x4x15 Spring                               | Any spring that is 4mm in diameter and no longer than 15mm should work your milage may vary for cutting force needed.|
| 1   | M2 x 4 FHCS                                   | Keeps the blade from sliding in and out.|
| 2   | M2 `Flange` Heatsets                          | This is the bread and butter of tolerances for the build. (<a href="https://www.digikey.com/en/products/detail/tri-star-industries-inc/HM20X157C/14205393">Digikey</a>) (<a href="https://www.aliexpress.us/item/3256805733805809.html">Ali Express</a>)|
| 1   | M3 x 6 SHCS                                   | Holds the Bridge on.|
| 2   | M3 x 4 BHCS                                   | For the `Link` between the `Cutter Arm` and `Blade Holder`.|
| 2   | M3 x 6 BHCS                                   | To attach the `Cutter Arm` and `Blade Holder` to the cowl.|
| 5   | M3 Threaded Heat Insert                       | Standard Voron spec: M3 x 5 x 4|
| 2   | M5 x 10 BHCS                                  | For attaching the `Depressor Arm Base`|
| 2   | M3 x 10 BHCS / SHCS & 2 Washers               | To attach the `Depressor Arm` to the base.


## Printing parts
### Print settings
Parts are meant to be printed in 0.2mm layer heights, 0.25mm first layer should be OK. Other layer heights will cause the built-in supports to fail or fuse to the printed part.<br/>
Print settings will depend on your printer setup / filament used / phase of the moon/etc.<br/>
The parts are not pre-scaled for any particular filament type. You will need to tune the filament you use for correct shrinkage compensation to get good results. Development was done with multiple brands of ASA and ASA-CF filaments (each individually tuned).<br/>

General voron-like settings are a good starting point for 0.4mm wall widths (four walls, 5 top/bottom layers and 40% infill).<br/>
The print setup was tested with 0.5mm nozzle printing 0.55mm line widths with 3 walls and 40% infill with good results.<br/>

(Same rules of A4T applies here so I kind of copied and pasted, sue me...)


## Assembly
### Assembly Steps

These are to come, please bear with me. Some stuff when installing are tight, I know they are on purpose. All will be explained once the instructions are done.

<br>

### 

### Credits
* Thanks to everyone that supported my last project/mod.
* Thanks to DW-Tas for all the help provided and for designing A4T.

Go support the guys over at <a href="https://github.com/Armchair-Heavy-Industries">Armchair Heavy Industries</a> as they are making some awesome stuff over there!


## Enjoy using A4T-AFC
This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

### License clarification regarding non-commercial use:
The non-commercial aspect of this license is for cases where A4T is the product, not the use of A4T to create products.<br/>
I.e. If you wish to sell A4T as a product, you would need to seek a commercial license before doing so. </br>
It is NOT intended to prevent the use of A4T in a printer that you use to provide commercial services. If you want to run A4T as a toolhead for your print farm printers, go right ahead.
