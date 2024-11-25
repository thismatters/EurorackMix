# Mix

Audio signal mixing. Basic module with simple OP Amp design.

The KiCAD project here uses the library/footprints [found in my companion repo](https://github.com/thismatters/EurorackKiCAD).

## Size

30hp on a 1u rack.

## Inputs

4x patch inputs and 4x potentiometers for adjusting the apparent effect of a patch input

## Outputs

Single 1/4" phone jack output.
4 LED array indicating output level.

## Notes

LED array takes some cues from the [MFOS Multifunction Module](https://musicfromouterspace.com/analogsynth_new/MULTIFUNCTIONMODULE/pdf/mfm_schempg1_schem.pdf)

## Vendors

There are part numbers in the [BOM](mix.csv) for many of the parts (not for basic passives though) at the following vendors:

* [Mouser](https://www.mouser.com): Needs no introduction. Get your ICs from here (or [digikey](https://www.digikey.com)).
* [Tayda Electronics](https://www.taydaelectronics.com/): Good supplier for passive components; audio jacks, and potentiometers. Their audio jacks are slightly smaller than the thonkiconn from thonk.
* [Love My Switches](https://lovemyswitches.com/): Has [really good knobs](https://lovemyswitches.com/anodized-aluminum-knob-the-lo-fi-1-4-smooth-shaft-12-5mm-od/) to go on those potentiometers!
* [OSHPark](https://oshpark.com/): Fast and (relatively) cheap PCB manufacturer. The [V0 circuit](https://oshpark.com/shared_projects/xlEAsl8K) works pretty well as a mix, but the output level indicator doesn't quite work right, there will be another version.


## Changelog

### V1
- [x] Adds full bridge rectifier to output level indicator
- [x] Adds capacitor and resistor to output level indicator
- [x] Removes capacitor from output op amp
- [x] Updates design langage