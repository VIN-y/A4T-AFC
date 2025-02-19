[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

# A4T-AFC: [A]nother [4]010 [T]oolhead - [A]nother [F]ilament [C]utter

## BETA Release

A toolhead cutter mod from: [![ko-fi](docs/images/Ko-fi_smol.png)](https://ko-fi.com/southash1) [SouthAsh1](https://ko-fi.com/southash1)



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
| 2   | M3 x 8 BHCS                                   | To attach the `Cutter Arm` and `Blade Holder` to the cowl.|
| 5   | M3 Threaded Heat Insert                       | Standard Voron spec: M3 x 5 x 4|
| 2   | M5 x 10 BHCS                                  | For attaching the `Depressor Arm Base`|
| 2   | M3 x 10 BHCS / SHCS & 2 Washers               | To attach the `Depressor Arm` to the base.|
|     | **OPTIONAL**
| 4   | M2.5 x 8 FHCS                                 | To mount the hotend for ONLY the UHF options.|


## Printing parts
### Print settings
Parts are meant to be printed in 0.2mm layer heights, 0.25mm first layer should be OK. Other layer heights will cause the built-in supports to fail or fuse to the printed part.<br/>
Print settings will depend on your printer setup / filament used / phase of the moon/etc.<br/>
The parts are not pre-scaled for any particular filament type. You will need to tune the filament you use for correct shrinkage compensation to get good results. Development was done with multiple brands of ASA and ASA-CF filaments (each individually tuned).<br/>

General voron-like settings are a good starting point for 0.4mm wall widths (four walls, 5 top/bottom layers and 40% infill).<br/>
The print setup was tested with 0.5mm nozzle printing 0.55mm line widths with 3 walls and 40% infill with good results.<br/>

⚠If you have any under-extrusion you will have problems with the parts stretching and mot keeping rigidity.⚠

(Same rules of A4T applies here so I kind of copied and pasted, sue me...)


## Assembly
### Assembly Steps


These istructions should be followed in conjunction with original <a href="https://github.com/Armchair-Heavy-Industries/A4T">A4T instructions</a>.

:information_source: CW2 and Tap users have to build the toolhead on the printer, Xol Carriage users can build off the printer.
| <center>Notes</center>                                                                                                | Images|
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-----: |
| Prep the M2 inserts for install by drilling them out with a 5/64 or 2mm Drill Bit, then in one of them chamfer the top and the other chamfer the bottom. | <img src='docs/images/m2_drilled.png' width=650><br/> |
| **Preping the Blade Holder** |
| Start by using a pair of vise grips, a pair of pliars, or a vise that can firmly grasp the blade and prevent it from moving. | <img src='docs/images/blade_grasp.png' width=650><br/> |
| Next, using flush cutters, cut the tab on the back `⚠⚠ flying parts ⚠⚠` and start triming the plastic off one side. | <img src='docs/images/trimming_plastic.png' width=650><br/> |
| When you get enough plastic off one side then the other side can just be pulled off then you will get a clean blade ready for install. | <img src='docs/images/clean_blade.png' width=650><br/> |
| There are alternate types of Bambu blades that may differ depending on where on the globe you buy them on, they will still work. | <img src='docs/images/alternate_blade.png' width=250><br/> |
| With the blade still in the vise grips, slide it into the Blade Holder. It will be tight but that is by design. Install the M2 FHCS making sure you don't overtighten as it's going into plastic. | <img src='docs/images/blade_install.png' width=650><br/> |
| **Preping the Extruder Adapter** |
| Install the M2 insert that is chamfered on the bottom into the Extruder Adapter. | <img src='docs/images/m2_adapter.png' width=650><br/> |
| **Cutter Install** |
| Before installing, CW2 and Tap users need to install the cowl to the carriage now. |
| UHF users will need to use `M2.5x8 FHCS` to install the hotend. |
| Insert the M3 inserts | <img src='docs/images/m3_inserts.png' width=650><br/> |
| Insert the M2 insert that is chamfered on the top into the cowl making it flush with the surface. | <img src='docs/images/m2_cowl.png' width=650><br/> |
| Carefully install the Blade Holder with an `M3x8 BHCS`. You can use thread locker in the brass insert. ⚠⚠ Do not use the brand Loctite if you are printing with ABS, I recommend Vibra-Tite. ⚠⚠ | <img src='docs/images/blade_holder.png' width=650><br/> |
| Install the Cutter Arm again with an `M3x8 BHCS`. You can use some thread locker in the brass insert here. ⚠⚠ Be sure not to get any thread locker on the intended moving parts. ⚠⚠ | <img src='docs/images/cutter_bar.png' width=650><br/> |
| Install the Link with 2 `M3x4 BHCS`, loosening the screws where needed to allow the parts to freely move. | <img src='docs/images/link.png' width=650><br/> |
| Using some tweasers install the spring, being sure to secure the ends into the holes. Test out the mechanism to make sure it resets with no binding. | <img src='docs/images/spring.png' width=650><br/> |
| Last the Extruder adapter can be installed and secured with an `M3x6 SHCS`. The rest of A4T instructions can be continued. | <img src='docs/images/extruder_adapter.png' width=650><br/> |

<br>

### 

### Credits
* Thanks to everyone that supported my last project/mod.
* Thanks to DW-Tas for all the help provided and for designing <a href="https://github.com/Armchair-Heavy-Industries/A4T">A4T</a>.

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
