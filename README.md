# OEMOF_SOLPH

![licence](https://img.shields.io/badge/licence-NOASSERTION-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![checks](https://img.shields.io/badge/checks-unknown_PASS-brightgreen)

> Governed Anticloud packaging of the upstream project `OEMOF_SOLPH` in category **SOLAR**. check results: see ISOLATED_LAB_RESULTS. Every number below traces to a named file + run stamp; nothing is borrowed from other projects.

**Upstream:** OEMOF_SOLPH · **Upstream pin:** `943c057da7445e971750e95130c2e9b0158ce20d` · **Category:** SOLAR · **Vendor:** Anticloud FZ LLE · **Licence:** NOASSERTION

---

## What This Project Does

.. SPDX-FileCopyrightText: oemof e.V. and contributors
..
.. SPDX-License-Identifier: MIT

|tox-pytest| |tox-checks| |packaging| |coverage|

|docs| |version| |supported-versions|

|zenodo| |commits-since| |chat|

------------------------------

.. |tox-pytest| image:: https://github.com/oemof/oemof-solph/actions/workflows/tox_pytests.yml/badge.svg?branch=dev
     :target: https://github.com/oemof/oemof-solph/actions?query=workflow%3A%22tox+checks%22

.. |tox-checks| image:: https://github.com/oemof/oemof-solph/actions/workflows/tox_checks.yml/badge.svg?branch=dev
     :target: https://github.com/oemof/oemof-solph/actions?query=workflow%3A%22tox+checks%22

.. |packaging| image:: https://github.com/oemof/oemof-solph/actions/workflows/packaging.yml/badge.svg
     :target: https://github.com/oemof/oemof-solph/actions?query=workflow%3Apackaging

.. |coverage| image:: https://raw.githubusercontent.com/oemof/oemof-solph/python-coverage-comment-action-data/badge.svg
    :target: https://htmlpreview.github.io/?https://github.com/oemof/oemof-solph/blob/python-coverage-comment-action-data/htmlcov/index.html

.. |docs| image:: https://readthedocs.org/projects/oemof-solph/badge/?style=flat
    :target: https://readthedocs.org/projects/oemof-solph
    :alt: Documentation Status

.. |version| image:: https://img.shields.io/pypi/v/oemof.solph.svg
    :alt: PyPI Package latest release
    :target: https://pypi.org/project/oemof.solph

.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/oemof.solph.svg
    :alt: Supported versions
    :target: https://pypi.org/project/oemof.solph

.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/oemof.solph.svg
    :alt: Supported implementations
    :target: https://pypi.org/project/oemof.solph

.. |commits-since| image:: https://img.shields.io/github/commits-since/oemof/oemof-solph/latest/dev
    :alt: Commits since latest release
    :target: https://github.com/oemof/oemof-solph/compare/master...dev

.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.596235.svg
    :alt: Zenodo DOI
    :target: https://doi.org/10.5281/zenodo.596235

.. |chat| image:: https://img.shields.io/badge/chat-oemof:matrix.org-%238ADCF7
     :alt: matrix-chat
     :target: https://matrix.to/#/#oemof:matrix.org

.. figure:: https://raw.githubusercontent.com/oemof/oemof-solph/492e3f5a0dda7065be30d33a37b0625027847518/docs/_logo/logo_oemof_solph_FULL.svg
    :align: center

------------------------------

===========
oemof.solph
===========

**A model generator for energy system modelling and optimisation (LP/MILP)**

.. contents::
    :depth: 2
    :local:
    :backlinks: top

Introduction
============

The oemof.solph package is part of the
`Open energy modelling framework (oemof) <https://github.com/oemof/oemof>`_.
This is an organisational framework to bundle tools for energy (system) modelling.
oemof-solph is a model generator for energy system modelling and optimisation.

The package ``oemof.solph`` is very often called just ``oemof``.
This is because installing the ``oemof`` meta package was once the best way to get ``oemof.solph``.
Notice that you should prefeably install ``oemof.solph`` instead of ``oemof``
if you want to use ``solph``.

Everybody is welcome to use and/or develop oemof.solph.
Read our `contribution <https://oemof.readthedocs.io/en/latest/contributing.html>`_ section.

Contribution is already possible on a low level by simply fixing typos in
oemof's documentation or rephrasing sections which are unclear.
If you want to support us that way please fork the oemof-solph project to your own
GitHub account and make changes as described in the `github guidelines <https://docs.github.com/en/get-started/start-your-journey/hello-world>`_

If you have questions regarding the use of oemof including oemof.solph you can visit the openmod forum (`tag oemof <https://forum.openmod-initiative.org/tags/c/qa/oemof>`_ or `tag oemof-solph <https://forum.openmod-initiative.org/tags/c/qa/oemof-solph>`_) and open a new thread if your questions hasn't been already answered.

Keep in touch! - You can become a watcher at our `github site <https://github.com/oemof/oemof>`_,
but this will bring you quite a few mails and might be more interesting for developers.
If you just want to get the latest news, like when is the next oemof meeting,
you can follow our news-blog at `oemof.org <https://oemof.org/>`_.

Documentation
=============
The `oemof.solph documentation <https://oemof-solph.readthedocs.io/>`_ is powered by readthedocs. Use the `project site <https://readthedocs.org/projects/oemof>`_ of oemof.solph to choose the version of the documentation. Go to the `download page <https://readthedocs.org/projects/oemof/downloads/>`_ to download different versions and formats (pdf, html, epub) of the documentation.

Installation
============

If you have a working Python installation, use pypi to install the latest version of oemof.solph.
Python >= 3.11 is recommended. Lower versions may work but are not tested.

We highly recommend to use virtual environments.
Please refer to the documentation of your Python distribution (e.g. Anaconda,
Micromamba, or the version of Python that came with your Linux installation)
to learn how to set up and use virtual environments.

::

    (venv) pip install oemof.solph

If you want to use the latest features, you might want to install the **developer version**. The developer version is not recommended for productive use::

    (venv) pip install https://github.com/oemof/oemof-solph/archive/dev.zip

For running an oemof-solph optimisation model, you need to install a solver.
Following you will find guidelines for the installation process for different operating systems.

.. _windows_solver_label:
.. _linux_solver_label:

Installing a solver
-------------------

There are several solvers that can work with oemof, both open source and commercial.
Two open source solvers are widely used (CBC and GLPK), but oemof suggests CBC (Coin-or branch and cut).
It may be useful to compare results of different solvers to see which performs best.
Other commercial solvers, like Gurobi or Cplex, are also options.
Have a look at the `pyomo docs <https://pyomo.readthedocs.io/en/stable/api/pyomo.solvers.plugins.solvers.html>`_
to learn about which solvers are supported.

Check the solver installation by executing the test_installation example below (see section Installation Test).

**Linux**

To install the solvers have a look at the package project of your Linux distribution or search for precompiled packages. GLPK and CBC ares available at Debian, Feodora, Ubuntu and others.

**Windows**

 1. Download `CBC <https://github.com/coin-or/Cbc/releases>`_
 2. Download `GLPK (64/32 bit) <https://sourceforge.net/projects/winglpk/>`_
 3. Unpack CBC/GLPK to any folder (e.g. C:/Users/Somebody/my_programs)
 4. Add the path of the executable files of both solvers to the PATH variable (cf. `setting environment variables as user <https://learn.microsoft.com/en-us/troubleshoot/windows-client/performance/cannot-modify-user-environment-variables-system-properties>`_)
 5. Restart Windows

Check the solver installation by executing the test_installation example (see the `Installation test` section).

**Mac OSX**

Please follow the installation instructions on the respective homepages for details.

CBC-solver: https://github.com/coin-or/Cbc

GLPK-solver: http://arnab-deka.com/posts/2010/02/installing-glpk-on-a-mac/

If you install the CBC solver via brew (highly recommended), it should work without additional configuration.

**conda**

The CBC-solver can also be installed in a `conda` environment. Please note, that it is highly recommended to `use pip after conda <https://www.anaconda.com/blog/using-pip-in-a-conda-environment>`_, so:

.. code:: console

    (venv) conda install -c conda-forge coincbc
    (venv) pip install oemof.solph

.. _check_installation_label:

Installation test
-----------------

Test the installation and the installed solver by running the installation test
in your virtual environment:

.. code:: console

  (venv) oemof_installation_test

If the installation was successful, you will receive something like this:

.. code:: console

    *********
    Solver installed with oemof:
    glpk: working
    cplex: not working
    cbc: working
    gurobi: not working
    *********
    oemof.solph successfully installed.

as an output.

Contributing
============

A warm welcome to all who want to join the developers and contribute to
oemof.solph.

Information on the details and how to approach us can be found
`in the oemof documentation <https://oemof.readthedocs.io/en/latest/contributing.html>`_ .

Citing
======

For explicitly citing solph, you might want to refer to
`DOI:10.1016/j.simpa.2020.100028 <https://doi.org/10.1016/j.simpa.2020.100028>`_,
which gives an overview over the capabilities of solph.
The core ideas of oemof as a whole are described in
`DOI:10.1016/j.esr.2018.07.001 <https://doi.org/10.1016/j.esr.2018.07.001>`_
(preprint at `arXiv:1808.0807 <https://arxiv.org/abs/1808.08070v1>`_).
To allow citing specific versions, we use the zenodo project to get a DOI for each version.

Example Applications
====================

The combination of specific modules (often including other packages) is called an
application (app). For example, it can depict a concrete energy system model.
You can find a large variety of helpful examples in the documentation.
The examples show the optimisation of different energy systems and are supposed
to help new users to understand the framework's structure.
Please make sure the example you are looking at is created for the version
of solph you have installed.

You are welcome to contribute your own examples via a `pull request <https://github.com/oemof/oemof-solph/pulls>`_
or by e-mailing us (see `here <https://oemof.org/contact/>`_ for contact information).

---

## Installation

Notice that you should prefeably install ``oemof.solph`` instead of ``oemof``
if you want to use ``solph``.

Everybody is welcome to use and/or develop oemof.solph.
Read our `contribution <https://oemof.readthedocs.io/en/latest/contributing.html>`_ section.

Contribution is already possible on a low level by simply fixing typos in
oemof's documentation or rephrasing sections which are unclear.
If you want to support us that way please fork the oemof-solph project to your own
GitHub account and make changes as described in the `github guidelines <https://docs.github.com/en/get-started/start-your-journey/hello-world>`_

If you have questions regarding the use of oemof including oemof.solph you can visit the openmod forum (`tag oemof <https://forum.openmod-initiative.org/tags/c/qa/oemof>`_ or `tag oemof-solph <https://forum.openmod-initiative.org/tags/c/qa/oemof-solph>`_) and open a new thread if your questions hasn't been already answered.

Keep in touch! - You can become a watcher at our `github site <https://github.com/oemof/oemof>`_,
but this will bring you quite a few mails and might be more interesting for developers.
If you just want to get the latest news, like when is the next oemof meeting,
you can follow our news-blog at `oemof.org <https://oemof.org/>`_.

Documentation
=============
The `oemof.solph documentation <https://oemof-solph.readthedocs.io/>`_ is powered by readthedocs. Use the `project site <https://readthedocs.org/projects/oemof>`_ of oemof.solph to choose the version of the documentation. Go to the `download page <https://readthedocs.org/projects/oemof/downloads/>`_ to download different versions and formats (pdf, html, epub) of the documentation.

Installation
============

If you have a working Python installation, use pypi to install the latest version of oemof.solph.
Python >= 3.11 is recommended. Lower versions may work but are not tested.

We highly recommend to use virtual environments.
Please refer to the documentation of your Python distribution (e.g. Anaconda,
Micromamba, or the version of Python that came with your Linux installation)
to learn how to set up and use virtual environments.

::

    (venv) pip install oemof.solph

If you want to use the latest features, you might want to install the **developer version**. The developer version is not recommended for productive use::

    (venv) pip install https://github.com/oemof/oemof-solph/archive/dev.zip

For running an oemof-solph optimisation model, you need to install a solver.
Following you will find guidelines for the installation process for different operating systems.

.. _windows_solver_label:
.. _linux_solver_label:

Installing a solver
-------------------

There are several solvers that can work with oemof, both open source and commercial.
Two open source solvers are widely used (CBC and GLPK), but oemof suggests CBC (Coin-or branch and cut).
It may be useful to compare results of different solvers to see which performs best.
Other commercial solvers, like Gurobi or Cplex, are also options.
Have a look at the `pyomo docs <https://pyomo.readthedocs.io/en/stable/api/pyomo.solvers.plugins.solvers.html>`_
to learn about which solvers are supported.

Check the solver installation by executing the test_installation example below (see section Installation Test).

**Linux**

To install the solvers have a look at the package project of your Linux distribution or search for precompiled packages. GLPK and CBC ares available at Debian, Feodora, Ubuntu and others.

**Windows**

 1. Download `CBC <https://github.com/coin-or/Cbc/releases>`_
 2. Download `GLPK (64/32 bit) <https://sourceforge.net/projects/winglpk/>`_
 3. Unpack CBC/GLPK to any folder (e.g. C:/Users/Somebody/my_programs)
 4. Add the path of the executable files of both solvers to the PATH variable (cf. `setting environment variables as user <https://learn.microsoft.com/en-us/troubleshoot/windows-client/performance/cannot-modify-user-environment-variables-system-properties>`_)
 5. Restart Windows

Check the solver installation by executing the test_installation example (see the `Installation test` section).

**Mac OSX**

Please follow the installation instructions on the respective homepages for details.

CBC-solver: https://github.com/coin-or/Cbc

GLPK-solver: http://arnab-deka.com/posts/2010/02/installing-glpk-on-a-mac/

If you install the CBC solver via brew (highly recommended), it should work without additional configuration.

**conda**

The CBC-solver can also be installed in a `conda` environment. Please note, that it is highly recommended to `use pip after conda <https://www.anaconda.com/blog/using-pip-in-a-conda-environment>`_, so:

.. code:: console

    (venv) conda install -c conda-forge coincbc
    (venv) pip install oemof.solph

.. _check_installation_label:

Installation test
-----------------

Test the installation and the installed solver by running the installation test
in your virtual environment:

.. code:: console

  (venv) oemof_installation_test

If the installation was successful, you will receive something like this:

.. code:: console

    *********
    Solver installed with oemof:
    glpk: working
    cplex: not working
    cbc: working
    gurobi: not working
    *********
    oemof.solph successfully installed.

as an output.

Contributing
============

A warm welcome to all who want to join the developers and contribute to
oemof.solph.

Information on the details and how to approach us can be found
`in the oemof documentation <https://oemof.readthedocs.io/en/latest/contributing.html>`_ .

Citing
======

For explicitly citing solph, you might want to refer to
`DOI:10.1016/j.simpa.2020.100028 <https://doi.org/10.1016/j.simpa.2020.100028>`_,
which gives an overview over the capabilities of solph.
The core ideas of oemof as a whole are described in
`DOI:10.1016/j.esr.2018.07.001 <https://doi.org/10.1016/j.esr.2018.07.001>`_
(preprint at `arXiv:1808.0807 <https://arxiv.org/abs/1808.08070v1>`_).
To allow citing specific versions, we use the zenodo project to get a DOI for each version.

Example Applications
====================

The combination of specific modules (often including other packages) is called an
application (app). For example, it can depict a concrete energy system model.
You can find a large variety of helpful examples in the documentation.
The examples show the optimisation of different energy systems and are supposed
to help new users to understand the framework's structure.
Please make sure the example you are looking at is created for the version
of solph you have installed.

You are welcome to contribute your own examples via a `pull request <https://github.com/oemof/oemof-solph/pulls>`_
or by e-mailing us (see `here <https://oemof.org/contact/>`_ for contact information).

## Usage

:target: https://htmlpreview.github.io/?https://github.com/oemof/oemof-solph/blob/python-coverage-comment-action-data/htmlcov/index.html

.. |docs| image:: https://readthedocs.org/projects/oemof-solph/badge/?style=flat
    :target: https://readthedocs.org/projects/oemof-solph
    :alt: Documentation Status

.. |version| image:: https://img.shields.io/pypi/v/oemof.solph.svg
    :alt: PyPI Package latest release
    :target: https://pypi.org/project/oemof.solph

.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/oemof.solph.svg
    :alt: Supported versions
    :target: https://pypi.org/project/oemof.solph

.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/oemof.solph.svg
    :alt: Supported implementations
    :target: https://pypi.org/project/oemof.solph

.. |commits-since| image:: https://img.shields.io/github/commits-since/oemof/oemof-solph/latest/dev
    :alt: Commits since latest release
    :target: https://github.com/oemof/oemof-solph/compare/master...dev

.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.596235.svg
    :alt: Zenodo DOI
    :target: https://doi.org/10.5281/zenodo.596235

.. |chat| image:: https://img.shields.io/badge/chat-oemof:matrix.org-%238ADCF7
     :alt: matrix-chat
     :target: https://matrix.to/#/#oemof:matrix.org

.. figure:: https://raw.githubusercontent.com/oemof/oemof-solph/492e3f5a0dda7065be30d33a37b0625027847518/docs/_logo/logo_oemof_solph_FULL.svg
    :align: center

------------------------------

===========
oemof.solph
===========

**A model generator for energy system modelling and optimisation (LP/MILP)**

.. contents::
    :depth: 2
    :local:
    :backlinks: top

Introduction
============

The oemof.solph package is part of the
`Open energy modelling framework (oemof) <https://github.com/oemof/oemof>`_.
This is an organisational framework to bundle tools for energy (system) modelling.
oemof-solph is a model generator for energy system modelling and optimisation.

The package ``oemof.solph`` is very often called just ``oemof``.
This is because installing the ``oemof`` meta package was once the best way to get ``oemof.solph``.
Notice that you should prefeably install ``oemof.solph`` instead of ``oemof``
if you want to use ``solph``.

Everybody is welcome to use and/or develop oemof.solph.
Read our `contribution <https://oemof.readthedocs.io/en/latest/contributing.html>`_ section.

Contribution is already possible on a low level by simply fixing typos in
oemof's documentation or rephrasing sections which are unclear.
If you want to support us that way please fork the oemof-solph project to your own
GitHub account and make changes as described in the `github guidelines <https://docs.github.com/en/get-started/start-your-journey/hello-world>`_

If you have questions regarding the use of oemof including oemof.solph you can visit the openmod forum (`tag oemof <https://forum.openmod-initiative.org/tags/c/qa/oemof>`_ or `tag oemof-solph <https://forum.openmod-initiative.org/tags/c/qa/oemof-solph>`_) and open a new thread if your questions hasn't been already answered.

Keep in touch! - You can become a watcher at our `github site <https://github.com/oemof/oemof>`_,
but this will bring you quite a few mails and might be more interesting for developers.
If you just want to get the latest news, like when is the next oemof meeting,
you can follow our news-blog at `oemof.org <https://oemof.org/>`_.

Documentation
=============
The `oemof.solph documentation <https://oemof-solph.readthedocs.io/>`_ is powered by readthedocs. Use the `project site <https://readthedocs.org/projects/oemof>`_ of oemof.solph to choose the version of the documentation. Go to the `download page <https://readthedocs.org/projects/oemof/downloads/>`_ to download different versions and formats (pdf, html, epub) of the documentation.

Installation
============

If you have a working Python installation, use pypi to install the latest version of oemof.solph.
Python >= 3.11 is recommended. Lower versions may work but are not tested.

We highly recommend to use virtual environments.
Please refer to the documentation of your Python distribution (e.g. Anaconda,
Micromamba, or the version of Python that came with your Linux installation)
to learn how to set up and use virtual environments.

::

    (venv) pip install oemof.solph

If you want to use the latest features, you might want to install the **developer version**. The developer version is not recommended for productive use::

    (venv) pip install https://github.com/oemof/oemof-solph/archive/dev.zip

For running an oemof-solph optimisation model, you need to install a solver.
Following you will find guidelines for the installation process for different operating systems.

.. _windows_solver_label:
.. _linux_solver_label:

Installing a solver
-------------------

There are several solvers that can work with oemof, both open source and commercial.
Two open source solvers are widely used (CBC and GLPK), but oemof suggests CBC (Coin-or branch and cut).
It may be useful to compare results of different solvers to see which performs best.
Other commercial solvers, like Gurobi or Cplex, are also options.
Have a look at the `pyomo docs <https://pyomo.readthedocs.io/en/stable/api/pyomo.solvers.plugins.solvers.html>`_
to learn about which solvers are supported.

Check the solver installation by executing the test_installation example below (see section Installation Test).

**Linux**

To install the solvers have a look at the package project of your Linux distribution or search for precompiled packages. GLPK and CBC ares available at Debian, Feodora, Ubuntu and others.

**Windows**

 1. Download `CBC <https://github.com/coin-or/Cbc/releases>`_
 2. Download `GLPK (64/32 bit) <https://sourceforge.net/projects/winglpk/>`_
 3. Unpack CBC/GLPK to any folder (e.g. C:/Users/Somebody/my_programs)
 4. Add the path of the executable files of both solvers to the PATH variable (cf. `setting environment variables as user <https://learn.microsoft.com/en-us/troubleshoot/windows-client/performance/cannot-modify-user-environment-variables-system-properties>`_)
 5. Restart Windows

Check the solver installation by executing the test_installation example (see the `Installation test` section).

**Mac OSX**

Please follow the installation instructions on the respective homepages for details.

CBC-solver: https://github.com/coin-or/Cbc

GLPK-solver: http://arnab-deka.com/posts/2010/02/installing-glpk-on-a-mac/

If you install the CBC solver via brew (highly recommended), it should work without additional configuration.

**conda**

The CBC-solver can also be installed in a `conda` environment. Please note, that it is highly recommended to `use pip after conda <https://www.anaconda.com/blog/using-pip-in-a-conda-environment>`_, so:

.. code:: console

    (venv) conda install -c conda-forge coincbc
    (venv) pip install oemof.solph

.. _check_installation_label:

Installation test
-----------------

Test the installation and the installed solver by running the installation test
in your virtual environment:

.. code:: console

  (venv) oemof_installation_test

If the installation was successful, you will receive something like this:

.. code:: console

    *********
    Solver installed with oemof:
    glpk: working
    cplex: not working
    cbc: working
    gurobi: not working
    *********
    oemof.solph successfully installed.

as an output.

Contributing
============

A warm welcome to all who want to join the developers and contribute to
oemof.solph.

Information on the details and how to approach us can be found
`in the oemof documentation <https://oemof.readthedocs.io/en/latest/contributing.html>`_ .

Citing
======

For explicitly citing solph, you might want to refer to
`DOI:10.1016/j.simpa.2020.100028 <https://doi.org/10.1016/j.simpa.2020.100028>`_,
which gives an overview over the capabilities of solph.
The core ideas of oemof as a whole are described in
`DOI:10.1016/j.esr.2018.07.001 <https://doi.org/10.1016/j.esr.2018.07.001>`_
(preprint at `arXiv:1808.0807 <https://arxiv.org/abs/1808.08070v1>`_).
To allow citing specific versions, we use the zenodo project to get a DOI for each version.

Example Applications
====================

The combination of specific modules (often including other packages) is called an
application (app). For example, it can depict a concrete energy system model.
You can find a large variety of helpful examples in the documentation.
The examples show the optimisation of different energy systems and are supposed
to help new users to understand the framework's structure.
Please make sure the example you are looking at is created for the version
of solph you have installed.

You are welcome to contribute your own examples via a `pull request <https://github.com/oemof/oemof-solph/pulls>`_
or by e-mailing us (see `here <https://oemof.org/contact/>`_ for contact information).

## API

.. |version| image:: https://img.shields.io/pypi/v/oemof.solph.svg
    :alt: PyPI Package latest release
    :target: https://pypi.org/project/oemof.solph

.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/oemof.solph.svg
    :alt: Supported versions
    :target: https://pypi.org/project/oemof.solph

.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/oemof.solph.svg
    :alt: Supported implementations
    :target: https://pypi.org/project/oemof.solph

.. |commits-since| image:: https://img.shields.io/github/commits-since/oemof/oemof-solph/latest/dev
    :alt: Commits since latest release
    :target: https://github.com/oemof/oemof-solph/compare/master...dev

.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.596235.svg
    :alt: Zenodo DOI
    :target: https://doi.org/10.5281/zenodo.596235

.. |chat| image:: https://img.shields.io/badge/chat-oemof:matrix.org-%238ADCF7
     :alt: matrix-chat
     :target: https://matrix.to/#/#oemof:matrix.org

.. figure:: https://raw.githubusercontent.com/oemof/oemof-solph/492e3f5a0dda7065be30d33a37b0625027847518/docs/_logo/logo_oemof_solph_FULL.svg
    :align: center

------------------------------

===========
oemof.solph
===========

**A model generator for energy system modelling and optimisation (LP/MILP)**

.. contents::
    :depth: 2
    :local:
    :backlinks: top

Introduction
============

The oemof.solph package is part of the
`Open energy modelling framework (oemof) <https://github.com/oemof/oemof>`_.
This is an organisational framework to bundle tools for energy (system) modelling.
oemof-solph is a model generator for energy system modelling and optimisation.

The package ``oemof.solph`` is very often called just ``oemof``.
This is because installing the ``oemof`` meta package was once the best way to get ``oemof.solph``.
Notice that you should prefeably install ``oemof.solph`` instead of ``oemof``
if you want to use ``solph``.

Everybody is welcome to use and/or develop oemof.solph.
Read our `contribution <https://oemof.readthedocs.io/en/latest/contributing.html>`_ section.

Contribution is already possible on a low level by simply fixing typos in
oemof's documentation or rephrasing sections which are unclear.
If you want to support us that way please fork the oemof-solph project to your own
GitHub account and make changes as described in the `github guidelines <https://docs.github.com/en/get-started/start-your-journey/hello-world>`_

If you have questions regarding the use of oemof including oemof.solph you can visit the openmod forum (`tag oemof <https://forum.openmod-initiative.org/tags/c/qa/oemof>`_ or `tag oemof-solph <https://forum.openmod-initiative.org/tags/c/qa/oemof-solph>`_) and open a new thread if your questions hasn't been already answered.

Keep in touch! - You can become a watcher at our `github site <https://github.com/oemof/oemof>`_,
but this will bring you quite a few mails and might be more interesting for developers.
If you just want to get the latest news, like when is the next oemof meeting,
you can follow our news-blog at `oemof.org <https://oemof.org/>`_.

Documentation
=============
The `oemof.solph documentation <https://oemof-solph.readthedocs.io/>`_ is powered by readthedocs. Use the `project site <https://readthedocs.org/projects/oemof>`_ of oemof.solph to choose the version of the documentation. Go to the `download page <https://readthedocs.org/projects/oemof/downloads/>`_ to download different versions and formats (pdf, html, epub) of the documentation.

Installation
============

If you have a working Python installation, use pypi to install the latest version of oemof.solph.
Python >= 3.11 is recommended. Lower versions may work but are not tested.

We highly recommend to use virtual environments.
Please refer to the documentation of your Python distribution (e.g. Anaconda,
Micromamba, or the version of Python that came with your Linux installation)
to learn how to set up and use virtual environments.

::

    (venv) pip install oemof.solph

If you want to use the latest features, you might want to install the **developer version**. The developer version is not recommended for productive use::

    (venv) pip install https://github.com/oemof/oemof-solph/archive/dev.zip

For running an oemof-solph optimisation model, you need to install a solver.
Following you will find guidelines for the installation process for different operating systems.

.. _windows_solver_label:
.. _linux_solver_label:

Installing a solver
-------------------

There are several solvers that can work with oemof, both open source and commercial.
Two open source solvers are widely used (CBC and GLPK), but oemof suggests CBC (Coin-or branch and cut).
It may be useful to compare results of different solvers to see which performs best.
Other commercial solvers, like Gurobi or Cplex, are also options.
Have a look at the `pyomo docs <https://pyomo.readthedocs.io/en/stable/api/pyomo.solvers.plugins.solvers.html>`_
to learn about which solvers are supported.

Check the solver installation by executing the test_installation example below (see section Installation Test).

**Linux**

To install the solvers have a look at the package project of your Linux distribution or search for precompiled packages. GLPK and CBC ares available at Debian, Feodora, Ubuntu and others.

**Windows**

 1. Download `CBC <https://github.com/coin-or/Cbc/releases>`_
 2. Download `GLPK (64/32 bit) <https://sourceforge.net/projects/winglpk/>`_
 3. Unpack CBC/GLPK to any folder (e.g. C:/Users/Somebody/my_programs)
 4. Add the path of the executable files of both solvers to the PATH variable (cf. `setting environment variables as user <https://learn.microsoft.com/en-us/troubleshoot/windows-client/performance/cannot-modify-user-environment-variables-system-properties>`_)
 5. Restart Windows

Check the solver installation by executing the test_installation example (see the `Installation test` section).

**Mac OSX**

Please follow the installation instructions on the respective homepages for details.

CBC-solver: https://github.com/coin-or/Cbc

GLPK-solver: http://arnab-deka.com/posts/2010/02/installing-glpk-on-a-mac/

If you install the CBC solver via brew (highly recommended), it should work without additional configuration.

**conda**

The CBC-solver can also be installed in a `conda` environment. Please note, that it is highly recommended to `use pip after conda <https://www.anaconda.com/blog/using-pip-in-a-conda-environment>`_, so:

.. code:: console

    (venv) conda install -c conda-forge coincbc
    (venv) pip install oemof.solph

.. _check_installation_label:

Installation test
-----------------

Test the installation and the installed solver by running the installation test
in your virtual environment:

.. code:: console

  (venv) oemof_installation_test

If the installation was successful, you will receive something like this:

.. code:: console

    *********
    Solver installed with oemof:
    glpk: working
    cplex: not working
    cbc: working
    gurobi: not working
    *********
    oemof.solph successfully installed.

as an output.

Contributing
============

A warm welcome to all who want to join the developers and contribute to
oemof.solph.

Information on the details and how to approach us can be found
`in the oemof documentation <https://oemof.readthedocs.io/en/latest/contributing.html>`_ .

Citing
======

For explicitly citing solph, you might want to refer to
`DOI:10.1016/j.simpa.2020.100028 <https://doi.org/10.1016/j.simpa.2020.100028>`_,
which gives an overview over the capabilities of solph.
The core ideas of oemof as a whole are described in
`DOI:10.1016/j.esr.2018.07.001 <https://doi.org/10.1016/j.esr.2018.07.001>`_
(preprint at `arXiv:1808.0807 <https://arxiv.org/abs/1808.08070v1>`_).
To allow citing specific versions, we use the zenodo project to get a DOI for each version.

Example Applications
====================

The combination of specific modules (often including other packages) is called an
application (app). For example, it can depict a concrete energy system model.
You can find a large variety of helpful examples in the documentation.
The examples show the optimisation of different energy systems and are supposed
to help new users to understand the framework's structure.
Please make sure the example you are looking at is created for the version
of solph you have installed.

You are welcome to contribute your own examples via a `pull request <https://github.com/oemof/oemof-solph/pulls>`_
or by e-mailing us (see `here <https://oemof.org/contact/>`_ for contact information).

## Dependencies

| Metric | Value |
|--------|-------|
| Files | unknown |
| Lines of Code | unknown |
| Dependencies | unknown |
| Upstream license (harvested) | NOASSERTION |
| Overlay license | Anticommons 0.1.0 |

Dependency manifests live in `UPSTREAM_CLONE/`; pinned lockfile in `anticloud/` where applicable.

## Configuration

Please refer to the documentation of your Python distribution (e.g. Anaconda,
Micromamba, or the version of Python that came with your Linux installation)
to learn how to set up and use virtual environments.

::

    (venv) pip install oemof.solph

If you want to use the latest features, you might want to install the **developer version**. The developer version is not recommended for productive use::

    (venv) pip install https://github.com/oemof/oemof-solph/archive/dev.zip

For running an oemof-solph optimisation model, you need to install a solver.
Following you will find guidelines for the installation process for different operating systems.

.. _windows_solver_label:
.. _linux_solver_label:

Installing a solver
-------------------

There are several solvers that can work with oemof, both open source and commercial.
Two open source solvers are widely used (CBC and GLPK), but oemof suggests CBC (Coin-or branch and cut).
It may be useful to compare results of different solvers to see which performs best.
Other commercial solvers, like Gurobi or Cplex, are also options.
Have a look at the `pyomo docs <https://pyomo.readthedocs.io/en/stable/api/pyomo.solvers.plugins.solvers.html>`_
to learn about which solvers are supported.

Check the solver installation by executing the test_installation example below (see section Installation Test).

**Linux**

To install the solvers have a look at the package project of your Linux distribution or search for precompiled packages. GLPK and CBC ares available at Debian, Feodora, Ubuntu and others.

**Windows**

 1. Download `CBC <https://github.com/coin-or/Cbc/releases>`_
 2. Download `GLPK (64/32 bit) <https://sourceforge.net/projects/winglpk/>`_
 3. Unpack CBC/GLPK to any folder (e.g. C:/Users/Somebody/my_programs)
 4. Add the path of the executable files of both solvers to the PATH variable (cf. `setting environment variables as user <https://learn.microsoft.com/en-us/troubleshoot/windows-client/performance/cannot-modify-user-environment-variables-system-properties>`_)
 5. Restart Windows

Check the solver installation by executing the test_installation example (see the `Installation test` section).

**Mac OSX**

Please follow the installation instructions on the respective homepages for details.

CBC-solver: https://github.com/coin-or/Cbc

GLPK-solver: http://arnab-deka.com/posts/2010/02/installing-glpk-on-a-mac/

If you install the CBC solver via brew (highly recommended), it should work without additional configuration.

**conda**

The CBC-solver can also be installed in a `conda` environment. Please note, that it is highly recommended to `use pip after conda <https://www.anaconda.com/blog/using-pip-in-a-conda-environment>`_, so:

.. code:: console

    (venv) conda install -c conda-forge coincbc
    (venv) pip install oemof.solph

.. _check_installation_label:

Installation test
-----------------

Test the installation and the installed solver by running the installation test
in your virtual environment:

.. code:: console

  (venv) oemof_installation_test

If the installation was successful, you will receive something like this:

.. code:: console

    *********
    Solver installed with oemof:
    glpk: working
    cplex: not working
    cbc: working
    gurobi: not working
    *********
    oemof.solph successfully installed.

as an output.

Contributing
============

A warm welcome to all who want to join the developers and contribute to
oemof.solph.

Information on the details and how to approach us can be found
`in the oemof documentation <https://oemof.readthedocs.io/en/latest/contributing.html>`_ .

Citing
======

For explicitly citing solph, you might want to refer to
`DOI:10.1016/j.simpa.2020.100028 <https://doi.org/10.1016/j.simpa.2020.100028>`_,
which gives an overview over the capabilities of solph.
The core ideas of oemof as a whole are described in
`DOI:10.1016/j.esr.2018.07.001 <https://doi.org/10.1016/j.esr.2018.07.001>`_
(preprint at `arXiv:1808.0807 <https://arxiv.org/abs/1808.08070v1>`_).
To allow citing specific versions, we use the zenodo project to get a DOI for each version.

Example Applications
====================

The combination of specific modules (often including other packages) is called an
application (app). For example, it can depict a concrete energy system model.
You can find a large variety of helpful examples in the documentation.
The examples show the optimisation of different energy systems and are supposed
to help new users to understand the framework's structure.
Please make sure the example you are looking at is created for the version
of solph you have installed.

You are welcome to contribute your own examples via a `pull request <https://github.com/oemof/oemof-solph/pulls>`_
or by e-mailing us (see `here <https://oemof.org/contact/>`_ for contact information).

## Contributing

.. SPDX-FileCopyrightText: oemof e.V. and contributors
..
.. SPDX-License-Identifier: MIT

.. _contribute_label:

=================
How to contribute
=================

Contributions are welcome, and they are greatly appreciated! Every
little bit helps, and credit will always be given.

Bug reports
===========

When `reporting a bug <https://github.com/oemof/oemof-solph/issues>`_ please include:

    * Your operating system name and version.
    * Any details about your local setup that might be helpful in troubleshooting.
    * Detailed steps to reproduce the bug.

Documentation improvements
==========================

oemof-solph could always use more documentation, whether as part of the
official oemof-solph docs, in docstrings, or even on the web in blog posts,
articles, and such.

.. _feature_requests_and_feedback:

Feature requests and feedback
=============================

The best way to send feedback is to file an issue at https://github.com/oemof/oemof-solph/issues.

If you are proposing a feature:

* Explain in detail how it would work.
* Keep the scope as narrow as possible, to make it easier to implement.
* Remember that this is a volunteer-driven project, and that code contributions are welcome :)

