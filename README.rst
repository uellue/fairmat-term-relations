:code:`fairmat-term-relations` is a demo for a structured collection of terms
and relations based on Sphinx and RST files.

Installation
------------

* Clone this repo
* Set up a Python environment
* Install the required packages: :code:`pip install -r requirements.txt`

Build
-----

* For a live-updating build: Run :code:`sphinx-autobuild source build/html`
  in the root directory of the cloned repository and open the URL in your browser,
  by default http://localhost:8000/.
* For a static HTML build: Run :code:`make html`.
* See https://www.sphinx-doc.org/en/master/ for more information!

.. note::
    Many features and tags in README.rst don't work stand-alone,
    but only if this file is embedded in :code:`index.rst` and built
    with the rest of the project!


How it works
------------

* Terms are defined as individual files in :code:`./source/terms/`.
* An overview of terms is generated with a table of content in :ref:`terms`.
* Relation between terms are defined in :ref:`relations`. This can be
  structured in smaller units as well by splitting it in files, just like the terms, if desired.
* The main document :code:`./source/index.rst` provides an overview.

Features
--------

* BibTeX bibliography and citations like so: :cite:`clausen_alexander_2021_5547992`.
* Intersphinx links such as :ref:`numpy:whatisnumpy`. Entries here are also linkable from
  other Sphinx documentation in the same way, once the documentation is online.
* Links to Issues or Pull Requests on GitHub like :issue:`1`, for example.
* Human-readable and accessible, can easily be built to documents in various formats
* Can be machine-readable if a defined form is kept for entries. Possibly, entries
  can be pre-compiled from another source of truth, like for example `author
  information in LiberTEM <https://libertem.github.io/LiberTEM/acknowledgments.html>`_
  that is compiled from a JSON file.
* Suitable for GitHub-based collaborative editing since individual files for entries avoid
  merge conflicts.
* Many more Sphinx features available if desired, such as testing code examples
  and/or building documentation from Jupyter notebooks.

Acknowledgments
---------------

Based on the changelog infrastructure of `LiberTEM <https://libertem.github.io/LiberTEM/>`_.
