=======
phasepy
=======

.. image:: https://mybinder.org/badge_logo.svg
   :target: https://mybinder.org/v2/gh/gustavochm/phasepy/master

Introduction
------------

Phasepy is an open-source scientific Python package for calculation of
`physical properties of phases <https://en.wikipedia.org/wiki/Physical_property>`_ at
`thermodynamic equilibrium <https://en.wikipedia.org/wiki/Thermodynamic_equilibrium>`_.
Main application areas include computation of fluid phase equilibria
and interfacial properties.

Phasepy includes routines for calculation of vapor-liquid equilibrium (VLE),
liquid-liquid equilibrium (LLE) and vapor-liquid-liquid equilibrium
(VLLE). Phase equilibrium can be modelled either with *the continous
approach*, using a combination of a cubic equation of state (EoS,
e.g. Van der Waals, Peng-Robinson, Redlich-Kwong, or their
derivatives) model and a mixing rule (Quadratic, Modified Huron-Vidal
or Wong-Sandler) for all phases, or *the discontinuous approach* using
a virial equation for the vapor phase and an activity coefficient model
(NRTL, Wilson, Redlich-Kister, UNIQUAC or Dortmund Modified UNIFAC) for the
liquid phase(s).

Interfacial property estimation using the continuous phase equilibrium
approach allows calculation of density profiles and interfacial
tension using the Square Gradient Theory (SGT).

Phasepy supports fitting of model parameter values from experimental data.

Installation Prerequisites
--------------------------
- numpy
- scipy
- pandas
- openpyxl
- C/C++ Compiler for Cython extension modules

Installation
------------
     $ sudo apt-get update
     $ sudo apt install build-essential
     $ sudo apt install gcc
     $ sudo apt install gcc-multilib
     $ sudo apt install g++
     $ sudo apt install g++-multilib
     
Get the latest version of phasepy from
https://pypi.python.org/pypi/phasepy/

An easy installation option is to use Python pip:

    $ pip install phasepy

Alternatively, you can build phasepy yourself using latest source
files:

    $ git clone https://github.com/gustavochm/phasepy


Documentation
-------------

Phasepy's documentation is available on the web:

    https://phasepy.readthedocs.io/en/latest/


Getting Started
---------------

Base input variables include temperature [K], pressure [bar] and molar
volume [cm^3/mol]. Specification of a mixture starts with

Bug reports
-----------

To report bugs, please use the phasepy's Bug Tracker at:

    https://github.com/gustavochm/phasepy/issues


License information
-------------------

See ``LICENSE.txt`` for information on the terms & conditions for usage
of this software, and a DISCLAIMER OF ALL WARRANTIES.

Although not required by the phasepy license, if it is convenient for you,
please cite phasepy if used in your work. Please also consider contributing
any changes you make back, and benefit the community.


Chaparro, G., Mejía, A. Phasepy: A Python based framework for fluid phase
equilibria and interfacial properties computation. J Comput Chem. 2020, 41, 29,
2504-2526. `https://doi.org/10.1002/jcc.26405 <https://doi.org/10.1002/jcc.26405>`_.