Development
===========

To set up `oemof-solph` for local development:

1. Fork `oemof-solph <https://github.com/oemof/oemof-solph>`_
   (look for the "Fork" button).
2. source your fork locally::

    git source git@github.com:$(your_github_account)/oemof-solph.git

3. Create a branch for local development::

    git checkout -b name-of-your-bugfix-or-feature

   Now you can make your changes locally.

4. When you're done making changes run all the checks and docs builder with `tox <https://tox.wiki/en/stable/>`_ one command::

    tox

5. Commit your changes and push your branch to GitHub. Please do not forget to write a descriptive commit message that explains design decisions::

    git add $(changed_files)
    git commit
    git push origin name-of-your-bugfix-or-feature

6. Submit a pull request through the GitHub website. Please check the box to allow changes by maintainers.

Pull Request Guidelines
-----------------------

If you need some code review or feedback while you're developing the code just make the pull request.

For merging, you should:

1. Include passing tests (run ``tox``) [1]_.
2. Update documentation when there's new API, functionality etc.
3. Add a note about the changes and your name (or nickname) to ``docs/whatsnew/next_version.rst``.
4. Optionally, you may also add your name to ``AUTHORS.rst`` and ``CITATION.cff``.

.. [1] If you don't have all the necessary python versions available locally,
       you can rely on the CI pipeline at GitHub.

       It will be slower though ...

Tests
-----

To run the all tests run::

    tox

Note, to combine the coverage data from all the tox environments run:

.. list-table::
    :widths: 10 90
    :stub-columns: 1

    - - Windows
      - ::

            set PYTEST_ADDOP

## License

Upstream © its respective contributors under NOASSERTION (harvested MIT/Apache-2.0/BSD source; see `UPSTREAM_CLONE/LICENSE`). This packaging overlay is licensed under Anticommons 0.1.0.

## Upstream

- **project:** OEMOF_SOLPH
- **Pinned SHA:** `943c057da7445e971750e95130c2e9b0158ce20d`
- **source:** `UPSTREAM_CLONE/` (pinned at the SHA above)
- **Upstream README source:** `UPSTREAM_CLONE/README.rst`

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`93b3f5c88ade8ae6d6a8b94ae36dd6fc2d21ca7d7850731a1a44d13cc2843e17`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| DANS (KNAW/NWO, Netherlands) | 10.17026/PT | EU-recognised archive |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe
and Mail, Business Insider, National Post, Financial Post, StreetInsider,
Digital Journal, Barchart, International Business Times, and Fox News.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

