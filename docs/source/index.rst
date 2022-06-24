
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

Here's a few brief examples of how to use the package:


.. code-block:: python


   from dataset import fmnist
   from pretrained import fmn_classifier
   from model import CNN
   import torch
   
   
   cs2d_classifier = CNN()
   cs2d_classifier = torch.load(fmn_classifier)
   

   



Implementation of the full API is in progress. The documentation will update on an as-needed basis to reflect this.

The National Weather Service API can be found here: https://www.weather.gov/documentation/services-web-api#/

Table of Contents
=================
.. toctree::
   :maxdepth: 2
   
   api


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
