
=====================================================================
Welcome to CS2D's documentation!
=====================================================================

- **Data-driven methods to select samples**
- **A benchmark for backdoor attack**


Check out the :doc:`usage` section for further information, including
how to :ref:`installation` the project.

.. note::

   This project is under active development.

Contents
--------

Here's a few brief examples of how easy it is to use the package:


.. code-block:: python

   from cs2d import fit,

   nwsapy.set_user_agent("Application Name", "youremail@domain.com or website")
   active_tor_warnings = nwsapy.get_active_alerts(event = "Tornado Warning")
   df = active_tor_warnings.to_dataframe()



Implementation of the full API is in progress. The documentation will update on an as-needed basis to reflect this.

The National Weather Service API can be found here: https://www.weather.gov/documentation/services-web-api#/

Table of Contents
=================
.. toctree::
   :maxdepth: 2
   
   Getting Started <gettingstarted>
   Using NWSAPy <using_nwsapy/intro>
   Data Validation Tables <dvt>


Advantages of using CS2D
==========================
- **End-to-end learning** - The CS2D provides end-to-end learning.


Dependencies
============

NWSAPy has minimal dependencies, with core functionality being pure python:

- shapely
- pandas
- numpy
- requests
- pint

Contact
=======


Important Links
===============

- `GitHub <https://github.com/WxBDM/nwsapy>`_


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
