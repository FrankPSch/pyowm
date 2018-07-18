.. pyowm documentation master file, created by
   sphinx-quickstart on Thu Aug 25 12:34:05 2016.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

PyOWM
=====

Welcome to PyOWM's documentation!

What is PyOWM?
--------------

PyOWM is a client Python wrapper library for OpenWeatherMap web APIs. It allows quick and easy
consumption of OWM data from Python applications via a simple object model and in a human-friendly fashion.


What APIs does PyOWM allow me to use?
-------------------------------------

With PyOWM you can interact programmatically with the following OpenWeatherMap web APIs:

 - **Weather API v2.5**, offering
    + current weather data
    + weather forecasts
 - **Air Pollution API v3.0**, offering data about CO, O3, NO2 and SO2
 - **UV Index API v3.0**, offering data about Ultraviolet exposition
 - **Stations API v3.0**, allowing to create and manage meteostation and publish local weather measurements
 - **Weather Alerts API v3.0**, allowing to set triggers on weather conditions and areas and poll for spawned alerts


and more will be supported in the future. Stay tuned!

The documentation of OWM APIs can be found on the OWM Website_

.. _Website: https://openweathermap.org/api


Supported environments and Python versions
------------------------------------------

PyOWM runs on Windows, Linux and MacOS.

PyOWM runs on:

  - Python 2.7
  - Python 3.4+

Please notice that **support for Python 2.x will eventually be dropped** - check details_

.. _details: https://github.com/csparpa/pyowm/wiki/Timeline-for-dropping-Python-2.x-support


PyOWM also integrates with Django_ 1.10+ models, but that integration might have issues (contributions are welcome)

.. _Django: https://github.com/csparpa/pyowm/wiki/Django-support


Installation
------------

pip
~~~

The easiest method of all:

.. code::

    $ pip install pyowm

Get the lastest development version
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You can install the development trunk with _pip_:

.. code::

    $ pip install git+https://github.com/csparpa/pyowm.git@develop


but be aware that it might not be stable!

setuptools
~~~~~~~~~~

You can install from source using _setuptools_: either download a release from GitHub or just take the latest main branch), then:

.. code::

   $ unzip <zip archive>   # or tar -xzf <tar.gz archive>
   $ cd pyowm-x.y.z
   $ python setup.py install

The .egg will be installed into the system-dependent Python libraries folder:

.. code::

   C:\PythonXY\Lib\site-packages            # Windows
   /usr/local/lib/pythonX.Y/dist-packages   # Ubuntu
   /usr/local/lib/pythonX.Y/dist-packages   # MacOS 10.5.4


Distribution packages
~~~~~~~~~~~~~~~~~~~~~

  - On Windows you have installers
  - On ArchLinux you can install PyOWM with the Yaourt package manager, run:

      .. code::

         Yaourt -S python2-owm  # Python 2.7 (https://aur.archlinux.org/packages/python-owm)
         Yaourt -S python-owm   # Python 3.x (https://aur.archlinux.org/packages/python2-owm)



Examples and Guides
-------------------

Here are some usage examples for the different OWM APIs


Weather API examples
~~~~~~~~~~~~~~~~~~~~
.. toctree::
   :maxdepth: 1

   object-model
   usage-examples


UV API examples
~~~~~~~~~~~~~~~
.. toctree::
   :maxdepth: 1

   uv-api-usage-examples


Air Pollution API examples
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. toctree::
   :maxdepth: 1

   air-pollution-api-usage-examples

Stations API examples
~~~~~~~~~~~~~~~~~~~~~
.. toctree::
   :maxdepth: 1

   stations-api-usage-examples

Alerts API examples
~~~~~~~~~~~~~~~~~~~
.. toctree::
   :maxdepth: 1

   alerts-api-usage-examples



PyOWM software API documentation
--------------------------------

This is the Python API documentation of PyOWM:

.. toctree::
   :maxdepth: 1

   pyowm


Indices and tables
------------------

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

