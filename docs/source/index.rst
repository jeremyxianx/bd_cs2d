
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
   :maxdepth: 1
   
   Getting Started <gettingstarted>
   Using NWSAPy <using_nwsapy/intro>
   Data Validation Tables <dvt>

Advantages of using NWSAPy
==========================
- **Clean and Simplistic Code** - The syntax is very english-like.
- **No worries about JSON**. NWSAPy takes care of anything JSON-related, including formats (GeoJSON, JSON-LD, etc).
- **No worries about URLs**. Similar to the Django ORM, you're able to make a request without ever writing code to make a request.
- **404 Error Minimization.** This is handled through data validation checks, as well as handling URL construction.
- **Response errors are handled.** Response errors are handled appropriately.

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
- `National Weather Service API Documentation <https://www.weather.gov/documentation/services-web-api>`_
- `National Weather Service API <https://api.weather.gov/>`_
- `National Weather Service API Discussion <https://github.com/weather-gov/api/discussions>`_

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
