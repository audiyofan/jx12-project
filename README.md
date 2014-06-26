# JX12 Project

JX12 was a secret audio project, this is why it has such stupid name. Since it is a public work, all the content in the repo is under the Creative Common CC-BY-SA licence. This means you can share the work, enhance the work, use it for commercial purposes but you cannot change its license nor strip my name from it.

    Copyright 2014 - Grégoire HUBERT

This work implies the use of **LETAL VOLTAGES** causing severe injuries or death. You have been warned.

## What is this secret audio project ?

This work is based on an original idea from Arnaud Heagele on [René Conseil's forum](http://6bm8-lab.fr/phpBB/viewtopic.php?f=3&t=170 [6B8M]). This comes from a [Bell Lab patent](http://www.google.fr/patents?id=lTN8AAAAEBAJ&pg=PA2&hl=fr&source=gbs_selected_pages&cad=4#v=onepage&q&f=false [original patent description]) in the 70s.

Instead of using a classical negative passive feedback it uses an active correction feedback. This dramatically lowers the output impedance and removes electronic coloration from the signal.

The model 400 is an evolution of the model 250 with more power. Using Russian transmission tubes GU19-1, it delivers almost 40W in 4Ω. The differential correction feedback is handled by a valve with more gain loaded by a FET cascode to block power supply's noise.

# Technical characteristics

 * Output power: 39W in 4Ω
 * THD 1kHz for 1W in 4Ω: -66dB
 * THD 1kHz for 35W in 4Ω: -55dB
 * Damping factor: > 31
 * Output impedance: 0.12Ω
 * Bandwidth -3dB @ 1W: 8Hz - 85kHz

All schematic informations and measures are made using Charly Doria's hand made output transformers model DA159. Using any other output transformer *will* lead to changes in the correction filters and may not work at all and turn the whole thing into a high frequencies power oscillator. (I had troubles up to 2.5MHz). It is possible to build this amplifier for 8Ω and 16Ω speakers using the same output transformer. 

![schematic](schematics/JX12.png)
