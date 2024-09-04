Equipment
==========
*to be implemented*

MRI Scanner
--------
Siemens Prisma 3T:
  * actively shielded;
  * whole body 3T magnet;
  * 80mT/m gradients with a slew rate og 200 T/m/s;
  * 20ch and 64ch Head/Neck RF Coil for experimental neuroimaging applications.

Peripheral Equipment
----------
  * 32" LCD for visual stimuli from Nordic NeuroLab (NNL), always inside the Magnet room (see Visual Presentation section);
  * 2 x 4 button response pads (Cedrus LP-400 Response pad and Cedrus Lumina LSC-400B Controller);
  * MR compatible glass frames (adult and pediatric, max visual correction from -6 to +6 with intervals of 0.5);
  * tactile piezoelectric stimulator, 2 x 5 fingers (QuaeroSys);
  * Eye Tracker (Eyelink1000);
  * physiological data monitoring and recording (ECG, pOx, Resp tracking);

Stimulation PCs
---------
MRI Lab provides the researchers with:
  * a Stimulation PC located in the control room, connected to the Peripheral Equipment within the Magnet room and equipped with a stimulation software. The Stim-PC can receive triggers from the scanner and responses from the NNL ButtonBox systems;

  * a Training PC, clone of the Stim-PC, can be found in the MRI Area and used to test paradigms and to train subjects outside the MR Scanner.

HW Specs
~~~~~~~~~~
  * CPU: 
  * GPU:
  * RAM:

The Stim-PC is connected to the NNL Monitor, used to present visual stimuli. Images can be seen by the subject through a mirror put on the Head/Neck Coil.

Instructions for users
~~~~~~~~~~
  * Access to Stim-PC: the password is printed on LCD monitor in the control room. You must log in locally, the PC has not Internet connection;
  * Connection: use a portable device (most likely an USB Drive) to copy your script in the designed folder on the Stim-PC.

Updates and Development
------
The descripted hardware and software equipment is the standard configuration of the Stim-PC. Updates made by MRI Lab will be announced in advance and described to the users. Potential specific configurations should be requested by sending an email to MRI Lab staff. The staff will discuss if and how implement requested changes in the lab environment.

Nordic NeuroLab Box
------
Signals coming from Scanner Room are managed by Nordic NeuroLab Box (NNL Box), which is connected to the button boxes through a optic fiber cable and to the scanner through a BNC cable.
NNL Box is in turn connected to the Stim-PC through USB. Stim-PC collect signal from the scanner room as if it was an external USB keyboard.
This means that whenever a signal is sent from within scanner room, numbers appear on the Stim-PC. Keep this in mind when you need to collect responses within your matlab code.

Scanner Sync
--------
The scanner, during functional acquisitions, sends a 50μs "pulse" every TR, marking in this way the "volumes" of your MRI experiment. Synchronization with the scanner trigger is provided through a BNC cable connected to the NordicNeuroLab box, attached to Stim-PC via a USB Port. Stim-PC collect triggers as if someone was systematically pressing "5" key (the one located in the alphanumeric part of the keyboard) at the beginning of each volume acquisition. This means that in debugging, you can test your scripts by simply accepting "5" key.

Participants' responses
----------
MRI Lab provides two 4-button boxes for the participant to send responses while performing inside the scanner. Buttons are arranged in a linear way. They are marked as right and left through a duct tape. They send, respectively, "1","2","3","4" and "6","7","8","9" keys to Stim-PC.

You can check the responses by focusing on NNL Box during the experiments. Specific green leds light up when a button is pressed.

Visual Presentation
---------
For the visual stimuli presentation MR-Lab provides a compatible Nordic NeuroLab LCD monitor positioned at the back of the magnet bore.

Basic monitor specs include: 878 mm horizontal x 485 mm vertical; 3840 x 2160 pixels; surface luminance 350 c/m2; contrast ratio 5000:1 typ, refresh rate 60Hz @ UHD, 120Hz @ FHD.

Auditory Presentation
----------
Current setup includes very basic auditory capabilities. Participants can hear auditory stimuli sent from Stim-PC through earplugs. Currently there is no possibility to work with different channels, fine-tune the equalisation or record participants' voice.

Help
-------
You can always send an email to MRI Lab staff asking generic questions. In this way the whole staff will notice your request and specific staff memebers would combine their efforts to provide you an answer.
