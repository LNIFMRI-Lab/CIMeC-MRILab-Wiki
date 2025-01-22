MR Data Retrieving System (CDRMS)
===============

Introduction
------------

The purpose of the data retrieving system (CDMRS) is to provide a repository of raw MR Data (and compounds) that users can download. Furthermore, the system allows searching and sharing between projects existing structural MRI data (e.g. for MEG and TMS experiments). You can reach the data retrieving system at `this link <https://dicom.cimec.unitn.it/CDRMS-WEB>`_.

The application allows you browsing and downloading, down to the single sequence level, all MR data acquired within your CIMeC approved projects that involves MR Scans. Detailed information about volunteer, projects, exams and sequences are available, together with a preview of the single raw images. During a download session you can choose among a couple of DICOM sorting options. A text file (scan_list.txt) with a summary of exam/sequences information will be saved on your disk for each exam. A text file containing detailed sequence information will be saved within each sequence (text_header.txt). The system also manages physiological data acquired during scans, provided that, before starting the exam, you requested MRI Staff to register and upload them.
The retrieving system also manages data sharing between projects: if your project needs structural data of a volunteer that already partecipated in some experiments at MRI lab, you can search the database for his/her anatomical MRI sequences (if they has been made shareable by the correspondent PI). If you are a PI of a project that produces MRI Structural Data you can manage your shares. A form useful for contacting automatically by email all volunteers with available anatomical data is also available.
Please remember that data sharing is possible only between CIMeC projects approved by Research Ethical Committee.

Any suggestion,feedback, request, criticism etc ... is welcome and will be discussed by the IT offi ce together with the head of the LNIF-MRI lab.

Requirements
-------------

In order to use CDRMS the following requirements are mandatory:

  - Working within the UniTN Network (a VPN connection is required of working remotely);
  - Being member of a CIMeC approved project that involves MRI Scanning;
  - Having UniTN credentials with a password not older than 3 months, this constraint follow on from UniTN Data Protection Policy;
  - Using only Mozilla Firefox Web Browser, allowing TLS protocol 1.0 typing 'about:config' in the address bar, 'tls' in the seach box and set '1' the 'security.tls.version.min' option and set 'true' at 'security.tls.version.enable-deprecated' option. (for a in depth guide, see the `How to ... page <link>`_).
  - Having Java Runtime version less than 8u291 installed on your computer (`download 8u231 <>`_).

How to retrieve data
-------------

Once logged into CDRMS you can easily browse and select your data for retrieving, selecting a sorting order for your DICOM files or accepting the default one. Hereafter a brief step-by-step guide for the download process (see `How to ... <link>`_ to consult a short graphical guide).

  -  Marking objects for retrieving:
      at first a list of all the exams acquired within the last month is presented; you can choose another month by using the selectors placed on the center of the bottom bar. You can browse objects, directly download physiological data and mark DICOM data for retrieving by clicking on the small download icon at the right of each displayed item (accession, exam or sequence). Once your selection is complete, you can customize the sorting options, by pressing Customize download on the right of the bottom bar, or accept the default sorting pressing Download.
  - Previewing/customizing DICOM sorting:
      a preview of the way data will be organized on your disk is presented; if you choose to customize sorting options on the left you will find also a couple of sorting options. When you're ready for starting the download session press Download on the right of the bottom bar.
  - Download session:
      after you press download Java will start on your computer, connecting you directly with the PACS archive where images are stored. The first time you start a download session you have to confirm a security exception by choosing Always trust content from this publisher and pressing Yes. The CDRMS Download Manager, will start. Choose the directory in which you want to save your data and press Start download. The application will download all the selected data in the directory you specify.
  -  Solving Java security issue:
      sometimes Java updates changes automatically some security settings that prevents you to start the Download Manager application. To solve them open the Java Control Panel, navigate to the Security tab security, lower the Security level to the minimum available and add 'https://dicom.cimec.unitn.it' to the Exception site list (see`How to ... <link>`_ to consult a short graphical guide).

How to obtain MRI Structural Data from another project
-------------

If you are member of a project, approved by our ethical commitee, that needs a structural scan of a volunteer that already partecipated to an MRI experiment at LNIF, follow these steps (see also this step-by-step graphical guide):

  - Log into the retrieving system and open the Search MR sequences page.
  - At this point we assume you have already contacted the volunteer. If not, you can use the Contact subjects by e-mail form: this will send an e-mail to all volunteers for whom structural data are available. Please, use this feature with caution! Any abuse will be monitored.
  - Make sure that the volunteer give his/her consent to sharing data. This can be done by asking the participant to sign a form in which he/she allows a particular PI to release his/her structural scan available for your project; here the english and the italian forms. Please consider that it is your responsibility to archive the subject consent in a way that is compliant with the UniTN personal data protection code.
  - Now fill the Search for anatomical shareable sequences form, asking the volunteer for the necessary information. The system will provide a list of exams that have a structural scan of your volunteer.
  - Choose an exam and contact the respective PI, providing him the code of your project and an hard copy of the signed subjects consent.
  - Once the PI you contacted shares the scan to your project, you can browse/download the shared structural scan from within your project data as usual; shared data will be shown in italics font.

How to share MRI Data to another project
-------------

If you are a PI of a project, approved by our ethical commitee, producing MRI structural data and you want your data to be shareable (i.e. allow people search/ask for your data) please contact the head of the LNIF-MRI lab or the IT Office (preferably Davide Tabarelli). If you already did that and now you just want to share structural sequences to another project, follow these steps (see also this step-by-step graphical guide):

  - At this point we assume that:
      - the requesting PI provided/shown you a copy of the volunteer consent (you must take care controlling the volunteer gave consent).
      - the requesting PI provided you the code of the project data has to be shared to.
  - Log in to the retrieving system and navigate data down to the sequence you want to share.
  - Open the sharing frame by clicking on the sharing icon on the right of the sequence.
  - Select from the list the project code; now data has been shared.
  - If you want to remove a share, open the sharing frame as above and click on the trash icon on the left of the project list. Consider that this will only remove the share within the retrieving system; all data already downloaded by the requesting PI are not managed.
