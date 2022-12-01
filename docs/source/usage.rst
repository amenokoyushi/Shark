Usage
=====

.. _quick start:

Quick Start
------------

The quickest start is to use an exe file builded for windows with mainly ``python3.11``, ``streamlit1.14.0`` and ``pyinstaller``.
Creating a shortcut of the exe in ```../dist/OSCE_timer/OSCE_timer.exe``` may help us to find the exe in a shorter time. 

To start the app, just click the short cut.


Calibration
------------
Please notify the timer should be calibrated before real run.
The method of calibration is shown below.

Turn the ```Debug Mode``` to ```on```.
Turn the ```Settings``` to ```calibration```.
Setting other necessary parameters.
Click ```Set```.
Click ```Start```



To use Lumache, first install it using pip:

.. code-block:: console

   (.venv) $ pip install lumache

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

