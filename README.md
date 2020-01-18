# DIL Chip Labels

Copyright 2019 Jake Little

These files and original documents are [MIT licensed](http://en.wikipedia.org/wiki/MIT_License).

## What's Here
 - _*GIMP*_   .xcf files from GIMP 2.10 in Ubuntu
 - _*Labels*_   Individual PDF files for each label on an 8.5 x 11 inch background
 - _*BenEaters6502/8b-BC*_   All the labels for Ben's 6502 and 8 Bit Breadboard Computer project thus far.
 
 <img src="https://raw.githubusercontent.com/Upcycle-Electronics/ChipLabels/master/example-labels.jpg" width="500">

## Document Viewers 

 You may need to try different PDF viewers and print settings to get these to print right. I use the default “Document Viewer” that came with Lubuntu. I have tried printing from Firefox, Okular, and GIMP directly. With the 8.5 x 11 inch background I get good print results from most. Without the sized background the Document Viewer is the only one that prints at the correct print scale.
  I print, cut these out, and glue them on with stick-type school glue. It holds but is easy to clean off too.
  
##  Making Your Own Sheets of Labels
 Inside the GIMP  standard .xcf file the individual finished labels are created as layers and filed away under the following: Files > Labels-toPrint. I use the GIMP file to make sheets with lots of labels to print at once. I get the layers tab visible on the right side of GIMP. If you are not familiar with GIMP the layers menu should be on the right side in the docked frame. If it is not, then navigate the little tab like icons that should be at the top of the right side menu. The layers menu looks like a file directory with folders. After you've found the layers menu, find the labels you want to make. In the layers menu, right click on the labels you want to print, and select "Duplicate Layer." Then left click and drag each of the duplicate layers outside of the main "Files" layer group. Once this is done, duplicate them as necessary and place them in whatever pattern you think will make it easy to cut them out. Now merge the labels together into a single layer. To do this, make sure only the layers you have copied for printing are visible with a little eye icon beside them in the layers menu, then press (control + M) and hit enter, the default settings should work. This merges them together into a single layer. I usually save my work at this point because the the next step will use a lot more system resources (control + S). 
  
  Now, at the bottom of the layers menu on the right select the little white paper icon to add a new layer. On the options menu that pops up, name the layer, and change the dimensions from PX to Inches. Then set the X axis to 8.5 inches and the Y axis to 11 inches. Below this change the offset units to inches. Change the offset to -1 and -1 in each box. Lastly, be sure the setting option at the bottom of the menu is set to White, and click OK. This layer needs to be lower on the layer menu list than the labels you want to print, you can just click and drag them around to reorder them. The canvas still needs to be sized to fit this new background layer. Click on the Image tab on the pull down menu bar at the top of the page. Now select "Fit canvas to Layers." Everything should be setup for printing now. I haven't had success printing directly from GIMP using the File > Print option. I use the "Export" feature. Click on File > Export. Now select where you would like to save a PDF to print. Name the file what ever you want then type .pdf at the end to tell GIMP to create a PDF. The default options are fine. Once this is done check the PDF file to be sure everything looks right and print the file. I always go back into gimp at this point and change from the layers dock on the right to the undo history tab. I then reset the history to the marker just before I created the 8.5 x 11 inch background. This is by-far the fastest way to reduce the size of the canvas and entire file to keep it manageable despite having so many layers, and complexity. I always delete the file/label layer I made for printing. 
  
## Make New Labels (Standard):
   Start off with the datasheet pin-out in view. Duplicate one of the blank templates with the correct pin count. Templates are in a folder at the bottom of the Files folder. Copy the layer and take it to the top. Next you will find a folder called FAB that has line guides I use to make labels. It's set up to establish the location of each line of text, and the center line of every pin. The best way to see how I use this guide layer is to look at one of the more simple completed labels from the 74-Series. The top and bottom of the FAB guide has a couple of colored semi opaque lines that delineate where the Pin number text belongs. This text is size 65 Ubuntu-Bold with the letter spacing set to -2 on all newer style labels. Next, there are two thick green bars on the FAB guide. These are for the Inverted bars that go above Pin descriptions. The bar height is the minimum thickness for the bars to show up on my printers. I make a box the width of the pin name and use the green bar to locate it vertically, then fill the box with the paint tool. I always try to make the bars 2 pixels taller than the green guide. Next, in the middle of the green bar there is a darker green line. This is the top guide for the height of pin text. There is another line guide below. This is setup for two text sizes. With the Ubuntu-Bold font selected, I use a size 60 font for most 2 character pin names. If you look at the FAB guide layer, I have a copy of the entire alphabet and numerals with funny coloring. This is split to show which numbers and letters extend onto the text guide lines. The letters with green or red overlap the line on one side or the other. This just keeps everything centered straight and uniform for each label. I mentioned this text guide is for two sizes of text. The second size is 52 instead of 60. I only use the lower guide line for this size text. Size 52 will place the text just below the inverted bar guide. This is also my standard text size for anything longer than 2 characters. I try to limit pin text to these two sizes but occasionally I use a size 48 for something really wide. Size 45 is the smallest that I can print and read most of the time. I have made a few labels that even have size 35 text, but it is challenging to get this to print legibly. The center of the FAB guide label area has a few yellow lines. These are my guidelines for centering the part number and title. I use Ubuntu-Bold-Italic for all of this text. I try to always print this text in size 100 although it is tough to fit sometimes. I set the character width spacing to the smallest I can manage without letting the letters touch each other. There are also several templates saved in the FAB guide layer. This is where I make and save a copy of gates, truth tables or anything else I've tried and might want to reuse later. I also have a bunch of custom fonts made with the letter Q and the sizes of text I use marked below them. This is specifically because the upper case Ubuntu font's "Q" is the only letter that extends below the bottom boundary of the rest of the letters in the font. This creates lots of interference issues. Of the dozens of fonts I tried none of them print as well as Ubuntu in the required size range. Most fonts that have a more compact capital Q print like a zero or O at the sizes required. To use these custom Q's, I copy the one I need into it's own layer from the FAB guide. I just use the regular Ubuntu-Bold Q font when I'm making the text for a label. Once I have everything setup where I want it, I go back and align the copied custom Q's over the typed Q. The circumference of the custom Q is identical to the same size Ubuntu font. The exaggerated cross of the custom Q and the gap makes it quite definitive even at the smallest sizes. It also has a much more manageable lower extension for fitting more text in tight spaces.
   
## Nuts and Bolts Details
   Where do I get my pin descriptions? They are usually based on a combination of Texas Instruments(primary), Motorola, and Fairchild datasheets. I often use the databooks directly. If you are not aware, Archive.org/bit-savers has thousands of free databooks available for download. I don't commit to following any specific datasheet pin nomenclature though. If the nomenclature requires me to look at a datasheet description to figure out it's basic meaning or function I won't use it if I can think of something more obvious and intuitive. I will not use CP for Clock or MR for Reset. I use CLK and RST. The think "G" was intended to mean "gate" when Texas Instruments used it for the enable function. I don't like it.  I call it EN or OE and IE. I'm moving towards even more detailed ways of labeling special function pins by replacing the pin number with 2 lines of text. I generally try to avoid using O. I will use Y for gate outputs, and use Q like a crossed O or O-proper for an output. I just don't want to wonder if I'm looking at a zero or O. There are a few labels still around with 8 channels and either A-H or 1-8 pin names. In most (probably all) cases I made this pin-out as an alternate version because this is how it was done on a datasheet. In all instances where there are 8 pins, I now label them 0-7 just like the buses they are most likely to be used with. Also of note, there are several labels with various alternate versions. I usually made one, didn't like it, or wanted to see if I could fit more functionality. I just kept the old version too. It might be useful to someone with a lower resolution printer. There are several labels with a (NAR) ending. These are narrow versions. It means the inventory I have has the narrow half pin end with the shortened body without much overhang beyond the last pins. My regular labels hang over the ends of these chips by around 1mm on both sides. They are still functional, but it just bugs me so I started making a narrow version that fits tighter.
   
  Lastly, It should go without saying...but I will anyways, assume everything I have done is wrong and double check the pin-outs before using them. If you find an error before I do, feel free to let me know. I’m sure I’ll figure it out eventually and update it. Hopefully this is useful to you, but I make these for myself.
-Jake
