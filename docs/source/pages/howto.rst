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
            - A new window will appear showing the installed Java version.
    - For Windows
        - Open the Java Control Panel:
            - Press Windows + S and type Control Panel, then open it.
            - In the Control Panel, search for Java using the search bar in the top-right corner.
            - Click on Java (32-bit) or Java (64-bit) to open the Java Control Panel.
        - Check the Java Version:
            - In the Java Control Panel, go to the General tab.
            - Click the About... button.
            - A dialog box will appear showing the installed Java version.
    - For Linux
        - Open the Java Control Panel:
            - Open a terminal window.
            - Type the command ``ControlPanel`` (case-sensitive) and press Enter. This will launch the Java Control Panel if it is installed.

    .. warning::
        If the :bdg-secondary:`ControlPanel` command does not work, ensure Java is properly installed and included in your system's PATH. Alternatively, use the terminal command ``java -version`` to quickly check the installed Java version.

    - Check the Java Version:
        - In the Java Control Panel, go to the General tab.
        - Click the About... button.
        - A dialog box will appear displaying the installed Java version.
    
