### MATERIALS REQUIRED

1.	Adalm Pluto SDR (along with its USB cable and antennas)
2.	Phone with radio application and earphones (earphones act as receiver antenna)

### SOFTWARES REQUIRED

1.	MATLAB Simulink
2.	Any built-in or installed radio application on your mobile

### SETUP

#### HARDWARE SETUP:

 
STEP 1: Connect the antennas to the ADALM PLUTO SDR
STEP 2: Connect the PLUTO SDR to your computer using the USB
             Cable
STEP 3: Connect your earphones to your mobile to act as a receiver  
            Antenna and place the phone near your hardware.

The Hardware setup is done.

SOFTWARE SETUP:

In case you don’t already have the “Communications Toolbox Support Package for Analog Devices ADALM-Pluto Radio” package in your MATLAB, go to “Get Hardware Support Packages” in the Add-Ons drop box and install and setup the package.

 
 

STEP 1: Once the package has been installed and set up, open a new
blank model on your Simulink. 
STEP 2: Add the following blocks and connect them in the same order
1.	“From Multimedia File” block from the Audio Toolbox 
2.	“FM Broadcast Modulator Baseband” 
3.	“Adalm Pluto Radio Transmitter”

        STEP 3:  Browse and select your multimedia or audio file that you want
        to transmit in the “From Multimedia File” block 

 
STEP 4: In the block parameters pop-up for FM Broadcast block, make sure the settings are as follows and the stereo audio box is selected.
 
 

STEP 5: In the pop-up settings for the ADALM PLUTO receiver, make sure that the “Enable output port got underflow indicator” box is deselected. And under the Center Frequency (Hz) choose a frequency that is not available/taken by any radio stations near your area. 

 
I have chosen the center frequency of 97 MHz (or 97.0e6 Hz). 

 

STPE 6: Give the stop time as infinity (inf).

 

 
Now the Simulink set-up is done. Let us now look at how we should set up our phone.

STEP 1: Go to your built-in radio application or install a FM radio application.
STEP 2: Select the radio station frequency that you have given in your Simulink, here, 97 MHz

 

STEP 3: Connect your earphones to your phone to act as a receiver antenna. 

Now that the setup is done, run the Simulink code and then turn on the radio, and we can hear the audio that we had transmitted using your Pluto SDR. 

OUTPUT
The video of the output can be found in the below Google Drive Link:

https://drive.google.com/file/d/1oybitRnOT6V51BMUq06X4WFYO0KlrBBd/view?usp=sharing

RESOURCES

1.	Laboratory 1: Introduction to Software-Defined Radio 
         Communication Systems Laboratory

