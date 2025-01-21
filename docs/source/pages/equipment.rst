Equipment
==========
*to be implemented*

MRI Scanner
--------

`Siemens Prisma 3T <https://www.siemens-healthineers.com/magnetic-resonance-imaging/3t-mri-scanner/magnetom-prisma>`_:
  * actively shielded;
  * whole body 3T magnet;
  * bore diameter: 60cm;
  * 80mT/m gradients with a slew rate of 200 T/m/s;
  * 20ch and 64ch Head/Neck RF Coil for experimental neuroimaging applications.

Peripheral Equipment
----------
  * 40" LCD monitor for visual stimuli from `Nordic NeuroLab <https://www.nordicneurolab.com/products/inroomviewing-device>`_ (NNL), always inside the MRI Room (see `Visual Presentation <https://cimec-mrilab-wiki.readthedocs.io/en/latest/pages/equipment.html#id2>`_ section in this page);
  * 2 x 4 Button Response Pads (`Current Designs <https://www.curdes.com/mainforp/responsedevices/hhsc-2x4-l.html>`_);
  * Button Response Pads Interface (`Current Designs <https://www.curdes.com/mainforp/interfaces/fiu-932b.html>`_);
  * Earplugs from `Sensimetric <https://www.sens.com/products/earphones-for-fmri-research/>`_ connected to the Stim-PC via `Pyle USA PCA1 Amplifier <https://pyleusa.com/products/pca1>`_
  * MR compatible glass frames for adult and pediatric subjects, max visual correction from -6 to +6 with intervals of 0.5 (`Cambridge Research System <https://www.crsltd.com/mri-patient-comfort-communication-and-entertainment/mri-patient-comfort/mediglasses/mediglasses-for-fmri/>`_);
  * Tactile Piezoelectric Stimulator, 2 x 5 fingers (`QuaeroSys <https://www.quaerosys.com/index.php?lang=en&page=piezostimulator>`_);
  * Eye Tracker (`Eyelink <https://www.sr-research.com/fmri-meg-systems/>`_);
  * Physiological data monitoring and recording (ECG, pOx, Resp tracking);

.. warning::
 It is possible to use additional peripheral devices provided by the Researchers; however, these must be approved by the Magnetic Resonance Safety Officer (MRSO) and the MRI Staff. The devices must meet the requirements for Electromagnetic Compatibility and Safety to ensure their suitability for use in Zone 4.

Stimulation PCs
---------

MRI Lab provides the researchers with:
  * a Stimulation PC (Stim-PC from now on) located in the control room, connected to the Peripheral Equipment within the MRI Room and equipped with a stimulation software. The Stim-PC can receive triggers from the scanner and responses from the NNL ButtonBox systems;

  * a Stimulation Development PC (StimDev-PC from now on), clone of the Stim-PC, can be found in the MRI Area and used to test paradigms and to train subjects outside the MR Scanner.

.. note::
  * Stim-PC stays offline. Researchers should come with a USB Drive with their files;
  * Stim-PC is not updated on researchers requests. Current software equipment was judged as stable and powerful enough for most of the experiments, specific requests could be evaluated and implemented by `MR Lab Staff <https://cimec-mrilab-wiki.readthedocs.io/en/latest/pages/contacts.html>`_;
  * StimDev-PC is online, and the researcher can access it using their UniTN account;
  * StimDev-PC use requires a booking through `this link <https://calendar.google.com/calendar/u/0/appointments/schedules/AcZssZ3ncrIjmsWNRckJOE-qsOklLg7HLzWjrCwNrVpKXB8smYFSV6onrzHU7mS22sJCPAh2CY3Rweya>`_

Hardware Specs
~~~~~~~~~~
  * CPU: `Intel Core i7-13700 <https://www.intel.com/content/www/us/en/products/sku/230490/intel-core-i713700-processor-30m-cache-up-to-5-20-ghz/specifications.html>`_, up to 5.2 Ghz, 16 Cores
  * GPU: `NVIDIA GeForce RTX 4060 <https://www.nvidia.com/en-gb/geforce/graphics-cards/40-series/rtx-4060-4060ti/>`_
  * RAM: 2x16Gb 4400Mhz

The Stim-PC is connected to the NNL Monitor, used to present visual stimuli. Images can be seen by the subject through a mirror put on the Head/Neck Coil.

Software Specs
~~~~~~~~~~

