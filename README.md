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
| :green_heart: | :heart:       | Branch                           |
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
| :green_heart: | :heart:       |  B        | Branch                |
| :green_heart: | :heart:       |  BL       | Branch with Link      |

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
















