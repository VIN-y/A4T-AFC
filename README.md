[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

# A4T-AFC: [A]nother [4]010 [T]oolhead - [A]nother [F]ilament [C]utter

## BETA Release

A toolhead cutter mod from: [![ko-fi](docs/images/Ko-fi_smol.png)](https://ko-fi.com/southash1) [SouthAsh1](https://ko-fi.com/southash1)



<img src='docs/images/main_render.png' width=800 />


<br/> 
A filament cutter mod designed around the A4T that is designed by DW-Tas. Focused on keeping the original size as close as possible while still keeping the build relatively simple. <br/><br/>

I will try to get the board mounts made soon.



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
| 2   | M2 `Flange` Heatsets                          | This is the bread and butter of tolerances for the build. <br/> Recommended: ---<a href="https://www.digikey.com/en/products/detail/tri-star-industries-inc/HM20X157C/14205393">Digikey</a> <br/> Alternative: --------<a href="https://www.aliexpress.us/item/3256805733805809.html">Ali Express</a>|
| 2   | 3 x 10 mm pin                                 | Pivot pins for the `Link`<br/> Example: <a href="https://www.amazon.com/uxcell-Stainless-Cylindrical-Support-Elements/dp/B07Y58VWDW?th=1">Amazon</a>|
| 2   | 3 x 12 mm pin                                 | Pivot pins for the `Cutter Arm` and `Blade Holder`<br/> Example: <a href="https://www.amazon.com/uxcell-Stainless-Cylindrical-Support-Elements/dp/B07Y58CFYF?th=1">Amazon</a>|
| 4   | 3 ID x 5 OD x 5 H mm Sleeve Bearings                  | Bearing surfaces for the pins to guide on. <br/> Example: <a href="https://www.amazon.com/uxcell-Bearings-Wrapped-Bushings-Machinery/dp/B0CW31938R?th=1">Amazon</a>|
| 1   | M3 Threaded Heat Insert                       | Standard Voron spec: M3 x 5 x 4|
| 1   | M3 x 6 SHCS                                   | Holds the `Extruder Adapter` on.|
|     | **OPTIONAL**                                  |
| 4   | M2.5 x 8 / M2.5 x 12 FHCS                     | To mount the hotend for ONLY the UHF options. 12mm length if you are using the spacer.|
|     | **Extruder Mounting Screws**                  |
|     | WWBMG, Orbiter                                | 2-`M3x18 SHCS`|
|     | WWG2                                          | 1-`M3x20 SHCS` 1-`M3x18 SHCS`|
|     | Sherpa                                        | 2-`M3x24 BHCS` Sorry but you need to file/sand down 1mm on 25mm screws.|


## Printing parts
### Print settings
> [!WARNING]<br/>
> Recommended to print the `Link` and `Blade Holder` with 100% infill.<br/>

Parts are meant to be printed in 0.2mm layer heights, 0.25mm first layer should be OK. Other layer heights will cause the built-in supports to fail or fuse to the printed part.<br/>
Print settings will depend on your printer setup / filament used / phase of the moon/etc.<br/>
The parts are not pre-scaled for any particular filament type. You will need to tune the filament you use for correct shrinkage compensation to get good results. Development was done with multiple brands of ASA and ASA-CF filaments (each individually tuned).<br/>

General voron-like settings are a good starting point for 0.4mm wall widths (four walls, 5 top/bottom layers and 40% infill).<br/>

⚠ If you have any under-extrusion you will have problems with the parts stretching and not keeping rigidity. ⚠

(Similar rules of A4T applies here so I kind of copied and pasted, sue me...)

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
| Insert 2 of the `Sleeve Bearings` into the `Blade Holder` | <img src='docs/images/blade_holder_bearings.png' width=650><br/> |
| With the blade still in the vise grips, slide it into the Blade Holder. Install the M2 FHCS making sure you don't overtighten as it's going into plastic. | <img src='docs/images/blade_install.png' width=650><br/> |
| Insert the 2 remaining `Sleeve Bearings` into the `Cutter Bar` | <img src='docs/images/cutter_bar_bearings.png' width=650><br/> |
| Insert the 2 `3x10mm Pins` into the `Link` the pins will stick out the top with 5mm coming out the bottom. Picture is showing the bottom of the link. | <img src='docs/images/link_pins.png' width=650><br/> |
| **Preping the Extruder Adapter** |
| Install the M2 insert that is chamfered on the bottom into the Extruder Adapter. | <img src='docs/images/m2_adapter.png' width=650><br/> |
| **Cutter Install** |
| Before installing, CW2 and Tap users need to install the cowl to the carriage now. |
| UHF users will need to use `M2.5x8/12 FHCS` to install the hotend. |
| Insert the M3 insert | <img src='docs/images/m3_insert.png' width=650><br/> |
| Insert the M2 insert that is chamfered on the top into the cowl making it flush with the surface. | <img src='docs/images/m2_cowl.png' width=650><br/> |
| Insert the 2 `3x12mm Pins` into the cowl. | <img src='docs/images/pins_cowl.png' width=650><br/> |
| Carefully install the `Blade Holder` | <img src='docs/images/blade_holder.png' width=650><br/> |
| Install the `Cutter Arm` | <img src='docs/images/cutter_bar.png' width=650><br/> |
| Install the `Link` | <img src='docs/images/link.png' width=650><br/> |
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
