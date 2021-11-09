# the-assembler

Core coverage: [![codecov](https://codecov.io/gh/darkgap/the-assembler-core/branch/master/graph/badge.svg?token=BGLJ6X5SUZ)](https://codecov.io/gh/darkgap/the-assembler-core)

## Description
Just a little WIP game, where you have to program in ARM assembly to make thigs do things.


## Programming reference

[reference PDF for ARM sintax](https://iitd-plos.github.io/col718/ref/arm-instructionset.pdf#page=3) (will implement own sintax documentation)

[Other reference](https://www.macs.hw.ac.uk/~hwloidl/Courses/F28HS/Docu/DDI0406C_C_arm_architecture_reference_manual.pdf), more advanced but not taken as reference
 


## Features

### Commands List

The list of supported commands can be seen [here](docs/commands.md) 

### Updates

The Code editor window is coming together!
It also have spell checking in advance, and a little play scene for
preview is being made

![editor_panel](/docs/images/editor_panel_preview.png)

### Bonus

How to know that it's time to go to bed because of the max # of cycle terminate condition you did not put while testing <sub><sup>(~~hence not being able to stop the cycle)~~</sup></sub>


```assembly
vara: .word   2         
varb: .word   1         
text: .ascii  "8CHARTXT"  
       LDR R1, =vara    
       LDR R2, =varb    
       LDR R3, =text    
       LDR R4, [R2, #1] 
       LDR R5, [R1, #2] 
       LDR R6, [R2, #1]!
loop:                   
trap:  B trap           
       B loop
```








<!-- ![][OK]

![][WIP]

![][TODO]

![][NODO] -->

<!-- [OK]: https://image.flaticon.com/icons/png/32/3248/3248235.png -->
<!-- ICONS SIMPLE -->
<!-- [OK]: https://image.flaticon.com/icons/png/32/190/190411.png -->
<!-- [WIP]: https://image.flaticon.com/icons/png/32/190/190435.png -->
<!-- [WIP]: https://image.flaticon.com/icons/png/32/190/190420.png
[TODO]: https://image.flaticon.com/icons/png/32/190/190406.png
[NODO]: https://image.flaticon.com/icons/png/32/190/190438.png -->

<!-- rating and validation pack -->

<!-- [OK]: https://image.flaticon.com/icons/png/32/1721/1721945.png -->
[OK]: https://image.flaticon.com/icons/png/32/1722/1722017.png

[WIP]:  https://image.flaticon.com/icons/png/32/1721/1721923.png

[TODO]: https://image.flaticon.com/icons/png/32/3248/3248209.png

<!-- [NODO]: https://image.flaticon.com/icons/png/32/1721/1721955.png -->
[NODO]: https://image.flaticon.com/icons/png/32/1721/1721977.png

[NODO]: https://image.flaticon.com/icons/png/32/3558/3558838.png

<!-- 
![][OK]

![][WIP]

![][TODO]

![][NODO] -->




