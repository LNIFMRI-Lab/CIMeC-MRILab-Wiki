How To ...
============

.. dropdown:: StimDev-PC Booking

    Open the "Book your appointment" link on `Best Practices <https://cimec-mrilab-wiki.readthedocs.io/en/latest/pages/bestpractices.html#code-testing>`_ page of the Wiki.
        
    It opens this page where you have to select the slot(s) that you want to book:
    
    .. image:: figures/selectDateandHour.png
      :width: 800
      :alt: SlotSelection
    
    After you have selected the slot there will be a Pop-up where you need to insert your Name, Surname and Institutional Email:
    
    .. warning::
      If the slot is booked without an Institutional Email, the reservation will be canceled.
    
    .. image:: figures/insertDatas.png
      :width: 800
      :alt: DataInsertion
    
    Press the "Prenota" button to confirm the booking, there will be a confirmation message in the same Pop-up:
    
    .. image:: figures/confirmation.png
      :width: 800
      :alt: BookingConfirmation
    
    Check if you have the event on your calendar:
    
    .. image:: figures/slot.png
      :width: 800
      :alt: ConfirmedSlot


.. dropdown:: Configuration of Mozilla Firefox for CDRMS
    
    Once you have Mozilla Firefox installed, you need to allow TLS protocol 1.0 by typing ``about:config`` in the address bar and press Enter.

    .. image:: figures/aboutconfig.png
        :width: 800
        :alt: about:config

    
    Type ``tls`` in the seach box, from here set :bdg-primary:`security.tls.version.min`` option to :bdg-primary-line:`1` and set :bdg-primary:`security.tls.version.enable-deprecated` option to :bdg-primary-line:`true`.

    .. image:: figures/securitytls.png
        :width: 800
        :alt: tlsConfig
