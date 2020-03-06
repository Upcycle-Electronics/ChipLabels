
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

* _*2020.3.5*_ 
  - Updated all (except Motorola) old wide labels to the new template version.
  - New chips added: MSM80C85, MSM81C55, HM6116, NMC27C32, CAT28C256, CAT28C16, G65SC02

* _*2020.15.2*_ 
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
    1.) 74HC00
    2.) 74HC02
    3.) 74HC04
    4.) 74HC05
    5.) 74HC06
    6.) 74HC07
    7.) 74HC08
    8.) 74HC11
    9.) 74HC13
    10.) 74HC14
    11.) 74HC20
    12.) 74HC30
    13.) 74HC32
    14.) 74HC51
    15.) 74HC74
    16.) 74HC75
    17.) 74HC76
    18.) 74HC86
    19.) 74HC107
    20.) 74HC112
    21.) 74HC123
    22.) 74HC132
    23.) 74HC133
    24.) 74HC138
    25.) 74HC139
    26.) 74HC151
    27.) 74HC154
    28.) 74HC157
    29.) 74HC161
    30.) 74HC164
    31.) 74HC165
    32.) 74HC166
    33.) 74HC173
    34.) 74HC181
    35.) 74HC193
    36.) 74HC194
    37.) 74HC240
    38.) 74HC244
    39.) 74HC245
    40.) 74HC251
    41.) 74HC257
    42.) 74HC259
    43.) 74HC273
    44.) 74HC283
    45.) 74HC299
    46.) 74HC365
    47.) 74HC366
    48.) 74HC367
    49.) 74HC368
    50.) 74HC373
    51.) 74HC374
    52.) 74HC377
    53.) 74HC390
    54.) 74HC540
    55.) 74HC541
    56.) 74HC573
    57.) 74HC574
    58.) 74HC590
    59.) 74HC595
    60.) 74HC640
    61.) 74HC641
    62.) 74HC642
    63.) 74HC643
    64.) 74HC644
    65.) 74HC645
    66.) 74HC646
    67.) 74HC670
    68.) 74HC688
    69.) 74HC4017
    70.) 74HC4020
    71.) 74HC4024
    72.) 74HC4040
    73.) 74HC4049h
    74.) 74HC4050h
    75.) 74HC4051
    76.) 74HC4052
    77.) 74HC4053
    78.) 74HC4060
    79.) 74HC4066
    80.) 74HC4514
    81.) 74HC40103
    82.) 74LS00
    83.) 74LS02
    84.) 74LS04
    85.) 74LS05
    86.) 74LS06
    87.) 74LS07
    88.) 74LS08
    89.) 74LS11
    90.) 74LS13
    91.) 74LS14
    92.) 74LS16
    93.) 74LS17
    94.) 74LS20
    95.) 74LS30
    96.) 74LS32
    97.) 74LS51
    98.) 74LS74
    99.) 74LS75
    100.) 74LS76
    101.) 74LS86
    102.) 74LS107
    103.) 74LS112
    104.) 74LS123
    105.) 74LS132
    106.) 74LS133
    107.) 74LS138
    108.) 74LS139
    109.) 74LS151
    110.) 74LS154
    111.) 74LS157
    112.) 74LS161
    113.) 74LS164
    114.) 74LS165
    115.) 74LS166
    116.) 74LS173
    117.) 74LS181
    118.) 74LS189
    119.) 74LS193
    120.) 74LS194
    121.) 74LS240
    122.) 74LS244
    123.) 74LS245
    124.) 74LS251
    125.) 74LS257
    126.) 74LS259
    127.) 74LS273
    128.) 74LS283
    129.) 74LS299
    130.) 74LS365
    131.) 74LS366
    132.) 74LS367
    133.) 74LS368
    134.) 74LS373
    135.) 74LS374
    136.) 74LS377
    137.) 74LS390
    138.) 74LS540
    139.) 74LS541
    140.) 74LS573
    141.) 74LS574
    142.) 74LS590
    143.) 74LS595
    144.) 74LS640
    145.) 74LS641
    146.) 74LS642
    147.) 74LS643
    148.) 74LS644
    149.) 74LS645
    150.) 74LS646
    151.) 74LS670
    152.) 74LS688
    153.) 74ACT251
    154.) 74F189
    155.) 74HCT00
    156.) 74HCT02
    157.) 74HCT32
    158.) 74HCT138
    159.) 74HCT193
    160.) 74HCT244
    161.) 74HCT245
    162.) 74HCT251
    163.) 74HCT540
    164.) 74HCT541
    165.) 74HCT646
    166.) 74HCT688
    167.) 74S189
    168.) DM7599
    169.) DM8599
    170.) CD4011
    171.) CD4013
    172.) CD4017
    173.) CD4020
    174.) CD4024
    175.) CD4040
    176.) CD4049h
    177.) CD4050h
    178.) CD4051
    179.) CD4052
    180.) CD4053
    181.) CD4060
    182.) CD4066
    183.) CD40103
    184.) AT89C2051
    185.) ATMEGA328
    186.) PIC18F26K22
    187.) CY7C199
    188.) IS61C1024
    189.) 11C90(NAR)
    190.) CA723
    191.) DAC0800(NAR)
    192.) DAC0808
    193.) GAL16V8
    194.) ICM7555
    195.) LM555
    196.) MAX202
    197.) MAX232
    198.) MAX233
    199.) MAX7219
    200.) MC144111
    201.) MC145157P2
    202.) MIC2981
    203.) SN754410
    204.) ULN2003
    
    205.) MAX512
    206.) MAX513
    
    207.) KID65783
    208.) PT2262
    209.) PT2272
    210.) MAX7221
    211.) TD62084
    212.) XR2240
    
    213.) MSM80C85
    214.) MSM81C55
    215.) HM6116
    216.) NMC27C32
    217.) CAT28C256
    218.) CAT28C16
    219.) G65SC02
    
