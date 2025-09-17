Created: Sep 16 2025
Class: [[Bootcamp]] 
- - -
# Loading
## Load value
```
LD r0, X

HALT

X .FILL #32
```
## Load at address
```
LD r0, MEM
LD r1, X
STR r1, r0, #0
HALT

MEM .FILL x3100
X .FILL #35
```

# [[Two's complement|Negation]]
```
NOT r0, r0
ADD r0, r0, #1
```
# Loops
```
ADD r0, r0, #10
loop
ADD r0, r0, #-1
BRp loop
```
# Functions
```
JSR FUNC ; stores mem addr in r7
OUT

HALT 

FUNC
ADD r0, r0, x31
RET ; JUMPS to pos stored in r7
```