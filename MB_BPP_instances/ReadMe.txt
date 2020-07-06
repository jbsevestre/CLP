Description for MB Benchmark files
-----------------------------------

Problem instances were introduced in:

Daniel Mack and Andreas Bortfeldt
"Eine Heuristik fuer das mehrdimensionale Bin Packing Problem"
Diskussionsbeitrag 423, April 2008
University in Hagen, Germany

------------------------------------------------------

1800 instances are divided in 12 testcases with 150 problems each;

Filename:
MBxx_yyy

where 
xx  = Testcase 01 - 12
yyy = 001 - 150

------------------------------------------------------

Each problem is given in the following tab-delimited format
that is very intuitive to read, 
as it contains a description of the data within the file.

It was introduced to get a rapid overview of the problem,
e.g. by opening it in Mircosoft Excel as a txt-file. 

File-structure: 
---------------

Line 01: Header: <Authors>

Line 02: Header: "Bin-Packing-Problem"

Line 03: Problem type specification:
         BP-RG   (BP=Bin-Packing, R=restriction free, G=guillotine)
	 /SBSBPP (Single Bin Size Bin Packing Problem)
	 /SSSCSP (Single Stock Size Cutting stock Problem)

Line 04: "Testcase-ID"\t<xx> 
         ( "\t" stands for the 'tab' code ascii(9), 
 	   <xx> stands for the value of xx )

Line 05: "Problem-ID" \t <yyy>

Line 06: "no_item_types" \t <number of item types>

Line 07: "no_items" \t <total number of items of all types>

Line 07: Header: "CONTAINER_DATA: \t l \t w \t h"

Line 08: "CONTAINER_DATA (l,h,w)"
        \t<container-length>
        \t<Container-width>
	\t<Container-height> 

Line 09: Header "ITEMS_DATA:"

Line 10: Header "Type \t x \t y \t z \t no_items"

LIne 11 to Line (10+<number of item types>):
	Description for the different item types (one line per type),
        given in the following format:
	<type-id>
	\t <item-length> (maximum item dimension)
	\t <item-width>  (medium item dimension)
	\t <item-height> (minimum item dimension)
	\t <number of items> (available items of this type)

All the items may be rotated freely within the container, 
there is no orientational restriction to be respected.

------------------------------------------------------------------------
April 2008 - Daniel Mack
For furher questions, please contact: daniel.mack@lcns.net