
=====================================================================
Welcome to CS2D's documentation!
=====================================================================

- **Data-driven methods to select samples**
- **A benchmark for backdoor attack**


Check out the :doc:`usage` section for further information, including
how to :ref:`installation` the project.

.. note::

   This project is under active development.

An example
--------

Here's a demonstrating example of how to use the package:


.. code-block:: python


   from dataset import fmnist
   from pretrained import fmn_classifier
   from model import CNN
   import torch
   
   
   cs2d_classifier = CNN()
   cs2d_classifier = torch.load(fmn_classifier)
   

   





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

CS2D has minimal dependencies, with core functionality being pure python:

- shapely
- pandas
- numpy
- requests
- pint

Contact
=======

Xun Xian at xian0044@umn.edu

Important Links
===============



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
