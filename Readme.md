# CUDA on a HP ProLiant DL360p G8 server  

We tested two ways to use a Nvidia compatible GPU card in a HP ProLiant DL 360 rackmount server for number crunching with Cuda. 

The challange was to find:
1) a low (not low profile) card with only 1 PCI slot high
2) a low power consuming card that take its power via PCI bus and do not need extra power plug
 

### ------------------------------------------

## MSI GeForce GT 1030
First we use a very cheap card (MSI GeForce GT 1030 with 384 cuda cores) that was working fine. We are useing Linux and mathlab.
This card can be used without modifications. 

MSI GeForce GT 1030:
- 384 CUDA Cores
- 2GB 64-Bit DDR4
- PCI Express 3.0 x16 (Uses x4)
- Maximum Power Consumption 	30 W

![MSI GeForce GT 1030 view from top](IMG-20180925-WA0009.jpg)
![MSI GeForce GT 1030 view from side](IMG-20180925-WA0006.jpg)

### ------------------------------------------

	
## NVIDIA Quadro P2000
With a grant from Nvidia to one of our research group  we could use a NVIDIA Quadro P2000. 

**WARNING: You need to modifiy the hood cover and remove the the opener. Maybe you lose your warranty!**

NVIDIA Quadro P2000: 
- CUDA Cores 	1024
- GPU Memory 	5 GB GDDR5	
- System Interface 	PCI Express 3.0 x16
- Maximum Power Consumption 	75 W

![MSI GeForce GT 1030 side view](IMG-20181017-WA0001.jpg)

Remove the opener by drilling out the opener rivets. Otherwise you could not close the top of the server. 
Seal the whole with duct tape or what you like if no server is above this one in the rack. The card should 
benefit of of the server ventilation. 

![MSI GeForce GT 1030 side view](IMG-20181017-WA0002.jpg)

### ------------------------------------------

Both solutions are working fine for cuda number crunching. 

We did not use or test the display port!


### ------------------------------------------

QuickSpecs
HP ProLiant DL360 Generation 8 (G8) (https://h20195.www2.hpe.com/v2/getdocument.aspx?docname=c04128242)

