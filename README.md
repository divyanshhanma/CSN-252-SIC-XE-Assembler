**Steps for running**
1. Write the input SIC/XE code in input.txt file
2. Run the main.cpp file
3. The ouput object file will be produced in objectfile

 INPUT AND OUTPUT:  
o Sample input code:  
SUM     START  0  
FIRST   LDX    #0  
        LDA    #0  
        +LDB   #0  
        +LDB   #TABLE2  
        LDT     =X'05'  
        BASE   TABLE2  
LOOP    ADD    TABLE,X  
        ADD    TABLE2,X  
        TIX    COUNT  
        JLT    LOOP  
        +STA   TOTAL  
        RSUB  
COUNT   RESW   1  
TABLE   RESW   2000  
TABLE2  RESW   2000  
TOTAL   RESW   1  
        END    FIRST  
  
o Input output object code:  
H^SUM   ^000000^002F03  
T^000000^1D^050000010000691017901BA0131BC0002F200A3B2FF40F102F004F0000  
M^000007^05  
M^000017^05  
E^000000  