Here you can find the list of installed software:
 * Audacity 3.4.2
 * E-Prime 3.0 Subject Station 3.0.3.214
 * EyeLink Developer's Kit 2.1.762.0
 * MATLAB R2017b
 * MATLAB R2022b
 * PsychToolBox 3.0.19
 * Tachyon
 * Anaconda 2024.06-1 with Python 3.12.4
 * PsychoPy 2024.2.2

Instructions for users
~~~~~~~~~~
  * Access to Stim-PC: the password is printed on LCD monitor in the control room. You must log in locally, the PC has not Internet connection;
  * Connection: use a portable device (most likely an USB Drive) to copy your script in the designed folder on the Stim-PC.

Updates and Development
------
The descripted hardware and software equipment is the standard configuration of the Stim-PC. Updates made by MR Lab will be announced in advance and described to the users.

Potential specific configurations should be requested by sending an email to MRI Lab staff.

The staff will discuss if and how implement requested changes in the lab environment.

Button Response Pads Interface
------
Signals coming from Scanner Room are managed by the Button Response Pads Interface (aka Trigger/Button Box), which is connected to the Button Response Pads through a optic fiber cable and to the scanner through a BNC cable.

Trigger/Button Box is in turn connected to the Stim-PC through USB. Stim-PC collect signal from the scanner room as if it was an external USB keyboard.

This means that whenever a signal is sent from within scanner room, numbers appear on the Stim-PC. Keep this in mind when you need to collect responses within your MATLAB code.

Scanner Sync
--------
The scanner, during functional acquisitions, sends a 50μs "pulse" every TR, marking in this way the "volumes" of your MRI experiment.

Synchronization with the scanner trigger is provided through a BNC cable connected to the Trigger/Button Box, attached to Stim-PC via a USB Port.

Stim-PC collect triggers as if someone was systematically pressing ``5`` key (the one located in the alphanumeric part of the keyboard) at the beginning of each volume acquisition.

This means that in debugging, you can test your scripts by simply accepting ``5`` key.

Participants' responses
----------
MRI Lab provides two 4-button boxes for the participant to send responses while performing inside the scanner.

Buttons are arranged in a linear way. They are marked as right and left through a duct tape. They send, respectively, ``1`` ``2`` ``3`` ``4`` and ``6`` ``7`` ``8`` ``9`` keys to Stim-PC.

You can check the responses by focusing on the Trigger/Button Box during the experiments. Specific green leds light up when a button is pressed.

Visual Presentation
---------
For the visual stimuli presentation, MRI Lab provides a compatible NNL LCD monitor positioned at the back of the Magnet Bore.

Basic monitor specs include:
 * 40" (878 mm horizontal x 485 mm vertical);
 * 3840 x 2160 pixels;
 * surface luminance 350 c/m2;
 * contrast ratio 5000:1 typ;
 * refresh rate: 60Hz @ 2160p, 120Hz @ 1080p.

For more specs, see `Nordic NeuroLab <https://www.nordicneurolab.com/products/inroomviewing-device>`_.

Note that the distance from participants eyes and the mirror on the coil can vary between 15 and 20cm.

Auditory Presentation
----------
The current setup includes high-quality auditory capabilities. Participants can hear stereo auditory stimuli delivered via Sensimetrics earplugs connected to the Stim-PC through an amplifier, ensuring high-quality audio presentation.

To ensure optimal audio stimuli, they must be created with a frequency of 48 kHz and equalized by following `this guide <https://www.sens.com/products/model-s14/#downloads>`_ using EQ_Filtering 4.0.

For more specs, see `Sensimetric <https://www.sens.com/products/earphones-for-fmri-research/>`_ and `Pyle USA PCA1 Amplifier <https://pyleusa.com/products/pca1>`_.

Peripherals Scheme
--------------
Here you can find a schematic representation of how the peripheral equipment is connected to the MR scanner and the Stim-PC:

.. image:: figures/LNIFMRI_SetupScannerAndPeripherals.png
  :width: 800

Help
-------

 * See `FAQs <https://cimec-mrilab-wiki.readthedocs.io/en/latest/pages/FAQ.html>`_ page.

 * If the topic you need assistance with is not covered in the FAQ section of the Wiki, you can refer to the `Discussion Board <https://github.com/orgs/LNIFMRI-Lab/discussions>`_ (`Link to Discussion Board Registration Form <https://forms.gle/s7nn7CRL5LL1yviq7>`_) for further support.

If the topic you need assistance with is not covered in the FAQ section of the Wiki or the discussion board, you can send an `email <https://arc.net/l/quote/ngemhopk>`_ to the MRI Lab for further support.
