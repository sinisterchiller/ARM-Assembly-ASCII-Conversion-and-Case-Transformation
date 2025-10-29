{\rtf1\ansi\ansicpg1252\cocoartf2865
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 # ARM Assembly \'96 ASCII Conversion and Case Transformation\
\
## \uc0\u55357 \u56589  Overview\
This project explores **ARM assembly programming** using the **THUMB2 instruction set** on an STM32 NUCLEO-L432KC board.  \
It implements two programs: one to convert ASCII characters to their **hexadecimal values**, and another to **switch between uppercase and lowercase** letters.\
\
## \uc0\u55356 \u57263  Objectives\
- Practice low-level ARM assembly with THUMB2 instructions  \
- Implement ASCII-to-hexadecimal conversion with error handling  \
- Perform case conversion between uppercase and lowercase  \
- Manage memory addressing and program flow control on embedded hardware  \
\
## \uc0\u9881 \u65039  Tools & Hardware\
- **Board:** STM32 NUCLEO-L432KC  \
- **IDE:** STM32CubeIDE 2024  \
- **Instruction Set:** ARM THUMB2  \
- **Programming Language:** ARM Assembly  \
\
## \uc0\u55358 \u56809  Implementation\
### Part A \'96 ASCII to Hexadecimal\
- Reads ASCII characters from memory  \
- Converts valid characters (`0\'969`, `A\'96F`, `a\'96f`) to hexadecimal  \
- Stores results at a new memory address  \
- Invalid characters return `\'961`  \
\
### Part B \'96 Case Conversion\
- Reads ASCII letters (`A\'96Z`, `a\'96z`)  \
- Converts uppercase \uc0\u8596  lowercase by adding or subtracting 32  \
- Invalid characters are replaced with `*`  \
- Program halts when **Enter (0x0D)** is detected  \
\
## \uc0\u55358 \u56810  Testing and Validation\
- Input data arrays are stored in memory starting at `0x20001000`  \
- Outputs for Part A and B are stored at `0x20002000` and `0x20003000` respectively  \
- Verified using multiple test sets containing valid and invalid inputs  \
- Results confirmed correct conversions and error handling  \
\
## \uc0\u55357 \u56492  Discussion\
This experiment illustrates direct manipulation of data in memory and conditional branching in assembly.  \
It reinforces understanding of ASCII encoding, address management, and flow-control mechanisms essential for embedded-systems programming.\
\
## \uc0\u55357 \u56516  License\
This work is licensed under the **Creative Commons Attribution\'96NonCommercial\'96ShareAlike 4.0 International (CC BY-NC-SA 4.0)**.  \
You may share and adapt this project for non-commercial use with proper credit.  \
See the [LICENSE](./LICENSE) file for details.\
}