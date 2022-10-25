How to contribute
=================

Getting started
---------------

So you're interested in contributing to ``odata-query``? That's great! We're
excited to hear your ideas and experiences.

This file describes all the different ways in which you can contribute.


Reporting a bug
------------------

Have you encountered a bug? Please let us know by reporting it.

Before doing so, take a look at the existing `Issues`_ to make sure the bug you
encountered hasn't already been reported by someone else. If so, we ask you to
reply to the existing Issue rather than creating a new one. Bugs with many
replies will obviously have a higher priority.

If the bug you encountered has not been reported yet, create a new Issue for it
and make sure to label it as a 'bug'. To allow us to help you as efficiently as
possible, always try to include the following:

- Which version of ``odata-query`` are you using?
- What went wrong?
- What did you expect to happen?
- Detailed steps to reproduce.

The maintainer of this repository monitors issues on a regular basis and will
respond to your bug report as soon as possible.


Requesting an enhancement
-------------------------

Do you have a great idea that could make ``odata-query`` even better?
Feel free to request an enhancement.

Before doing so, take a look at the existing `Issues`_ to make sure your idea
hasn't already been requested by someone else. If so, we ask you to reply or
give a thumbs-up to the existing Issue rather than creating a new one. Requests
with many replies will obviously have a higher priority.

If your idea has not been requested yet, create a new Issue for it and make sure
to label it as an 'enhancement'. Explain what your idea is in detail and how it
could improve ``odata-query``.

The maintainer of this repository monitors issues on a regular basis and will
respond to your request as soon as possible.


Contributing code
-----------------

Would you prefer to contribute directly by writing some code yourself? That's
great.

**If your contribution is minor**, such as fixing a bug or typo, we encourage
you to open a pull request right away.

**If your contribution is major**, such as a new feature or a breaking change,
start by opening an issue first. That way, other people can weigh in on the
discussion before you do any work.

The workflow for creating a pull request:

1. Fork the repository.
2. ``clone`` your forked repository.
3. Create a new feature branch from the ``master`` branch.
4. Make your contributions to the project's code. Please run the tests before
   committing, and keep the code style conform to the project's style guide
   (listed below).
5. Add documentation where required. Please keep the style conform.
6. Add your changes to the :ref:`changelog` in the "Unreleased"
   section. Include a link to your GitHub profile for some internet fame.
7. ``commit`` your changes in logical chunks.
8. ``push`` your branch to your fork on GitHub.
9. Create a pull request from your feature branch to the original repository's
   ``master`` branch.

The maintainer of this repository monitors pull requests on a regular basis and
will respond as soon as possible. The smaller individual pull requests are, the
faster the maintainer will be able to respond.


Local development
^^^^^^^^^^^^^^^^^

``odata-query`` uses `poetry`_ to manage the package and its dependencies, and
`tox`_ to run tests and linting in dedicated environments.

To install the project for development, run:

.. code-block:: bash

    poetry install -E testing -E linting -E docs


To run all tests and linting, run:

.. code-block:: bash

    tox

To ensure your files are configured correctly (linting will bug you if they're not),
you can configure your IDE to use the included linting tools OR run them manually
as follows:


.. code-block:: bash

    poetry run black .  # Format files to adhere to the Black code style
    poetry run isort .  # Ensure the imports are organised correctly


Contact
-------

Discussions about ``odata-query`` take place on this repository's `Issues`_ and
`Pull Requests`_ sections. Anybody is welcome to join the conversation. Wherever
possible, do not take these conversations to private channels, including
contacting the maintainers directly. Keeping communication public means
everybody can benefit and learn.


.. _Issues: https://github.com/gorilla-co/odata-query/issues
.. _Pull Requests: https://github.com/gorilla-co/odata-query/pulls
.. _poetry: https://python-poetry.org/
.. _tox: https://tox.readthedocs.io/en/latest/index.html
