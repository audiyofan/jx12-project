# JX12 Project

JX12 is a secret audio project, this is why it has such stupid name. 

## What is this secret audio project ?

This work is based on an original idea from Arnaud Heagele on [René Cariou's forum](http://6bm8-lab.fr/phpBB/viewtopic.php?f=3&t=170 [6B8M]). This comes from a [Bell Lab patent](http://www.google.fr/patents?id=lTN8AAAAEBAJ&pg=PA2&hl=fr&source=gbs_selected_pages&cad=4#v=onepage&q&f=false [original patent description]) in the 70s.

This is a very standard valve push pull amplifier using very common (and cheap) tubes. Instead of using a normal negative feedback it uses an extra valve to create a correction feedback. This particularity dramatically lowers the output impedance to levels rarely seen with valve amplifiers while not decreasing the gain. According Arnaud's experimentations, the output damping factor equals approximately the amplification factor of the correction tube. In this case, the 6N16B valve gives us an amplification factor of 20 which means a output impedance of 0,4Ω with 9,7W output power in 8Ω. 

## About the construction

### Power supply

The power supply is a critical part of this project and it deserves a lot of attention. Two parts do depend directly from the power supply :

 * The correction valve: any noise from the PSU will find itself on this valve's anode hence re-injected on the 6N2P (high gain) triode's grid with the input signal.
 * The cathode follower: it is auto-biased and it creates the polarisation for the power tubes. A 1V shift from the PSU will result on power tubes 1V bias shift.

Since the power tubes are pentodes, they are pretty immunised to noise except on their g2 grid. For the sake of simplicity it has been chosen to use a simple regulated power supply. Several of them have been tested but silicium is really sensitive to heat, this means no zener (unstable AND noisy) nor current diodes. The best choice is [Yves Monmagnon's regulated PSU](http://www.dissident-audio.com/RegulHT/Regul.html) which has been tested successfully to be reliable and stable in addition of beeing simple.

### Correction filters

The correction filters are really important since they directly determine what will be summed in the triode. As the output transformer is not linear, it has a great impact on the filters performances. The output transformer used is a DA17 from [bobinaudio](http://montagnaise.free.fr/transformateurs.html). The potentiometer is here to fine tune the bandwidth. An extra filter composed of 22nF + 2,2kΩ in the correction circuit proved to be successful in preventing the amplifier to oscillate at high frequencies. The resulting bandwidth is excellent between 20Hz and 20kHz.

![schematic](schematics/JX12.png)
