# the-assembler

![Coverage Badge](CodeCoverage/Report/badge_combined.svg)

## Description
Just a little WIP game, where you have to program in ARM assembly to make thigs do things.



## Programming reference

 [reference PDF for ARM sintax](https://iitd-plos.github.io/col718/ref/arm-instructionset.pdf#page=3) (will implement own sintax documentation)


## Features

### Command Format

:heart: : not available yet\
:orange_heart: : WIP\
:green_heart: : available\
:black_heart: : not planned

| Text > BitC   | BitC > Func   |  Format                          |
| :-----:       | :------:      | :------:                         |
| :green_heart: | :heart:       | Data Processing                  |
| :heart:       | :heart:       | PSR Transfer                     |
| :heart:       | :heart:       | Multiply                         |
| :heart:       | :heart:       | Multiply Long                    |
| :heart:       | :heart:       | Single Data Swap                 |
| :green_heart: | :heart:       | Branch and Exchange              |
| :heart:       | :heart:       | HW Data transfer: reg offset     |
| :heart:       | :heart:       | HW Data transfer: imm offset     |
| :green_heart: | :orange_heart:| Single Data Transfer             |
| :heart:       | :heart:       | Block  Data Transfer             |
| :green_heart: | :green_heart: | Branch                           |
| :black_heart: | :black_heart: | Coprocessor Data Transfer        |
| :black_heart: | :black_heart: | Coprocessor Data Operation       |
| :black_heart: | :black_heart: | Coprocessor Register Transfer    |

### Branch Format

| Text > BitC   | BitC > Func   | Format    | Description           | 
| :-----:       | :------:      | :------:  | :----:                |
| :green_heart: | :heart:       |  BX       | Branch and Exchange   |

### Branch And Exchange

| Text > BitC   | BitC > Func   | Format    | Description           | 
| :-----:       | :------:      | :------:  | :----:                |
| :green_heart: | :green_heart: |  B        | Branch                |
| :green_heart: | :green_heart: |  BL       | Branch with Link      |

### Data Processing

| Text > BitC   | BitC > Func   | Mnemonic | Description | 
| :-----:       | :------:      | :------: | :---------: |
| :green_heart: | :heart:       |  AND     | operand1 AND operand2              |
| :green_heart: | :heart:       |  EOR     | operand1 EOR operand2              |
| :green_heart: | :heart:       |  SUB     | operand1 - operand2                |
| :green_heart: | :heart:       |  RSB     | operand2 - operand1                |
| :green_heart: | :heart:       |  ADD     | operand1 + operand2                |
| :green_heart: | :heart:       |  ADC     | operand1 + operand2 + carry        |
| :green_heart: | :heart:       |  SBC     | operand1 - operand2 + carry - 1    |
| :green_heart: | :heart:       |  RSC     | operand2 - operand1 + carry - 1    |
| :green_heart: | :heart:       |  TST     | as AND, but result is not written  |
| :green_heart: | :heart:       |  TEQ     | as EOR, but result is not written  |
| :green_heart: | :heart:       |  CMP     | as SUB, but result is not written  |
| :green_heart: | :heart:       |  CMN     | as ADD, but result is not written  |
| :green_heart: | :heart:       |  ORR     | operand1 OR operand2               |
| :green_heart: | :heart:       |  MOV     | operand2(operand1 is ignored)      |
| :green_heart: | :heart:       |  BIC     | operand1 AND NOT operand2(Bit clear)
| :green_heart: | :black_heart: |  MVN     | NOT operand2(operand1 is ignored)  |


### Single Data Transfer

| Text > BitC   | BitC > Func   | Format    | Description                           | 
| :-----:       | :------:      | :------:  | :----                                 |
| :green_heart: | :green_heart: |  LDR      | Load data to register (pre-index)     |
| :green_heart: | :green_heart: |           | Load data to register (post-index)    |
| :green_heart: | :green_heart: |  ADR      | Load address to register (post-index) |
| :green_heart: | :orange_heart:|  STR      | Store register                        |


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




