## MOSFET
"Metal Oxide Semiconductor Field Effect Transistor". Voltage across gate determines conductivity, effectively forming a non-mechanical switch which is controlled electronically.


## CCD
"Charge Coupled Device". An integrated circuit used for high-quality industrial and scientific photographic imaging, in which <mark class="hltr-grey">pixels are represented by individual capacitors</mark> covered by a photoactive material (silicon). Each capacitor in the array can exchange charge with neighboring capacitors, which allows the signal in one pixel to travel to a charge amplifier, converting the signal from a pixel into a voltage.

The quality advantage of CCDs over [[#CMOS]] sensors has diminished in recent years. Both are based on metal oxide semiconductor technology (CCDs on MOS capacitors, and CMOS on [[#MOSFET]] amplifiers).


## Read noise
A CCD can make accurate, but not perfect, measurements of the charge accumulated in each CCD pixel.  One important limitation is the noise associated with the electronics that amplifies and digitizes the charge signal in the CCD readout. Read-out noise is generated in the amplifier on the [[#CCD]] chip that converts the stored charge of each photodiode (i.e., pixel) into an analog voltage to be quantified by A/D conversion. Read-out noise may be viewed as a "toll" that must be paid for reading the stored charge. Similar to Poisson noise it scales with the number of "counts" but linearly rather than the square root: $$\sigma_r = N_r$$Measured by taking zero-count images i think(?) Unclear.



## CMOS 
"Active pixel sensor / complementary [[#MOSFET|MOS(FET)]]". 


