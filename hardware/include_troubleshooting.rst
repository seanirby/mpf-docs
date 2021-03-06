Add debugging to related devices
--------------------------------

If you got problems with some switches also add ``debug: true`` to those as
it will give to more insights into the intentions of those devices.
Same will work for flippers, coils, lights, servos, steppers and more.
See :doc:`general debugging section </troubleshooting/general_debugging>`
for details.

Reducing light update rate
--------------------------

If you got a lot of lights you might run into bus contention issues.
You can reduce the light update rate in MPF:

.. code-block:: mpf-config

    mpf:
      default_light_hw_update_hz: 30   # defaults to 50

If you set this too low fades will be less smooth but otherwise it should not
affect your game.

Run MPF with verbose flag
-------------------------

See :doc:`general debugging section </troubleshooting/general_debugging>` for
details.
TLDR: run ``mpf both -t -v -V``.


Report Your Issue and Ask For Help
----------------------------------

If you cannot find the issue yourself please prepare some information about
your issue according to our
:doc:`troubleshooting guide </troubleshooting/index>` and ask in our forum.

Consider Improving the Documentation
------------------------------------

Did you solve your issue but found that some relevant information in the
documentation is missing or should be linked/located elsewhere?
Either tell us in the forum or consider
:doc:`improving the documentation </about/contributing_to_mpf_docs>`
yourself to save future users some troubles the same way others saved you
some troubles by writing this documentation.
