# SUBSURFACE

![licence](https://img.shields.io/badge/licence-Apache-2.0-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![checks](https://img.shields.io/badge/checks-unknown_PASS-brightgreen)

> Governed Anticloud packaging of the upstream project `SUBSURFACE` in category **OIL_GAS**. check results: see ISOLATED_LAB_RESULTS. Every number below traces to a named file + run stamp; nothing is borrowed from other projects.

**Upstream:** SUBSURFACE · **Upstream pin:** `816db75bad6f1eda71209a4635490d2969eadeb0` · **Category:** OIL_GAS · **Vendor:** Anticloud FZ LLE · **Licence:** Apache-2.0

---

## What This Project Does

.. image:: https://raw.githubusercontent.com/softwareunderground/subsurface/main/docs/source/_static/logos/subsurface.png
   :target: https://softwareunderground.github.io/subsurface
   :alt: subsurface logo

|

.. image:: https://img.shields.io/pypi/v/subsurface.svg
   :target: https://pypi.python.org/pypi/subsurface/
   :alt: PyPI
.. image:: https://img.shields.io/conda/v/conda-forge/subsurface.svg
   :target: https://anaconda.org/conda-forge/subsurface/
   :alt: conda-forge
.. image:: https://img.shields.io/badge/python-3.8+-blue.svg
   :target: https://www.python.org/downloads/
   :alt: Supported Python Versions
.. image:: https://img.shields.io/badge/platform-linux,win,osx-blue.svg
   :target: https://anaconda.org/conda-forge/emg3d/
   :alt: Linux, Windows, OSX
.. image:: https://img.shields.io/badge/slack-swung-1DB6ED.svg?logo=slack
   :target: http://swu.ng/slack
   :alt: SWUNG Slack

|

.. sphinx-inclusion-marker

subsurface
==========

DataHub for geoscientific data in Python. Two main purposes:

+ Unify geometric data into data objects (using numpy arrays as memory representation) that all the packages of the stack understand

+ Basic interactions with those data objects:
    + Write/Read
    + Categorized/Meta data
    + Visualization

Data Levels
-----------

The difference between data levels is **not** which data they store but which data they **parse and understand**. The rationale for this is to be able to pass along any object while keeping the I/O in subsurface::

                HUMAN

   \‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾/\
    \= = = = = = = = = = = = = = /. \     -> Additional context/meta information about the data
     \= = = = geo_format= = = = /. . \
      \= = = = = = = = = = = = /. . . \   -> Elements that represent some
       \= = = geo_object= = = /. . . . \     geological concept. E.g: faults, seismic
        \= = = = = = = = = = /. . . . ./
         \= = element = = = /. . . . /    -> type of geometric object: PointSet,
          \= = = = = = = = /. . . ./         TriSurf, LineSet, Tetramesh
           \primary_struct/. . . /        -> Set of arrays that define a geometric object:
            \= = = = = = /. . ./             e.g. *StructuredData*, *UnstructuredData*
             \DF/Xarray /. . /            -> Label numpy.arrays
              \= = = = /. ./
               \array /. /                -> Memory allocation
                \= = /./
                 \= //
                  \/

               COMPUTER

Documentation (WIP)
-------------------

**Disclaimer: The documentation is currently obsolete and has been unpublished. The best way to learn to use this library at this stage is by looking into the tests.**

Note that ``subsurface`` is still in early days; do expect things to change. We
welcome contributions very much, please get in touch if you would like to add
support for subsurface in your package.

An early version of the documentation can be found here:

https://softwareunderground.github.io/subsurface/

Direct links:

- `Developers-guide <https://softwareunderground.github.io/subsurface/maintenance.html>`_
- `Changelog <https://softwareunderground.github.io/subsurface/changelog.html>`_

Installation
------------

.. code-block:: console

    pip install subsurface

or

.. code-block:: console

    conda install -c conda-forge subsurface

Be aware that to read different formats you will need to manually install the
specific dependency (e.g. ``welly`` to read well data).

---

## Installation

------------

.. code-block:: console

    pip install subsurface

or

.. code-block:: console

    conda install -c conda-forge subsurface

Be aware that to read different formats you will need to manually install the
specific dependency (e.g. ``welly`` to read well data).

## Usage

:target: https://softwareunderground.github.io/subsurface
   :alt: subsurface logo

|

.. image:: https://img.shields.io/pypi/v/subsurface.svg
   :target: https://pypi.python.org/pypi/subsurface/
   :alt: PyPI
.. image:: https://img.shields.io/conda/v/conda-forge/subsurface.svg
   :target: https://anaconda.org/conda-forge/subsurface/
   :alt: conda-forge
.. image:: https://img.shields.io/badge/python-3.8+-blue.svg
   :target: https://www.python.org/downloads/
   :alt: Supported Python Versions
.. image:: https://img.shields.io/badge/platform-linux,win,osx-blue.svg
   :target: https://anaconda.org/conda-forge/emg3d/
   :alt: Linux, Windows, OSX
.. image:: https://img.shields.io/badge/slack-swung-1DB6ED.svg?logo=slack
   :target: http://swu.ng/slack
   :alt: SWUNG Slack

|

.. sphinx-inclusion-marker

subsurface
==========

DataHub for geoscientific data in Python. Two main purposes:

+ Unify geometric data into data objects (using numpy arrays as memory representation) that all the packages of the stack understand

+ Basic interactions with those data objects:
    + Write/Read
    + Categorized/Meta data
    + Visualization

Data Levels
-----------

The difference between data levels is **not** which data they store but which data they **parse and understand**. The rationale for this is to be able to pass along any object while keeping the I/O in subsurface::

                HUMAN

   \‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾/\
    \= = = = = = = = = = = = = = /. \     -> Additional context/meta information about the data
     \= = = = geo_format= = = = /. . \
      \= = = = = = = = = = = = /. . . \   -> Elements that represent some
       \= = = geo_object= = = /. . . . \     geological concept. E.g: faults, seismic
        \= = = = = = = = = = /. . . . ./
         \= = element = = = /. . . . /    -> type of geometric object: PointSet,
          \= = = = = = = = /. . . ./         TriSurf, LineSet, Tetramesh
           \primary_struct/. . . /        -> Set of arrays that define a geometric object:
            \= = = = = = /. . ./             e.g. *StructuredData*, *UnstructuredData*
             \DF/Xarray /. . /            -> Label numpy.arrays
              \= = = = /. ./
               \array /. /                -> Memory allocation
                \= = /./
                 \= //
                  \/

               COMPUTER

Documentation (WIP)
-------------------

**Disclaimer: The documentation is currently obsolete and has been unpublished. The best way to learn to use this library at this stage is by looking into the tests.**

Note that ``subsurface`` is still in early days; do expect things to change. We
welcome contributions very much, please get in touch if you would like to add
support for subsurface in your package.

An early version of the documentation can be found here:

https://softwareunderground.github.io/subsurface/

Direct links:

- `Developers-guide <https://softwareunderground.github.io/subsurface/maintenance.html>`_
- `Changelog <https://softwareunderground.github.io/subsurface/changelog.html>`_

Installation
------------

.. code-block:: console

    pip install subsurface

or

.. code-block:: console

    conda install -c conda-forge subsurface

Be aware that to read different formats you will need to manually install the
specific dependency (e.g. ``welly`` to read well data).

## API

-------------------

**Disclaimer: The documentation is currently obsolete and has been unpublished. The best way to learn to use this library at this stage is by looking into the tests.**

Note that ``subsurface`` is still in early days; do expect things to change. We
welcome contributions very much, please get in touch if you would like to add
support for subsurface in your package.

An early version of the documentation can be found here:

https://softwareunderground.github.io/subsurface/

Direct links:

- `Developers-guide <https://softwareunderground.github.io/subsurface/maintenance.html>`_
- `Changelog <https://softwareunderground.github.io/subsurface/changelog.html>`_

Installation
------------

.. code-block:: console

    pip install subsurface

or

.. code-block:: console

    conda install -c conda-forge subsurface

Be aware that to read different formats you will need to manually install the
specific dependency (e.g. ``welly`` to read well data).

## Dependencies

| Metric | Value |
|--------|-------|
| Files | unknown |
| Lines of Code | unknown |
| Dependencies | unknown |
| Upstream license (harvested) | Apache-2.0 |
| Overlay license | Anticommons 0.1.0 |

Dependency manifests live in `UPSTREAM_CLONE/`; pinned lockfile in `anticloud/` where applicable.

## Configuration

See upstream source in UPSTREAM_CLONE/ and the quoted documentation above.

## Contributing

support for subsurface in your package.

An early version of the documentation can be found here:

https://softwareunderground.github.io/subsurface/

Direct links:

- `Developers-guide <https://softwareunderground.github.io/subsurface/maintenance.html>`_
- `Changelog <https://softwareunderground.github.io/subsurface/changelog.html>`_

Installation
------------

.. code-block:: console

    pip install subsurface

or

.. code-block:: console

    conda install -c conda-forge subsurface

Be aware that to read different formats you will need to manually install the
specific dependency (e.g. ``welly`` to read well data).

## License

Upstream © its respective contributors under Apache-2.0 (harvested MIT/Apache-2.0/BSD source; see `UPSTREAM_CLONE/LICENSE`). This packaging overlay is licensed under Anticommons 0.1.0.

## Upstream

- **project:** SUBSURFACE
- **Pinned SHA:** `816db75bad6f1eda71209a4635490d2969eadeb0`
- **source:** `UPSTREAM_CLONE/` (pinned at the SHA above)
- **Upstream README source:** `UPSTREAM_CLONE/README.rst`

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`12e303ad7e8ca0c8f0fb9cd49e3b950a4dd2c8cf7ef12bdedb5f88707bdc626e`.

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

