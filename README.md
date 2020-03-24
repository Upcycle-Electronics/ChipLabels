
<img src="https://raw.githubusercontent.com/Upcycle-Electronics/ChipLabels/master/LS-labels.jpg" height="200">


# DIP Chip Labels

* Copyright 2020 Jake Little
* These files and original documents are [MIT licensed](http://en.wikipedia.org/wiki/MIT_License).

## What's in the Folders
 - _*GIMP*_   .xcf files from GIMP 2.10 in Ubuntu
 - _*Labels - Ready to Print PDF's*_   Individual PDF files for each label on an 8.5 x 11 inch background
 - _*BenEaters6502/8b-BC*_   All the labels for Ben's 6502 and 8 Bit Breadboard Computer project thus far.
 
 <img src="https://raw.githubusercontent.com/Upcycle-Electronics/ChipLabels/master/example-labels.jpg" width="500">
 
## Significant Updates

* _*2020.3.23*_ 
  - Updated the list of chips with premade PDF labels at the end of this page
  - New chips added: AY-3-8910, ICL7106, ICL7107, ICL7107S, ICL7135, ICM7216B, ICM7216D, NTE2050, P8251A, PIC18F46K22, PIC18F45K22, PIC18F44K22, PIC18F43K22, PIC18F26K22, PIC18F25K22, PIC18F24K22, PIC18F23K22, TMP82C79P-2
  
* _*2020.3.5*_ 
  - Updated all (except Motorola) old wide labels to the new template version.
  - New chips added: MSM80C85, MSM81C55, HM6116, NMC27C32, CAT28C256, CAT28C16, G65SC02

* _*2020.2.15*_ 
  - Added Readme entry (end) with a list of all chips that have PDF's made already
  - New chips added: MC144111, IS61C1024, CA723, MAX202, DAC800, DAC0808
  - Labels edited/added to: 74x138, 74x157, 74x173, 74x273, 74x283, 74x377, 74x390, 74x40103

* _*2020.2.2*_ 
  - Created "Significant Updates"
  - Revised DIPwideMAIN.xcf with a similar hierarchical layer structure as DIPstandardMAIN.xcf
  - Added a vertical FAB guide layer to DIPwideMAIN.xcf and expanded the Custom Q/Gates/Truth Tables copied from standardMain.xcf
  - Created new standardized 24, 28, 32, 40, and 48 pin blank frame templates
  - Listed the text settings I'm currently using in a layer called The Standard Standard
  - Created a '_TEN PDF with all Zilog Z80 CPU's and added a new Zilog folder to the premade PDF labels posted here.
 
## Document Viewers 

 You may need to try different PDF viewers and print settings to get these to print right. I use the default “Document Viewer” that came with Lubuntu. I have tried printing from Firefox, Okular, and GIMP directly. With the 8.5 x 11 inch background I get good print results from most. Without the sized background the Document Viewer is the only one that prints at the correct print scale.
  I print, cut these out, and glue them on with stick-type school glue. It holds but is easy to clean off too.
  
##  Making Your Own Sheets of Labels
 Inside the GIMP  standard .xcf file the individual finished labels are created as layers and filed away under the following: Files > Labels-toPrint. I use the GIMP file to make sheets with lots of labels to print at once. I get the layers tab visible on the right side of GIMP. If you are not familiar with GIMP the layers menu should be on the right side in the docked frame. If it is not, then navigate the little tab like icons that should be at the top of the right side menu. The layers menu looks like a file directory with folders. After you've found the layers menu, find the labels you want to make. In the layers menu, right click on the labels you want to print, and select "Duplicate Layer." Then left click and drag each of the duplicate layers outside of the main "Files" layer group. Once this is done, duplicate them as necessary and place them in whatever pattern you think will make it easy to cut them out. Now merge the labels together into a single layer. To do this, make sure only the layers you have copied for printing are visible with a little eye icon beside them in the layers menu, then press (control + M) and hit enter, the default settings should work. This merges them together into a single layer. I usually save my work at this point because the the next step will use a lot more system resources (control + S). 
  
  Now, at the bottom of the layers menu on the right select the little white paper icon to add a new layer. On the options menu that pops up, name the layer, and change the dimensions from PX to Inches. Then set the X axis to 8.5 inches and the Y axis to 11 inches. Below this change the offset units to inches. Change the offset to -1 and -1 in each box. Lastly, be sure the setting option at the bottom of the menu is set to White, and click OK. This layer needs to be lower on the layer menu list than the labels you want to print, you can just click and drag them around to reorder them. The canvas still needs to be sized to fit this new background layer. Click on the Image tab on the pull down menu bar at the top of the page. Now select "Fit canvas to Layers." Everything should be setup for printing now. I haven't had success printing directly from GIMP using the File > Print option. I use the "Export" feature. Click on File > Export. Now select where you would like to save a PDF to print. Name the file what ever you want then type .pdf at the end to tell GIMP to create a PDF. The default options are fine. Once this is done check the PDF file to be sure everything looks right and print the file. I always go back into gimp at this point and change from the layers dock on the right to the undo history tab. I then reset the history to the marker just before I created the 8.5 x 11 inch background. This is by-far the fastest way to reduce the size of the canvas and entire file to keep it manageable despite having so many layers, and complexity. I always delete the file/label layer I made for printing. 
  
## Make New Labels (Standard):
   Start off with the datasheet pin-out in view. Duplicate one of the blank templates with the correct pin count. Templates are in a folder at the bottom of the Files folder. Copy the layer and take it to the top. Next you will find a folder called FAB that has line guides I use to make labels. It's set up to establish the location of each line of text, and the center line of every pin. The best way to see how I use this guide layer is to look at one of the more simple completed labels from the 74-Series. The top and bottom of the FAB guide has a couple of colored semi opaque lines that delineate where the Pin number text belongs. This text is size 65 Ubuntu-Bold with the letter spacing set to -2 on all newer style labels. Next, there are two thick green bars on the FAB guide. These are for the Inverted bars that go above Pin descriptions. The bar height is the minimum thickness for the bars to show up on my printers. I make a box the width of the pin name and use the green bar to locate it vertically, then fill the box with the paint tool. I always try to make the bars 2 pixels taller than the green guide. Next, in the middle of the green bar there is a darker green line. This is the top guide for the height of pin text. There is another line guide below. This is setup for two text sizes. With the Ubuntu-Bold font selected, I use a size 60 font for most 2 character pin names. If you look at the FAB guide layer, I have a copy of the entire alphabet and numerals with funny coloring. This is split to show which numbers and letters extend onto the text guide lines. The letters with green or red overlap the line on one side or the other. This just keeps everything centered straight and uniform for each label. I mentioned this text guide is for two sizes of text. The second size is 52 instead of 60. I only use the lower guide line for this size text. Size 52 will place the text just below the inverted bar guide. This is also my standard text size for anything longer than 2 characters. I try to limit pin text to these two sizes but occasionally I use a size 48 for something really wide. Size 45 is the smallest that I can print and read most of the time. I have made a few labels that even have size 35 text, but it is challenging to get this to print legibly. The center of the FAB guide label area has a few yellow lines. These are my guidelines for centering the part number and title. I use Ubuntu-Bold-Italic for all of this text. I try to always print this text in size 100 although it is tough to fit sometimes. I set the character width spacing to the smallest I can manage without letting the letters touch each other. There are also several templates saved in the FAB guide layer. This is where I make and save a copy of gates, truth tables or anything else I've tried and might want to reuse later. I also have a bunch of custom fonts made with the letter Q and the sizes of text I use marked below them. This is specifically because the upper case Ubuntu font's "Q" is the only letter that extends below the bottom boundary of the rest of the letters in the font. This creates lots of interference issues. Of the dozens of fonts I tried none of them print as well as Ubuntu in the required size range. Most fonts that have a more compact capital Q print like a zero or O at the sizes required. To use these custom Q's, I copy the one I need into it's own layer from the FAB guide. I just use the regular Ubuntu-Bold Q font when I'm making the text for a label. Once I have everything setup where I want it, I go back and align the copied custom Q's over the typed Q. The circumference of the custom Q is identical to the same size Ubuntu font. The exaggerated cross of the custom Q and the gap makes it quite definitive even at the smallest sizes. It also has a much more manageable lower extension for fitting more text in tight spaces.
   
## Nuts and Bolts Details
  Where do I get my pin descriptions? They are usually based on a combination of Texas Instruments, Motorola, and Fairchild datasheets. I often use the old databooks directly. If you are not aware, Archive.org/bit-savers has thousands of free databooks available for download. I don't commit to following any specific datasheet pin nomenclature though. If the nomenclature requires me to look at a datasheet description to figure out it's basic meaning or function I won't use it assuming I can think of something more obvious and intuitive. For instance, I will not use CP for Clock or MR for Reset. I use CLK and RST. I think "G" was intended to mean "gate" for the enable function. I don't like it.  I call it EN or OE and IE. I'm moving towards even more detailed ways of labeling special function pins by replacing the pin number with 2 lines of text. I generally try to avoid using O. I will use Y for gate outputs, and use Q like a crossed O or O-proper for an output. I just don't want to wonder if I'm looking at a zero or O. In most instances where there are 8 pins, I label them 0-7 like the buses they are most likely to be used with. Also of note, there are several labels with various alternate versions. I usually made one, didn't like it, or wanted to see if I could fit more functionality. I just kept the old version too. It might be useful to someone with a lower resolution printer. There are several labels with a (NAR) ending. These are narrow versions. It means the inventory I have has the narrow half pin end with the shortened body without much overhang beyond the last pins. My regular labels hang over the ends of these chips by around 1mm on both sides. They are still functional, but it just bugs me so I started making a narrow version that fits tighter. As of January 28th 2020, I have started making a 3rd type of label. These use a new template set named hybrid. This template is setup between the standard (original) and Narrow size templates. Specifically, with the resolution setup in GIMP 120 pixels is 0.1 inch or 2.54mm. The Standard template extends past the corner pins by 55 pixels from the corner pins' center line to the center of the template outline. The Narrow template extends 10 pixels past center line and the Hybrid is 34 pixels larger (standard=55 narrow=10 hybrid=34). This means the hybrid may still extend slightly over the edge of some narrow chips, but is a way for me to make some of these things faster. It is easiest to make labels in the standard size where less specific adjustments are needed to fit text. Narrow usually requires far more manipulation. Hybrid is just a happy medium.
   
  Lastly, It should go without saying...but I will anyways, assume everything I have done is wrong and double check the pin-outs before using them. If you find an error before I do, feel free to let me know. I’m sure I’ll figure it out eventually and update it. Hopefully this is useful to you, but I make these for myself.
-Jake

## List of all Chips with Labels Made

These are all made in GIMP and is the hierarchal order they are roughly listed as layers.

    (AS OF Feb 20)
    1.)   11C90           1190
    2.)   74ACT251        74251
    3.)   74F189          74189
    4.)   74HC00          7400
    5.)   74HC02          7402
    6.)   74HC04          7404
    7.)   74HC05          7405
    8.)   74HC06          7406
    9.)   74HC07          7407
    10.)  74HC08          7408
    11.)  74HC107         74107
    12.)  74HC11          7411
    13.)  74HC112         74112
    14.)  74HC123         74123
    15.)  74HC13          7413
    16.)  74HC132         74132
    17.)  74HC133         74133
    18.)  74HC138         74138
    19.)  74HC139         74139
    20.)  74HC14          7414
    21.)  74HC151         74151
    22.)  74HC154         74154
    23.)  74HC157         74157
    24.)  74HC161         74161
    25.)  74HC164         74164
    26.)  74HC165         74165
    27.)  74HC166         74166
    28.)  74HC173         74173
    29.)  74HC181         74181
    30.)  74HC193         74193
    31.)  74HC194         74194
    32.)  74HC20          7420
    33.)  74HC240         74240
    34.)  74HC244         74244
    35.)  74HC245         74245
    36.)  74HC251         74251
    37.)  74HC257         74257
    38.)  74HC259         74259
    39.)  74HC273         74273
    40.)  74HC283         74283
    41.)  74HC299         74299
    42.)  74HC30          7430
    43.)  74HC32          7432
    44.)  74HC365         74365
    45.)  74HC366         74366
    46.)  74HC367         74367
    47.)  74HC368         74368
    48.)  74HC373         74373
    49.)  74HC374         74374
    50.)  74HC377         74377
    51.)  74HC390         74390
    52.)  74HC40103       7440103
    53.)  74HC4017        744017
    54.)  74HC4020        744020
    55.)  74HC4024        744024
    56.)  74HC4040        744040
    57.)  74HC4049        744049
    58.)  74HC4050        744050
    59.)  74HC4051        744051
    60.)  74HC4052        744052
    61.)  74HC4053        744053
    62.)  74HC4060        744060
    63.)  74HC4066        744066
    64.)  74HC4514        744514
    65.)  74HC51          7451
    66.)  74HC540         74540
    67.)  74HC541         74541
    68.)  74HC573         74573
    69.)  74HC574         74574
    70.)  74HC590         74590
    71.)  74HC595         74595
    72.)  74HC640         74640
    73.)  74HC641         74641
    74.)  74HC642         74642
    75.)  74HC643         74643
    76.)  74HC644         74644
    77.)  74HC645         74645
    78.)  74HC646         74646
    79.)  74HC670         74670
    80.)  74HC688         74688
    81.)  74HC74          7474
    82.)  74HC75          7475
    83.)  74HC76          7476
    84.)  74HC86          7486
    85.)  74HCT00         7400
    86.)  74HCT02         7402
    87.)  74HCT138        74138
    88.)  74HCT193        74193
    89.)  74HCT244        74244
    90.)  74HCT245        74245
    91.)  74HCT251        74251
    92.)  74HCT32         7432
    93.)  74HCT540        74540
    94.)  74HCT541        74541
    95.)  74HCT646        74646
    96.)  74HCT688        74688
    97.)  74LS00          7400
    98.)  74LS02          7402
    99.)  74LS04          7404
    100.)  74LS05          7405
    101.)  74LS06          7406
    102.)  74LS07          7407
    103.)  74LS08          7408
    104.)  74LS107         74107
    105.)  74LS11          7411
    106.)  74LS112         74112
    107.)  74LS123         74123
    108.)  74LS13          7413
    109.)  74LS132         74132
    110.)  74LS133         74133
    111.)  74LS138         74138
    112.)  74LS139         74139
    113.)  74LS14          7414
    114.)  74LS151         74151
    115.)  74LS154         74154
    116.)  74LS157         74157
    117.)  74LS16          7416
    118.)  74LS161         74161
    119.)  74LS164         74164
    120.)  74LS165         74165
    121.)  74LS166         74166
    122.)  74LS17          7417
    123.)  74LS173         74173
    124.)  74LS181         74181
    125.)  74LS189         74189
    126.)  74LS193         74193
    127.)  74LS194         74194
    128.)  74LS20          7420
    129.)  74LS240         74240
    130.)  74LS244         74244
    131.)  74LS245         74245
    132.)  74LS251         74251
    133.)  74LS257         74257
    134.)  74LS259         74259
    135.)  74LS273         74273
    136.)  74LS283         74283
    137.)  74LS299         74299
    138.)  74LS30          7430
    139.)  74LS32          7432
    140.)  74LS365         74365
    141.)  74LS366         74366
    142.)  74LS367         74367
    143.)  74LS368         74368
    144.)  74LS373         74373
    145.)  74LS374         74374
    146.)  74LS377         74377
    147.)  74LS390         74390
    148.)  74LS51          7451
    149.)  74LS540         74540
    150.)  74LS541         74541
    151.)  74LS573         74573
    152.)  74LS574         74574
    153.)  74LS590         74590
    154.)  74LS595         74595
    155.)  74LS640         74640
    156.)  74LS641         74641
    157.)  74LS642         74642
    158.)  74LS643         74643
    159.)  74LS644         74644
    160.)  74LS645         74645
    161.)  74LS646         74646
    162.)  74LS670         74670
    163.)  74LS688         74688
    164.)  74LS74          7474
    165.)  74LS75          7475
    166.)  74LS76          7476
    167.)  74LS86          7486
    168.)  74S189          74189
    169.)  A29040          29040
    170.)  AT28C16         2816
    171.)  AT28C256        28256
    172.)  AT89C2051       892051
    173.)  ATMEGA328       328
    174.)  AY-3-8910       38910
    175.)  CA723           723
    176.)  CAT28C16        2816
    177.)  CAT28C256       28256
    178.)  CD40103         40103
    179.)  CD4011          4011
    180.)  CD4013          4013
    181.)  CD4017          4017
    182.)  CD4020          4020
    183.)  CD4024          4024
    184.)  CD4040          4040
    185.)  CD4049h         4049
    186.)  CD4050h         4050
    187.)  CD4051          4051
    188.)  CD4052          4052
    189.)  CD4053          4053
    190.)  CD4060          4060
    191.)  CD4066          4066
    192.)  CY7C199         7199
    193.)  DAC0800         0800
    194.)  DAC0808         0808
    195.)  DM7599          7599
    196.)  DM8599          8599
    197.)  G65SC02         6502
    198.)  G65SC816        65816
    199.)  GAL16V8         168
    200.)  HM6116          6116
    201.)  HM65256         65256
    202.)  ICL7106         7106
    203.)  ICL7107         7107
    204.)  ICL7135         7135
    205.)  ICM7216         7216
    206.)  ICM7555         7555
    207.)  IS61C1024       611024
    208.)  KID65783        65783
    209.)  LM555           555
    210.)  MAX202          202
    211.)  MAX232          232
    212.)  MAX233          233
    213.)  MAX512          512
    214.)  MAX513          513
    215.)  MAX7219         7219
    216.)  MAX7221         7221
    217.)  MC144111        144111
    218.)  MC145157P2      145157
    219.)  MC68000         68000
    220.)  MC68008         68008
    221.)  MC68010         68010
    222.)  MC6809          6809
    223.)  MC6821          6821
    224.)  MC68230         68230
    225.)  MC6845          6845
    226.)  MC6850          6850
    227.)  MC68901         68901
    228.)  MC68HC000       68000
    229.)  MIC2981         2981
    230.)  MOS6502         6502
    231.)  MOS6522         6522
    232.)  MSM80C85        8085
    233.)  MSM81C55        8155
    234.)  NMC27C32        2732
    235.)  NTE2050         2050
    236.)  P8251A          8251
    237.)  PIC18F23K22     182322
    238.)  PIC18F24K22     182422
    239.)  PIC18F25K22     182522
    240.)  PIC18F26K22     182622
    241.)  PIC18F43K22     184322
    242.)  PIC18F44K22     184422
    243.)  PIC18F45K22     184522
    244.)  PIC18F46K22     184622
    245.)  PT2262          2262
    246.)  PT2272          2272
    247.)  R65C02          6502
    248.)  R65C22          6522
    249.)  SN754410        754410
    250.)  TD62084         62084
    251.)  TMP82C79P-2     8279
    252.)  ULN2003         2003
    253.)  VL65C816        65816
    254.)  W65C02S         6502
    255.)  W65C22          6522
    256.)  W65C816         65816
    257.)  XR2240          2240
    
    
    
