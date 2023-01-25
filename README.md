# Amplex-MK-Presets
![BoxGraphic](https://user-images.githubusercontent.com/14950643/184476179-c898eccb-d922-41bf-8894-fc49fe7a0af7.png)

Various amp schematics translated into .TXT files, written for the guitar amp sim plugin "[Amplex]( https://nalexsoft.blogspot.com/2021/11/amplex-multiamp.html )" developed by [NaLex Software]( https://nalexsoft.blogspot.com ).

## IMPORTANT!
Only the preamp circuits are ported. As such, the Power Amp knobs in Amplex's GUI will not work, so you must add a 3rd party power amp sim after. Below are the ones I would recommend:
- [Ignite Amps TPA-1]( https://www.igniteamps.com/#tpa-1 )
- [NaLex PowerBox]( https://nalexsoft.blogspot.com/2020/05/powerbox-poweramp.html )
- [Nick Crow Lab TubeDriver]( https://nickcrowlab.blogspot.com/2009/08/tubedriver-v10.html )

This is an intentional decision as the impedance curve that is baked in Amplex's own power amp section might be undesirable for some who prefer to hear the full frequency range of the preamp circuits.

# Setting up the power amp
(Note that this is just an oversimplification of the technological explanations behind power amps to make this easier to explain.)

Power amps are very crucial in the overall sound because they add coloration and other aspects depending on the type. We will only cover tube-based power amps in this scenario as that's the kind of sound that people usually think "sounds realistic", when what it actually does is add more saturation and harmonic content to the preamp and certain low/high frequencies are accentuated due to the non-linear nature of tubes.

The settings will cover all of them. Recommended settings are provided in the screenshots below, with explanations for each control knob.

## Ignite Amps TPA-1
Image of the back panel (accessed via the right arrow)

![TPA-1_BackPanel](https://user-images.githubusercontent.com/14950643/208229905-fff65d6d-2ef5-40cc-b794-45e47218b327.png)

- ***Bias*** changes how much current is drawn to the power tubes. For standard/real world operation, keep it in its default range.
- ***Sagging*** allows you to dial the power amp compression to sound transparent and modern, or smooth and compressed similar to vintage amp tones. Set the knob to 2-3 for modern rectifier tones, 5 and above for vintage sag.
- ***Tubes*** gives you 3 type of power tubes to choose from. EL34 is common for British-voiced amps, 6L6 for American-voiced (California), and KT88 for German-voiced.
- ***Feedback*** makes the tubes either sound more linear or very rich with harmonics at the expense of the ***Depth*** and ***Presence*** knobs. For standard use, leave the knob at full for the Depth/Presence knobs to work as intended.
- ***Resonance*** will add a peak boost in the low frequencies and a shelf boost in the highs. This may vary greatly depending on the Impulse Responses that you use. But as a general rule, setting the knob at 5 is the common setting for real world amps, but cranking the knob will provide a more modern and scooped tone.

This is an oversimplification of the explanations provided in the manual.

## NaLex PowerBox

![PowerBox_UI_updated](https://user-images.githubusercontent.com/14950643/209920135-b824b420-8ce8-4fc3-b808-ec431f15e3c5.png)

The output is quieter than the preamp itself so I had to set the Input knob's value to 1.50 to compensate.
- ***Power*** adds more compression to the preamp, similar to the Sagging knob found in TPA-1
- ***Low*** behaves like the Resonance knob found in TPA-1.
- ***Presence*** is a bit more interactive with the frequencies compared to TPA-1
- The ***Freq*** knobs below ***Low*** and ***Presence*** allow you to adjust the frequencies that both knobs would affect. They're set to 85Hz and 1kHz, respectively.
- ***Bias*** functions the same as the one found in TPA-1. Setting the knob to 0 provides the hottest signal, and higher values will provide colder and lower output.
- ***Asym*** affects the dynamic behavior of the power amp. Setting to 0 will result in a solid state-like power amp sound, while cranking it to full will result in a more non-linear sound similar to standard tube amps.

## Nick Crow Lab - TubeDriver

![TubeDriver_UI](https://user-images.githubusercontent.com/14950643/211717010-a082b4b4-8dd4-49fc-940e-e8b5ea7814fa.png)

- Only the High Shelf band is enabled in the ***Pre EQ*** section. It is set to 1kHz to emulate the "Presence" knob found in some preamp circuits/power amps.
- ***Bias*** affects the compression of the power amp. Turn it all the way up for a very open sound, and vice versa for colder tones.
- ***Drive*** essentailly functions like the "Master Volume" that you would find in Class A power amps, so it will add a bit of distortion the more you turn it up. Adjust to taste.
- ***Volume*** is the output level. Adjust this along with the Drive knob to avoid clipping.
- The ***HP/LP Freq*** knobs shape the overall sound coming out of TubeDriver. I have set them to null for the full frequency range, but you may adjust them to remove low or high frequencies that you don't need.

# List of Amp Models
This collection covers a wide range of amplifier types based on gain amount, voicing, etc. This is never set in stone as I may add more amp models at any given time.

## Clean to Crunch
- 1950's Gibson Gibonette
- 1979 Roland JC-120 "3rd Edition" (re-translated into tube stages)
- 6V6 Plexi
- AX84 P1
- AX84 P1 eXtreme
- AX84 P1 Hi-Octane
- AX84 P1 Single-Ended Lead
- Bogen CHB-35A (Amp Conversion)
- Cameron CCV (2007, rev1)
- Fender Bassman 5F6-A
- Filmosound 385
- Fortin "Cali Mod"
- Hiwatt DR103
- Laney GH100TI Tony Iommi Signature
- Laney Supergroup 100 MK1 1969 build
- Magnatone 280a
- Marshall 1959 SLP "Dookie Mod"
- Marshall JMP 2203
- Marshall JTM45
- Marshall 200 1967 "Lead"
- Marshall Studio 15 4001
- Marshall Studio Vintage SV20H
- Matamp GT120
- Monoprice 15 (a.k.a. Harley Benton TUBE15)
- Pignose G40
- Pignose G60
- Reverend Kingsnake 20/60
- Selmer Treble and Bass MkII
- Sovtek MIG-50
- Sovtek MIG-60
- Sovtek MIG-100H
- Supro 1690T
- Trainwreck Express/Liverpool
- Trainwreck Rocket
- Yerasov Hammer Head

## High Gain and Beyond
- Friedman Dirty Shirley
- Friedman Pink Taco
- Marshall 1959 SLP "Jose Arredondo Mod"
- Marshall 200 1967 "Lead" ("Ritchie Blackmore" Cascade Mod)
- Marshall JCM900 SLX 2100
- Merlin Blencowe "Ultra High Gain"
- Orange Jim Root #4
- Peavey Windsor
- Secondary Lead (loosely based on the Sunn Beta series)
- Violet Delta Fuzz (original preset)
- Visio Aro Project Staalhoofd Mod
- Weighty Steel (circuit structure loosely based on the Boss HM-2 Heavy Metal pedal)

## Multi Channel
- Ampeg V4, 1970 (1971 VT-40 also shares the same preamp circuit)
- Ampeg V2, VT-40, V4, VT-22 Distortion Model, 1976
- Ampeg Lee Jackson VL-502/VL-1002
- AMT SS-11A & SS-11B
- AMT SS-11B Atomium Amplification Mod
- AX84 Firefly
- B-52 AT-100
- Bogner Triple Giant
- CAE 3+ Preamp
- Dumble ODS #094
- Dumble ODS #124
- Dumble ODS #183
- Duncan DDS-2250V
- ENGL E762/E765 Retro Tube 100
- ENGL Ritchie Blackmore Signature 100
- EVH 5150 III
- Fender '86 Red Knob Dual Showman
- Fender Machete
- Fender MH-500 Metalhead (re-translated into tube stages)
- Fender Prosonic
- Framus Cobra
- Friedman Small Box
- Henning Amps PlexRod
- Hughes & Kettner Triamp
- Ibanez Thermion TN120
- Jansen Amplifiers Gunn 50
- Kitty Hawk Junior Series I
- Kitty Hawk Quattro
- Koch Multitone I
- Krank Krankenstein
- Krank Chadwick 50w
- Laney AOR 100 Series II
- Laney GC30V
- Laney GH100L
- Laney Ironheart 120H
- Laney VH100R
- Lee Jackson Perfect Connection GP-1000 preamp
- Lee Jackson XLS-1000
- Marshall 1959RR Randy Rhoads Signature
- Marshall 6100 30th Anniversary
- Marshall JCM600
- Marshall JCM800 2210
- Marshall JCM900 4100
- Marshall JCM2000 DSL100
- Marshall JCM2000 TSL100
- Marshall JTM60
- Marshall JVM410H
- Marshall Silver Jubilee 2555
- Marshall SL5 Slash Signature
- Marshall Valvestate 8080/8100 (gain channel only, Contour knob not supported)
- Marshall Vintage Modern 2266/2466
- MESA/Boogie Lone Star/Lone Star Special
- MESA/Boogie Nomad 55/100
- MESA/Boogie Road King II
- MESA/Boogie Stiletto Stage II
- Metaltronix M-1000 Head
- MTA'02 (inspired by PRS MT15)
- Naylor Super-Drive 60
- Orange Rockerverb
- Orange Thunderverb
- Peavey Classic 20
- Peavey JSX 120
- Philipp Frank's homemade 18 Watt Plexi
- PRS SE 50
- Randall RGT100
- Randall Thrasher 50 (gain channel only)
- Rivera Knucklehead
- Rivera S-120/M60/M100
- Silvertone 1484
- Soldano SP-77 (Early Blue Model)
- Soldano SP-77 (Series II)
- Soldano X88R
- Splawn Nitro
- Splawn Quick Rod
- Sunn Model T
- Tube Works RT-2100
- Vox AC30 Top Boost (Silver Jubilee/S.S. Red)
- Vox AC30 Top Boost (Reissue)
- Weber 6M45p Amp Kit (with "Cascade mod" by me)
- Wizard Modern Classic I
- Yamaha T100
- Yerasov Soldier 30H

## Bass Amps
- Ampeg B-15N Late 1960's
- Ampeg B-15NC
- Ampeg B-15NF
- Marshall JMP Super Bass 100w 1992
- Marshall 200 1978 "Bass"
- Orange Terror Bass
- Secondary Bass (loosely based on the Sunn Beta series)
- Sovtek MIG-500 "Bassov Blues Boy"

# Troubleshooting
There are a few notable bugs that may cause Amplex to work or sound as intended. The ones mentioned below are the most prominent ones.

## Oversampling
There may be cases where some of the presets will not work correctly, it is largely in part of a bug within Amplex's oversampling feature.

A workaround for this is to set the oversampling to 8x* only (if you have touched the oversampling settings prior), and restart the plugin.
*In some cases, other presets may require higher or lower oversampling rates. Please experiment with them until any of the presets function properly.

## ASIO Drivers
***This has only been tested in REAPER so I am not sure if this problem is applicable to other DAWs.***
There are instances where some high gain presets sound too overcompressed to the point of being unusable. This issue seems to be exclusive to ASIO as the issue is not present with other audio devices. (Tested with WASAPI and DirectSound.) As of now, the only workaround for this is to switch to WASAPI as the DAW's main audio device.

# Special Thanks
- [StateOfMercury]( https://www.youtube.com/c/StateOfMercury ) and [【ブギウギ】]( https://soundcloud.com/funnyfaceman ) for indirectly inspiring me to write these presets in the first place.
- [@sdleffler]( https://github.com/sdleffler ) for providing me a schematic of the Orange Thunderverb.
- [@jorins]( https://github.com/jorins ) for recommending me to host these presets here.
- "Violet Delta Fuzz" is named after [Violet Delta]( https://www.youtube.com/c/VioletDelta2 ).
- Ceriatone for the [Dookie Mod layout]( http://www.ceriatone.com/british-style-plexi100-super-lead/#doc ).
- [Philipp Frank]( https://www.youtube.com/watch?v=eGBc4lC8zaY ) for kindly making his Plexi schematic publicly available.
- [Atomium Amplification]( https://atomiumamps.tumblr.com/post/116256981951/amt-ss-11b-mods-above-is-my-new-fly-in-show-setup ) for sharing their mod and schematics for the AMT SS-11B.
- [Paul P's Bogen amp conversion schematics]( https://ppamps.blogspot.com/2013_02_01_archive.html ) as a basis for comparison with the stock Bogen CHB-35A circuits.
