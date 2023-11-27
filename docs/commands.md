# Commands available

:heart: : not available yet\
:orange_heart: : WIP\
:green_heart: : available\
:black_heart: : not planned

## Formats

### Command Format

|  Text > BitC  |  BitC > Func  |            Format             |
| :-----------: | :-----------: | :---------------------------: |
| :green_heart: | :green_heart: |        Data Processing        |
|    :heart:    |    :heart:    |         PSR Transfer          |
|    :heart:    |    :heart:    |           Multiply            |
|    :heart:    |    :heart:    |         Multiply Long         |
|    :heart:    |    :heart:    |       Single Data Swap        |
| :green_heart: | :green_heart: |      Branch and Exchange      |
|    :heart:    |    :heart:    | HW Data transfer: reg offset  |
|    :heart:    |    :heart:    | HW Data transfer: imm offset  |
| :green_heart: | :green_heart: |     Single Data Transfer      |
|    :heart:    |    :heart:    |     Block  Data Transfer      |
| :green_heart: | :green_heart: |            Branch             |
| :black_heart: | :black_heart: |   Coprocessor Data Transfer   |
| :black_heart: | :black_heart: |  Coprocessor Data Operation   |
| :black_heart: | :black_heart: | Coprocessor Register Transfer |

### Branch Format

|  Text > BitC  |  BitC > Func  | Format |     Description     |
| :-----------: | :-----------: | :----: | :-----------------: |
| :green_heart: | :green_heart: |   BX   | Branch and Exchange |

### Branch And Exchange

|  Text > BitC  |  BitC > Func  | Format |   Description    |
| :-----------: | :-----------: | :----: | :--------------: |
| :green_heart: | :green_heart: |   B    |      Branch      |
| :green_heart: | :green_heart: |   BL   | Branch with Link |

### Data Processing

|  Text > BitC  |  BitC > Func  | Mnemonic |             Description              |
| :-----------: | :-----------: | :------: | :----------------------------------: |
| :green_heart: | :green_heart: |   AND    |        operand1 AND operand2         |
| :green_heart: | :green_heart: |   EOR    |        operand1 EOR operand2         |
| :green_heart: | :green_heart: |   SUB    |         operand1 - operand2          |
| :green_heart: | :green_heart: |   RSB    |         operand2 - operand1          |
| :green_heart: | :green_heart: |   ADD    |         operand1 + operand2          |
| :green_heart: | :green_heart: |   ADC    |     operand1 + operand2 + carry      |
| :green_heart: | :green_heart: |   SBC    |   operand1 - operand2 + carry - 1    |
| :green_heart: | :green_heart: |   RSC    |   operand2 - operand1 + carry - 1    |
| :green_heart: | :green_heart: |   TST    |  as AND, but result is not written   |
| :green_heart: | :green_heart: |   TEQ    |  as EOR, but result is not written   |
| :green_heart: | :green_heart: |   CMP    |  as SUB, but result is not written   |
| :green_heart: | :green_heart: |   CMN    |  as ADD, but result is not written   |
| :green_heart: | :green_heart: |   ORR    |         operand1 OR operand2         |
| :green_heart: | :green_heart: |   MOV    |    operand2(operand1 is ignored)     |
| :green_heart: | :green_heart: |   BIC    | operand1 AND NOT operand2(Bit clear) |
| :green_heart: | :green_heart: |   MVN    |  NOT operand2(operand1 is ignored)   |

### Single Data Transfer

|  Text > BitC  |  BitC > Func  | Format | Description              |
| :-----------: | :-----------: | :----: | :----------------------- |
| :green_heart: | :green_heart: |  LDR   | Load data to register    |
| :green_heart: | :green_heart: |  ADR   | Load address to register |
| :green_heart: | :green_heart: |  STR   | Store register           |
