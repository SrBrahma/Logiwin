```
+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+
Logiwin Open Project
Version 1.1.0  - xx/05/2016

Starting date of this documentation: 28/02/15 (Like a year before publishing it!)

-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
                                   # Index #
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
|
| Also try Ctrl+f

    1. Introduction
    2. Basic Explanations
    3. Patch notes
    4. Future updates list
    5. Downloads links
    6. Advanced Explanations
    7. Console Special Codes
    8. Clock Script
    9. Instruction Set Descriptions
    A. Instruction Set List
    B. Credits, special thanks and contact
|
|
|
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
1.                               Introduction
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
|
| Hi!

    Hello, fellow reader! This is a hobby of mine, that I have been working for some years; maybe 3, maybe 4 (EDIT 1.1.0: Now maybe 6)
    This circuit is my interpretation of a computer, but it doesn't follow strictly any existing system.
|
|
|
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
2.                            Basic Explanations
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
|
| A better introduction!

    4.1)  My main idea in this project is to be an easily modified circuit by any one (with some knowledge), and you should do it. I really want a community
 for it, and this includes Programmers, Artists, JAR libraries modders (AltruismAndCake, the first one!) and Eletronics.
    4.2)  I didn't intended to make the project look like a real CPU, computer, etc. This is my interpretation of what it should be to work 
 in a single-clock and to have the fastest simulation speed as possible. When I started it, I didn't have specific knowledges about programmation, engineering, etc.
 Some stuff can work similiarly to real life. If you have better ideas for names of anything, tell me so I can correct it and make more 
 common user-friendly. Most instructions I made intended to look like Assembly but there's are some differences.
    4.3)  Most sub-circuits have explanations inside them. They might help you.
    4.4)  Remember the propagation delays in the circuits. Some stuff are ugly to workaround it.
    4.5)  Contact me by e-mail or in the Reddit. The information about contact is on the end of this documentation. If you share, modify 
 or just really liked this project, tell me! I will be happy to know that this hobby got its fans :)
    4.6)  The connections in this circuit can look strange, but most were intentional. Looks like the fewer wire nodes, the faster the simulation frequency will be.
    4.7)  Many informations you may need are in this documentation. However, some of the functionalities and explanations may be missing. Contact me 
 for further help..
    4.8)  Also, there can be some misleading informations in this document, as I change stuff on the project all the time and I forget to update they info here.     
 If anything is unclear or wrong, contact me to fix it.
    4.9)  Looking for basic help? So you should google: Hexadecimal, Logic gates, Machine Code, CPU architetures,
 Instruction sets, Assembly, etc.
    4.A)
|
|
|
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
3.                                Patch notes
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
|
| So, what's the news?

    v1.1.0 - xx/06/18 Yeah, this update took some really big time. Everytime I find a big problem here I just
get real bored just by opening Logisim and then I close it.


    New: LASM: Logiwin Assembly. A whole notepad++ Python Script code to compile Assembly-like codes.  
        Bin to BCD decoder intruction.
        Find lowest/highest low/high bit instruction (FLL, FHL, FLH, FHH)
        Compare instruction changed, it will now output Signed/Unsigned relations.
        So, new conditional Jumps added: Jump if Above and Jump if Below (and the Equal variations), for unsigned comparations.
        LIFO added, with Push, Pop, Call and Return instructions.
        Random instruction.
        Keyboard added.
        Added and changed a lot of stuff in this Readme.
        Store Current Address (SCA) instruction.
        Increase and Decrease (INC & DEC) instructions.  
        Joystick added.
        Renamed MOV to ACC, as MOV was very ambiguos.
        It now have 2 clocks instead of one (read 7.3).
        The main RAM controller is now inside the CPU, got some performance buff.
        Removed all the delayers from the Console, as I added a new Clock.
        Changed some intructions code.
        General perfomance boosts. Unfortunatelly, with all the new stuff, the performance has decayed.
        General changes.
        

    Fixes: Fixed CMP clearing Acc. 
        Fixed conditional jumps.
        Some general stuff.

    v1.0.5 - 03/03/16 Added SWP and ERS instructions. JMP instructions can now jump to values stored in Address. Changed text 7-bit to 8-bit
(easier to deal with). Some general changes. Changed some stuff in this documentation. Added a Mario in a screen for fun (and for some research).
Great times are coming!

    v1.0.1 - 25/02/16 Fixed a small problem, NOT and NEG weren't connected on ALU.    

    v1.0.0 - 25/02/16 Almost an year since the beggining of this documentation on notepad++ (but now you should open it on normal notepad for the
formatation). Time flies! The first public Logiwin version, still very alpha, but I wanted to share the most soon as possible! Most don't work yet,
but it is possible to have some fun just with the memory and console on the main circuit.
|
|
|
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
4.                            Future updates list
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
|
| Hey, hey! What's coming next?

    Mouse-Pad mod compatibility (when it exists!) - Ever wanted to touch you screen?
    Sound (Waiting for a mod!)
    Floating Point System
    Programs, as Notepad, programs editor, Paint brush style program, etc etc. Already writing some.
    An Operating System. Maybe I will call it Logiwin OS. Looks badass.
|
|
|
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
5.                              Downloads links
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
|
| Here's what you need to have it running. Be sure to do "5.2)" item. 

    5.1)  Logisim, the simulation program (I recommend the cornell unnoficial version). I don't like Logisim Evolution, it changes a lot of
 components, making them huge for 32 bits wide, complex and weird. Maybe on future I will port to it, however, as it is updated frequently.
 
        Unnoficial recomended version:
            NOTE: On my PC, to make the mods work with this unnoficial version, I had to first run the official Logisim and load them. 
            Otherwise the mods wouldn't load properly.
            http://www.cs.cornell.edu/courses/cs3410/2015sp/logisim-2.7.2-cs3410-20140215.jar
       
        Official Logisim:
            NOTE: I still recommend the unnoficial version above. With the official, you may not be able to select properly select devices
                like the keyboard, which have a part around it.
            https://sourceforge.net/projects/circuit/

    5.2)  The mods. You MUST download this, instructions on how to install on the page, but I assure you it's pretty easy! :) 
        https://www.reddit.com/r/logisim/comments/46lrow/modding_new_mods_folder/
|
|
|
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
6.                           Technical Informations
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
| So you want to LEARN?
    6.1)  "X" in this documentation can be even 0 or 1, sometimes changing it functionallity.
    6.2)  NEVER EVER write anything in Address 0x000000, it WILL get buggy. Some instructions propagations delays will use it.
        Just avoid this bad Address and everything is gonna be alright!  
    6.3)  0xxx xxx1:
        First bit = 1 (The last form left to right, the 1st bit)
        Last bit = 0  (The first from left to right, the 8th bit)
    6.4)  You can directly only use 24-bit data (like ADD #0xffffff), but it is possible to do stuff like this:
      Have the value already written on memory, and access it when you want
                      Or if you don't have it written
                ACC #0xffffff (load on Accumulator the last 24 bits.)
                SHL #0x000008 (shift left acc for 8 units)
                ADD #0x0000aa (add the first 8 bits)
      Now you will have a full 32-bit data on the Accumulator, and can do this
                STO #0xXXXXXX (store this value at any place you want)
      And finally, when you want
                ADD 0xXXXXXX  (will use the value you stored, that will stands for 0xffffffaa (32-bit sized))
    6.5)  "ALU Flag" is like a Carry Flag, but indicates if there is carry out from sum or multiplication, burrow out from substract and remain from divide.
    6.6)  "Out2" from ALU outputs the remain from divide or carry out from multiplication. I will give it an instruction later.
    6.7)  Address = 24bits
        0000 0000 0000 0000 0000 0000
        23-24bits for determinating the storage device (leftist ones)
         = 00 is for the non-volatile memory, a SSD-like memory.
         = 01 is for the volatile memory, a RAM-like memory.
         = The other values are for now unused, maybe in the future new storage devices will be added.
    6.8)  Deppending on your real hardware, you will get a faster or slower simulation frequency (so will be the Instructions per Second).
|
|
|
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
7.                          Console Special Codes
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
|
| Specials ASCII codes for the Console, the screen which outputs text.  

    7.1)  Copied from the Library Reference from Logisim: 
        "The only supported control sequences are: backspace (ASCII 8), which deletes the last character in the final row, unless the final row is already empty; 
        newline (ASCII 10), which moves the cursor to the beginning of the following line, scrolling if necessary;
        and form-feed (ASCII 12, typed as control-L), which clears the screen."

-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
8.                             Clock Script
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
|
| What happens in each part of the CPU clock cycle. Remember this concept: 
          ____      ____ _ _  1 (High)
     ____/    \____/    \____ 0 (Low) 
    (  8.1   8.2   8.1   8.2)

    8.1)  Rising Edge
        a) Program Counter Increases (or jump if instructed to).
        b) If instructed, data is be stored in the Memory, or in the Accumulator or in the LIFO.
        c) The instruction register is cleared (to avoid propagation issues).
        
    8.2) Falling Edge
        a) Instruction is loaded.
        b) Some instructions are executed.
        
    8.3)  Since v1.1.0, circuit have 2 clocks, the CPU clock and the new one.
        CPU Clock -> Now by default have a Low Duration of 3 (you can change to 5,7,9...), but still have a High Duration of 1. (Read 1/3 timing)
        It don't make the circuit work slower (for having a higher delay between clocks), as when you increase the delay, the simulation frequency increases.
        Ex: Before, when the CPU clock was 1/1, when the Logiwin CPU was 100% on load, the Logisim simulation was ~1KHz (~500 Instructions per Second).
        Now with 1/3 for example, in heavy usage (same circunstances), frequency displayed is on ~2KHz (still ~500 ips)
        For the curious ones, on 1/5 Clock, the frequency was ~3KHz (Still ~500ips!).
        As you see, this change (made to fix some issues) won't slow down the Logiwin CPU. 
        New one -> The another Clock is a 1/1 timing clock, for general porpouses (like console).
|
|
|
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
9.                        Instruction Set Explained                     
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
|
| Don't know how a instruction works, or what it do? Here you can learn about it.

 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
    9.1)    General
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
 
    a) ACC = Accumulator
        Move a value into Accumulator. If the 32nd bit is active, will take the value from the given Address, else, will store a direct value.
        But if the 32nd bit is active, and no Address is given, it will use the value from the Address, like a pointer.
        Ex1: Store the value 0x000010 into the Accumulator
            ACC #0x000010
        Ex2: Store the value of the Address 0x123321 into the Accumulator
            ACC 0x123321
        Ex3: Store the content of the Address given by the Accumulator into the Accumulator
            Accumulator holds 0x00001234
            Address 0x001234 holds 0xffffaaaa
            ACC 0x000000
            Now Accumulator holds 0xffffaaaa

    b) STO = Store
        Store the current value of the Accumulator on the given Address. The 32nd bit doesn't change the functionality.
        Ex1: Store the value into the Address 0x809010
            STO #0x809010 (or 0x809010)

    c) ERS = Erase
        Clears the selected Address (with zeroes). The same as "ACC #0x000000; STO Y", without messing the current value of Accumulator.
        The 32nd bit doesn't change the functionality.
        Ex1: Erase the Address 0x300020
            ERS #0x300020 (or 0x300020)

    d) SWP = Swap the values of Accumulator with the chosen Address. The 32nd bit doesn't change the functionality.
        Ex1: Accumulator holds value "100"
        The Address 0x000030 holds value "359"
        >SWP #0x000030  Now the Accumulator will hold the value "359", and the Address will hold the value "100".

    e) TXT = Outputs text in console            [CONS <= Y]
        Uses the simple 7-bit ASCII code (google it, uses the same scheme), but you can group them, and send up to four digits by time.
            (But to fit better on the 32bit system, the 7-bit ASCII is extended to 8-bit, with the last bit unused.)
        The writing on the console is made from left to right.
        You can use 64-bit to send the maximum of 4 characters by clock, using Address: 
            0x01 | TXT 0x00000f      = (0x9300000f) = 1001 0011 0000 0000 0000 0000 0000 1111
            ...
            0x0f | 0x4c6f6769                   = '0100 1100' '0110 1111' '0110 0111' '0110 1001' (the ' ' are separating the characters")
                                                          (L)         (o)         (g)         (i)
             Will output "Logi" to the console, as you can see in the circuit.
        Or you could just use just 32-bit of memory to send the maximum of 3 character per clock
                0x01 | TXT #0x4c6f67     = (0x134c6f67)  Will output "Log" to the console

        

    f) KEY = Stores the current character entered on keyboard   [ACC/MEM <= External Input #1]
        If no data is given with the instruction (=0x18000000), the ASCII will be saved on the Accumulator, else, 
        the ASCII will be saved on this Address. The 32nd bit doesn't change the functionality.
        Ex1: Stores the current key on the Accumulator
            KEY #0x000000 (or 0x000000)
        Ex2: Stores the current key on the Address 0x123456
            KEY #0x123456 (or 0x123456)

    g) SCA = Store Current Address on the memory or in the address
        Ex:   This command is being readed on the memory Address 0x000030 (=0x30).
        Ex1: 0x30 | SCA #0x000000                     The Accumulator will now hold the value 0x30.
        Ex2: 0x30 | SCA  0x000070 (Or SCA 0x000070)   The Address 0x000070 will now hold the value 0x30.

    h) SRA = Set Relative Address
        This one is a little complex, but just think of instead using the 0x000000 Address as an start point,
        we changed it, so you can place a code anywhere in the memory and it would work without changing anything
        (just the SRA value, but you can create a small function to do it automatically. Tip: Use SCA).
        Ex1: Here we won't use the SRA command. Imagine we just executed the instruction in 0x30.
               0x40 | 0xDEADBEEF   This address just hold this value.
               0x45 | 0xCAFEF00D   This address just hold this value.
               
               0x30 | ACC 0x000040 This will normally load the "0xDEADBEEF" into the Accumulator.
               
        Ex2: Here we will use the SRA command. Imagine we executed the instructions 0x30 and 0x31.
               0x40 | 0xDEADBEEF    This address just hold this value.
               0x45 | 0xCAFEF00D    This address just hold this value.
               
               0x30 | SRA #0x000005 This will make the address 0x000005 as an starting point.
               0x31 | ACC 0x000040  This is the same command from the Ex1, but it will load the "0xCAFEF00D" into the Accumulator,
                                        as you changed the starting point.
        As you can see, if you use the SRA command, all the Addresses you consult/change will be added from the SRA value.
        You can at anytime revert it to the normal by executing "SCA #0x000000").
        You can also use values stored on Memory. Imagine we started on address 0x09.
          Ex3: 0x07 | 0x00000003    This address just hold this value.
               0x09 | SRA 0x000007  As you see, no "#". So it will use an value stored in Memory. In the end, the Relative Address will now be 0x3.
   
    i) RND = Random
        This will generate a random 32 bits value, based on basic Logisim random number generator. If no data is given, the random number
        will be stored on Accumulator, else, it will be stored on the memory. The 32nd bit doesn't change the functionality.
        Ex1: Generate a random value to the Accumulator
            RND #0x000000 (or 0x000000)
        Ex2: Generate a random value to the Address 0x37
            RND #0x000047 (or 0x000047)
    
    j) PSH = Push
        This will store a 32 bits value into the LIFO (Last In First Out) memory. If the 32nd bit is active, it will store the value
        stored in the given address, else, will store the direct value.
        Ex1: Push the value 1000h
            PSH #0x001000
        Ex2: Push the value stored on the Address 0x000011
            PSH 0x000011

    k) POP = Pop
        This will take out the last value stored on the LIFO (as the name says), and will store it on the Accumulator if no data is given, else
        will store on the given Address. The 32nd bit doesn't change the functionality.
        Ex1: Pop into the Accumulator
            POP #0x000000
        Ex2: Pop into the Address 0x947203
            POP #0x947203 (or 0x947203)        
|
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
    9.2)    Jumps
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
|
| COMPFLAG = Comparative Flag
        
    a) CMP = Compare Accumulator and value                    [COMPFLAG = <, =, > = 1, 2, 4]
        Attention: the focus is the value at Acc, ex:
        ACC #0x000008 -> Acc value is now 8.
        CMP #0x000002 -> Compare with the number 2.
        This will result in ">", COMPFLAG 4. Number 8 is bigger than number 2. Be careful.

    b) JMP = Jump to Address                                   [ADDRESS <= Y]
        Ex1: JMP #0x000050 -> will jump to the address 0x000050
        Ex2: JMP 0x000060 -> will read value from the address 0x000060 and jump to that value. In this case, will jump to 0x0000ff.
            0x000060 = #0x0000ff

    c) JZ  = Jump to adress if Accumulator is 0                [ADDRESS = Y if ACC == 0]
    d) JNZ = Jump to adress if Accumulator is not 0            [ADDRESS = Y if ACC !== 0]
    e) JC  = Jump to adress if ALU Flag is 1                   [ADDRESS <= Y if ALUFLAG == 1]
    f) JNC = Jump to adress if ALU Flag is 0                   [ADDRESS <= Y if ALUFLAG == 0]
    
    g) JA  = Jump if Above             (Unsigned)
    h) JAE = Jump if Above or Equal    (Unsigned)
    i) JG  = Jump if Greater           (Signed)
    j) JGE = Jump if Greater/Equal     (Signed)
    k) JE  = Jump if Equal             (Both)
    l) JNE = Jump if Not Equal         (Both)
    m) JB  = Jump if Below             (Unsigned)
    n) JBE = Jump if Below/Equal       (Unsigned)
    o) JL  = Jump if Less              (Signed)
    p) JLE = Jump if Less or Equal     (Signed)
    
    q) CAL = Store (Push) the actual Address +1 into the LIFO memory, and Jump to the given Address.
    
    r) RET = Return
        Pops the last LIFO data, and use it as an Address to Jump to.
|
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
   9.3  Mathematics (X=ACC, Y=Value)
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
|
| The Value can be a direct value or indirect one.
|    Ex: ADD #0x000008  -> Will add the value 8 to the Accumulator.
|    Ex: ADD  0x0000FF  -> Will add the value stored on the address 0x0000FF.
        
    a) ADD = Add
        Move to the Accumulator the result of Accumulator + value
        
    SUB = Substract
        Move to the Accumulator the result of Accumulator - value
        
    MUL = Multiply
        Move to the Accumulator the result of Accumulator * value
        If there is a carry out, it will be stored on a auxiliar register inside the ALU, and it can be moved to the Accumulator with the AL2 instruction.
        
    DIV = Divide
        Move to the Accumulator the integer result of Accumulator / value
        If there is a remain, it will be stored on a auxiliar register inside the ALU, and it can be moved to the Accumulator with the AL2 instruction.
        
    INC = Increase by 1 the data hold on the selected Address. If the argument is 000000, will Increase the Accumulator value instead.
          The 32nd bit doesn't change this instruction functionallity.
        Ex1: ACC #0x000005      Move the value "5" to the Accumulator.
             STO #0x000080      Will store the value on the Accumulator ("5") on the Address 0x000080.
             INC #0x000080      The address will now hold the value "6" (5+1)
             INC #0x000080      The address will now hold the value "7" (6+1)
             
        Ex2: ACC #0x000003      Move the value "5" to the Accumulator.
             INC #0x000000      Now the Accumulator holds the value "4".

    DEC = Decrease by 1 the data hold on the selected Address. If the argument is 000000, will Decrease the Accumulator value instead.
          The 32nd bit doesn't change this instruction functionallity.
        Ex1: ACC #0x000005    Move the value "5" to the Accumulator.
             STO #0x000080    Will store the value on the Accumulator ("5") on the Address 0x000080.
             DEC #0x000080    The address will now hold the value "4" (5-1)
             DEC #0x000080    The address will now hold the value "3" (4-1)
             
        Ex2: ACC #0x000003      Move the value "5" to the Accumulator.
             DEC #0x000000      Now the Accumulator holds the value "2".
    
    NEG = Negate Accumulator                  [X <= -X]
        Invert the signal of the content of the Accumulator.
        Note that this instruction doesn't use any additional information. Just do "NEG #0x000000".
        The 32nd bit doesn't change this instruction functionallity.
        
    CMP = Compare
    
    AL2 = ALU output 2
        Move to the Accumulator the previous auxiliar output of Multiplication (carry out) or Division (remain).
        The 32nd bit doesn't change this instruction functionallity.
        
    FLL = Find Lowest Low
        Move to the Accumulator the position of the lowest bit of value 0 of the Accumulator value. If no low bit is found, 0 will be stored into the Accumulator.
        Ex: ACC #0x0000FC   (ACC = 0000 0000 0000 0000 0000 0000 1111 1100)
            FLL
            > Accumulator will now have the value 0x1
            
    FHL = Find Highest Low
        Move to the Accumulator the position of the highest bit of value 0 of the Accumulator value. If no low bit is found, 0 will be stored into the Accumulator.
        Ex: ACC #0x0000FC   (ACC = 0000 0000 0000 0000 0000 0000 1111 1100)
            FHL
            > Accumulator will now have the value 0x20 (32 in decimal)
            
    FLH = Find Lowest High
        Move to the Accumulator the position of the lowest bit of value 1 of the Accumulator value. If no high bit is found, 0 will be stored into the Accumulator.
        Ex: ACC #0x0000FC   (ACC = 0000 0000 0000 0000 0000 0000 1111 1100)
            FLH
            > Accumulator will now have the value 0x3
     
    FHH = Find Highest High
        Move to the Accumulator the position of the highest bit of value 1 of the Accumulator value. If no high bit is found, 0 will be stored into the Accumulator.
        Ex: ACC #0x0000FC   (ACC = 0000 0000 0000 0000 0000 0000 1111 1100)
            FHH
            > Accumulator will now have the value 0x8
|         
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
   9.4  Logical
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
| 
|  These ones are self explaining, logical operations.
|  If LSB 31 is 1, will use an Address content as argument, else, will use the direct value as argument.
  
    AND = Logical AND.
    OR  = Logical OR.
    XOR = Logical Exclusive OR.
    NND = NAND, Logical NOT AND. Took a letter out to have just 3 letters.
    NOR = Logical NOT OR.
    XNR = XNOR, Logical Exclusive NOT OR. Took a letter out to have just 3 letters.
    NOT = Logical NOT. Only affects the Accumulator. The 32nd bit doesn't change it's functionallity. Doesn't use any argument.
        Ex: ACC #0x0000AA (ACC = 0000 0000 0000 0000 0000 0000 1010 1010)
            NOT           Accumulator will now hold 0xFFFF55 ( = 1111 1111 1111 1111 1111 1111 0101 0101)
|
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-   
   9.5  Shift / Rotate 
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
|
|    Moves the bits of the value in the Accumulator.
|    6th bit to 24th bit aren't used, only the least 5 significant bits, for the distance (maximum of 32)
    
    SHL = Shift Accumulator value left
        Ex: ACC #0xF000F0 (ACC = 0000 0000 1111 0000 0000 0000 1111 0000)
            SHL #0x000008 (ACC = 1111 0000 0000 0000 1111 0000 0000 0000)
            SHL #0x000002 (ACC = 1100 0000 0000 0011 1100 0000 0000 0000)
            
    SHR = Shift Accumulator value right
    
    ROL = Rotate Accumulator value left
        Ex: ACC #0xF000F0 (ACC = 0000 0000 1111 0000 0000 0000 1111 0000)
            SHL #0x000008 (ACC = 1111 0000 0000 0000 1111 0000 0000 0000)
            SHL #0x000002 (ACC = 1100 0000 0000 0011 1100 0000 0000 0011)
            
    ROR = Rotate Accumulator value right
|
|
|
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
A.                          Instruction Set List
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
|
| A quick reference guide. Compact, simple, fast. Everything you need is in here.
|
|   The instructions are ordered by crescent order (the same way visible on Instructions sub-circuit).
|   If any of these doesn't work properly, contact me to fix it.
|   The X in the Binary means "Don't-Care" (https://en.wikipedia.org/wiki/Don%27t-care_term), it will not change
|       the instruction functionality. However, to don't make confusions, in the list below it wont be listed the hexadecimal code
|       for the indirect mode (X = 1). Do prefer the X = 0 alternative, as the X = 1 may be added in the future.
|   The D in the Binary will usually stands for direct and indirect modes, in the Hexadecimal column, the "#" is Y = 0, and the 
|       "A" is Y = 1. To know the differences between them, read the specific instruction information in the previous section.
|
|   The "#" usually stands for the direct mode.
|       Ex: ACC #0xBABACA, will store this value on the Accumulator.
|
|   The "A" (Address) usually stands for the indirect mode, will use the value stored in the given Address.
|       Ex: ADD 0x000fff, will add the value stored in this address.
|          
|   The "S" stands for "Store at given Address".
|       If followed by "!", you can if you use 0x0 as argument to these instructions, it will involve the Accumulator
|       (usually storing something at the Accumulator). Read the instruction description.
|   The "-" stands for "Don't care" (https://en.wikipedia.org/wiki/Don%27t-care_term); doesn't matter.
|       This instruction doesn't have arguments. '-' instead of 'X' to facilitate the reading.
|       To make a default, The LSB 31 = 0 is encouraged (and always used in LASM compiler).


[Binary ][Name]  [    Hexadecimal     ]    [Quick description]
                 [Argument prefix LASM]
                     [#]      [None]   
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
   A.1  GENERAL    
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
                   
-000 0000 NOP  <>  0x00 (-) - 0x80 (-)    - No Operation. Nothing will happen.
D000 0001 ACC  <>  0x01 (#) - 0x81 (A)    - Move to Accumulator
1000 0010 STO  <>  -------  - 0x82 (S)    - Store
1000 0011 ERS  <>  -------  - 0x83 (S)    - Erase
1000 0100 SWP  <>  -------  - 0x84 (S)    - Swap


 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
   A.2  JUMPS
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-

D000 0111 CAL  <>  0x07 (#) - 0x87 (A!)   - Call

D000 1000 JMP  <>  0x08 (#) - 0x88 (A!)   - Jump
D000 1001 JZ   <>  0x09 (#) - 0x89 (A!)   - Jump if Zero
D000 1010 JNZ  <>  0x0A (#) - 0x8A (A!)   - Jump if Not Zero
D000 1011 JC   <>  0x0B (#) - 0x8B (A!)   - Jump if Carry flag
D000 1100 JNC  <>  0x0C (#) - 0x8C (A!)   - Jump if Not Carry flag
D000 1101 JA   <>  0x0D (#) - 0x8D (A!)   - Jump if Above            (Unsigned)
D000 1110 JAE  <>  0x0E (#) - 0x8E (A!)   - Jump if Above or Equal   (Unsigned)
D000 1111 JG   <>  0x0F (#) - 0x8F (A!)   - Jump if Greater          (Signed)
D001 0000 JGE  <>  0x10 (#) - 0x90 (A!)   - Jump if Greater or Equal (Signed)
D001 0001 JE   <>  0x11 (#) - 0x91 (A!)   - Jump if Equal
D001 0010 JNE  <>  0x12 (#) - 0x92 (A!)   - Jump if Not Equal
D001 0011 JB   <>  0x13 (#) - 0x93 (A!)   - Jump if Below            (Unsigned)
D001 0100 JBE  <>  0x14 (#) - 0x94 (A!)   - Jump if Below or Equal   (Unsigned)
D001 0101 JL   <>  0x15 (#) - 0x95 (A!)   - Jump if Less             (Signed)
D001 0110 JLE  <>  0x16 (#) - 0x96 (A!)   - Jump if Less or Equal    (Signed)
D001 0111 RESERVED 0x17 (#) - 0x97 (A)
D001 1000 RESERVED 0x18 (#) - 0x98 (A)
D001 1001 RESERVED 0x19 (#) - 0x99 (A)
D001 1010 RESERVED 0x1A (#) - 0x9A (A)

-001 1011 RET  <>  -------  - 0x9B (-)    - Return to Call command origin

 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
   A.3  GENERAL2
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-

1001 1100 INC  <>  -------  - 0x9C (S!)   - Increase (+=1) the data on Address (poderia os dois)
1001 1101 DEC  <>  -------  - 0x9D (S!)   - Decrease (-=1) the data on Address

1001 1110 SCA  <>  -------  - 0x1E (S!)   - Store Current Address
D001 1111 SRA  <>  0x1F (#) - 0x9F (A)    - Set Relative Address
1010 0000 RND  <>  -------  - 0x40 (S!)   - Random
D010 0001 PSH  <>  0x41 (#) - 0xC1 (A!)   - Push
1010 0010 POP  <>  -------  - 0x42 (S!)   - Pop

D001 1110 TXT  <>  0x43 (#) - 0xC3 (A!)   - Outputs text to console (External Output 1)
D001 0101 ???  <>  0x44 (#) - 0xC4 (A!)   - External Output 2 - to be added
D001 0110 ???  <>  0x45 (#) - 0xC5 (A!)   - External Output 3 - to be added
D001 0110 ???  <>  0x46 (#) - 0xC6 (A!)   - External Output 3 - to be added

1001 1000 KEY  <>  -------  - 0x47 (S!)   - Store the ASCII entered (External Input 1)
1001 1001 ???  <>  -------  - 0x48 (S!)   - To be added             (External Input 2)
1001 1010 JOY  <>  -------  - 0x49 (S!)   - Store the Joystick data (External Input 3)
1001 1011 ???  <>  -------  - 0x4A (S!)   - To be added             (External Input 4)




#######X010 0001 BCD  <>  0x41 (#) - 0xC1 (A)    - Bin to Bcd decoder (not added yet)


 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
   A.4  ARITHMETICH LOGIC UNIT (ALU)
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-

D010 0001 ADD  <>  0x21 (#) - 0xA1 (A!)   - Add
D010 0010 SUB  <>  0x22 (#) - 0xA2 (A!)   - Substract
D010 0011 MUL  <>  0x23 (#) - 0xA3 (A!)   - Multiply
D010 0100 DIV  <>  0x24 (#) - 0xA4 (A!)   - Divide

D010 0101 CMP  <>  0x25 (#) - 0xA5 (A!)   - Compare
D010 0110 ---  <>  0x26 (#) - 0xA6 (A!)   - RESERVED

D010 0111 AND  <>  0x27 (#) - 0xA7 (A!)   - And Logic
D010 1000 OR   <>  0x28 (#) - 0xA8 (A!)   - Or Logic
D010 1001 XOR  <>  0x29 (#) - 0xA9 (A!)   - Xor Logic
D010 1010 NND  <>  0x2A (#) - 0xAA (A!)   - Nand Logic
D010 1011 NOR  <>  0x2B (#) - 0xAB (A!)   - Nor Logic
D010 1100 XNR  <>  0x2C (#) - 0xAC (A!)   - Xnor Logic

D010 1101 SHL  <>  0x2D (#) - 0xAD (A!)   - Shift Left
D010 1110 SHR  <>  0x2E (#) - 0xAE (A!)   - Shift Right
D010 1111 ROL  <>  0x2F (#) - 0xAF (A!)   - Roll Left
D011 0000 ROR  <>  0x30 (#) - 0xB0 (A!)   - Roll Right

[D011 0001 ~ ?011 1000] Not used yet, feel free to add and share new instructions in this interval (floating points would be awesome)

-011 1001 AL2  <>        0x39 (-)         - ALU output 2

D011 1010 FLL  <>  0x3A (#) - 0xBE (A!)   - Find Lowest Low
D011 1011 FHL  <>  0x3B (#) - 0xBE (A!)   - Find Highest Low
D011 1100 FLH  <>  0x3C (#) - 0xBE (A!)   - Find Lowest High
D011 1101 FHH  <>  0x3D (#) - 0xBE (A!)   - Find Highest High

D011 1110 NOT  <>  0x3E (#) - 0xBE (A!)   - Not
D011 1111 NEG  <>  0x3F (#) - 0xBF (A!)     Negate
|
|
|
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
B.                Credits, special thanks and contact
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
|
| Contact me!

    Special thanks to:
        AltruismAndCake - Reddit
        armorall171     - Reddit

    By Henrique Bruno Fantauzzi de Almeida, Rio de Janeiro - RJ, Brazil.
        henrique.bruno.fa@gmail.com
        SrBrahma (Reddit), the Logisim subreddit is: https://www.reddit.com/r/logisim/
        Main post: https://redd.it/47lypv
|
|
|
+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+#+
```
