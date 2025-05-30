How To ...
============

.. dropdown:: StimDev-PC Booking

    Open the "Book your appointment" link on `Best Practices <https://cimec-mrilab-wiki.readthedocs.io/en/latest/pages/bestpractices.html#code-testing>`_ page of the Wiki.
        
    It opens this page where you have to select the slot(s) that you want to book:
    
    .. image:: figures/selectDateandHour.png
      :width: 800
      :alt: SlotSelection

    |
    | After you have selected the slot there will be a Pop-up where you need to insert your Name, Surname and Institutional Email:
    
    .. warning::
      If the slot is booked without an Institutional Email, the reservation will be canceled.
    
    .. image:: figures/insertDatas.png
      :width: 800
      :alt: DataInsertion

    |
    | Press the :bdg-primary:`Book/Prenota` button to confirm the booking, there will be a confirmation message in the same Pop-up:
    
    .. image:: figures/confirmation.png
      :width: 800
      :alt: BookingConfirmation

    |
    | Check if you have the event on your calendar:
    
    .. image:: figures/slot.png
      :width: 800
      :alt: ConfirmedSlot


.. dropdown:: Configuration of Mozilla Firefox for CDRMS
    
    Once you have Mozilla Firefox installed, you need to allow TLS protocol 1.0 by typing ``about:config`` in the address bar and press Enter.

    .. image:: figures/aboutconfig.png
        :width: 800
        :alt: about:config

    |
    | Type ``tls`` in the seach box, from here set :bdg-primary:`security.tls.version.min` option to :bdg-primary-line:`1` and set :bdg-primary:`security.tls.version.enable-deprecated` option to :bdg-primary-line:`true`.

    .. image:: figures/securitytls.png
        :width: 800
        :alt: tlsConfig


.. dropdown:: Configuration of Java for CDRMS

    Once you have Java SE Runtime Environment instaled, you will need to check if you have installed the correct version of it.

    - For macOS:
        - Open the Java Control Panel:
            - Go to System Settings from the Apple menu.
            - Locate and click on the Java icon to open the Java Control Panel.
        - Check the Java Version:
            - In the Java Control Panel, go to the General tab.
            - Click the About... button.
            

             .. image:: figures/Javaversion1.png
                :width: 800
                :alt: JavaControlPanel

            
            - A new window will appear showing the installed Java version.
            

             .. image:: figures/Javaversion3.png
                :width: 800
                :alt: JavaVersion
            
    - For Windows
        - Open the Java Control Panel:
            - Press Windows key to open the search box.

             .. image:: figures/JavaVersion_win1.png
                :width: 800
                :alt: JavaVersion_Win1

            - Type ``About Java``, then click it. If it does not come up, try ``Configure Java``. If you’re still having no luck, you probably don’t have Java installed.

             .. image:: figures/JavaVersion_win2.png
                :width: 800
                :alt: JavaVersion_Win2

            - Once you click through on About Java or Configure Java, you’ll see a pop-up window indicating the current version and build number.

             .. image:: figures/JavaVersion_win3.png
                :width: 800
                :alt: JavaVersion_Win3

    - For Linux
        - Open the Java Control Panel:
            - Open a terminal window.
            - Type the command ``ControlPanel`` (case-sensitive) and press Enter. This will launch the Java Control Panel if it is installed.

        - Check the Java Version:
            - In the Java Control Panel, go to the General tab.
            - Click the About... button.
            - A dialog box will appear displaying the installed Java version.
     .. warning::
        If the :bdg-secondary:`ControlPanel` command does not work, ensure Java is properly installed and included in your system's PATH. Alternatively, use the terminal command ``java -version`` to quickly check the installed Java version.


    - To Solve Java Security issue:
        - Go to the ``Security`` tab of the Java Control Panel and click on the ``Edit Site List`` button

             .. image:: figures/JavaSecurity1.png
                :width: 800
                :alt: JavaSecurity1
        
        - A new window will appear where you have to click on the ``Add`` button

             .. image:: figures/Javasecurity2.png
                :width: 800
                :alt: JavaSecurity2

        - Type ``https://dicom.cimec.unitn.it`` in the row that will compare after you have clicked the ``Add`` button and press Enter (Red Arrow in the image below). Then click the ``OK`` button.

             .. image:: figures/Javasecurity3.png
                :width: 800
                :alt: JavaSecurity3

        - Verify that this procedure was successfull by checkling if the URL is present in the ``Exception Site List`` (Red Arrow in the image below). If you do not see the URL written there, repeat the previous passages until this passage is correct. Click the ``OK`` button to confirm the procedure.

             .. image:: figures/Javasecurity4.png
                :width: 800
                :alt: JavaSecurity4


Help
-------

 * See `FAQs <https://cimec-mrilab-wiki.readthedocs.io/en/latest/pages/FAQ.html>`_ page.

 * If the topic you need assistance with is not covered in the FAQ section of the Wiki, you can refer to the `Discussion Board <https://github.com/orgs/LNIFMRI-Lab/discussions>`_ (`Link to Discussion Board Registration Form <https://forms.gle/s7nn7CRL5LL1yviq7>`_) for further support.

 * If the topic you need assistance with is not covered in the FAQ section of the Wiki or the discussion board, you can send an `email <https://arc.net/l/quote/ngemhopk>`_ to the MRI Lab for further support.
