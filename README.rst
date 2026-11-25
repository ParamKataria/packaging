packaging
=========

.. start-intro

Reusable core utilities for various Python Packaging
`interoperability specifications <https://packaging.python.org/specifications/>`_.

This library provides utilities that implement the interoperability
specifications which have clearly one correct behaviour (eg: :pep:`440`)
or benefit greatly from having a single shared implementation (eg: :pep:`425`).

.. end-intro

The ``packaging`` project includes the following: version handling, specifiers,
markers, requirements, tags, metadata, lockfiles, utilities.

Documentation
-------------

The `documentation`_ provides information and the API for the following:

- Version Handling
- Specifiers
- Markers
- Licenses
- Requirements
- Metadata
- Tags
- Lockfiles (pylock)
- Direct URL helpers
- Dependency groups
- Errors
- Utilities

Installation
------------

Use ``pip`` to install these utilities::

    pip install packaging

The ``packaging`` library uses calendar-based versioning (``YY.N``).

Building and Testing from Source
--------------------------------

Requires **Python 3.10 or newer** (no third-party runtime dependencies).

1. Clone the repository and enter the project directory::

       git clone https://github.com/ParamKataria/packaging.git
       cd packaging

2. Create and activate a virtual environment:

   On macOS / Linux::

       python3 -m venv .venv
       source .venv/bin/activate

   On Windows (PowerShell)::

       python -m venv .venv
       .venv\Scripts\Activate.ps1

3. Install the package in editable mode along with its test dependencies::

       pip install --upgrade pip
       pip install -e . --group test

   If using an older ``pip`` version that does not support ``--group``, install
   the test dependencies directly::

       pip install -e . pytest pretend tomli_w hypothesis coverage

4. Run the unit test suite::

       pytest

5. *(Optional)* Build source and wheel distributions::

       pip install build
       python -m build

Discussion
----------

If you run into bugs, you can file them in our `issue tracker`_.

You can also ask questions or get involved in the `Packaging category`_ on
discuss.python.org.

.. _`documentation`: https://packaging.pypa.io/
.. _`issue tracker`: https://github.com/pypa/packaging/issues
.. _`Packaging category`: https://discuss.python.org/c/packaging/14


Code of Conduct
---------------

Everyone interacting in the packaging project's codebases, issue trackers, chat
rooms, and mailing lists is expected to follow the `PSF Code of Conduct`_.

.. _PSF Code of Conduct: https://github.com/pypa/.github/blob/main/CODE_OF_CONDUCT.md

Contributing
------------

The ``CONTRIBUTING.rst`` file outlines how to contribute to this project as
well as how to report a potential security issue. The documentation for this
project also covers information about `project development`_ and `security`_.

.. _`project development`: https://packaging.pypa.io/en/latest/development/
.. _`security`: https://packaging.pypa.io/en/latest/security/

Project History
---------------

Please review the ``CHANGELOG.rst`` file or the `Changelog documentation`_ for
recent changes and project history.

.. _`Changelog documentation`: https://packaging.pypa.io/en/latest/changelog/
