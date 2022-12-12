<div align="center">
  <img src="https://pandas.pydata.org/static/img/pandas.svg"><br>
</div>

-----------------

# pandas: powerful Python data analysis toolkit
[![PyPI Latest Release](https://img.shields.io/pypi/v/pandas.svg)](https://pypi.org/project/pandas/)
[![Conda Latest Release](https://anaconda.org/conda-forge/pandas/badges/version.svg)](https://anaconda.org/anaconda/pandas/)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3509134.svg)](https://doi.org/10.5281/zenodo.3509134)
[![Package Status](https://img.shields.io/pypi/status/pandas.svg)](https://pypi.org/project/pandas/)
[![License](https://img.shields.io/pypi/l/pandas.svg)](https://github.com/pandas-dev/pandas/blob/main/LICENSE)
[![Coverage](https://codecov.io/github/pandas-dev/pandas/coverage.svg?branch=main)](https://codecov.io/gh/pandas-dev/pandas)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/pandas-dev/pandas/badge)](https://api.securityscorecards.dev/projects/github.com/pandas-dev/pandas)
[![Downloads](https://static.pepy.tech/personalized-badge/pandas?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/pandas)
[![Slack](https://img.shields.io/badge/join_Slack-information-brightgreen.svg?logo=slack)](https://pandas.pydata.org/docs/dev/development/community.html?highlight=slack#community-slack)
[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)

## What is it?

**pandas** is a Python package that provides fast, flexible, and expressive data
structures designed to make working with "relational" or "labeled" data both
easy and intuitive. It aims to be the fundamental high-level building block for
doing practical, **real world** data analysis in Python. Additionally, it has
the broader goal of becoming **the most powerful and flexible open source data
analysis / manipulation tool available in any language**. It is already well on
its way towards this goal.

## Main Features
Here are just a few of the things that pandas does well:

  - Easy handling of [**missing data**][missing-data] (represented as
    `NaN`, `NA`, or `NaT`) in floating point as well as non-floating point data
  - Size mutability: columns can be [**inserted and
    deleted**][insertion-deletion] from DataFrame and higher dimensional
    objects
  - Automatic and explicit [**data alignment**][alignment]: objects can
    be explicitly aligned to a set of labels, or the user can simply
    ignore the labels and let `Series`, `DataFrame`, etc. automatically
    align the data for you in computations
  - Powerful, flexible [**group by**][groupby] functionality to perform
    split-apply-combine operations on data sets, for both aggregating
    and transforming data
  - Make it [**easy to convert**][conversion] ragged,
    differently-indexed data in other Python and NumPy data structures
    into DataFrame objects
  - Intelligent label-based [**slicing**][slicing], [**fancy
    indexing**][fancy-indexing], and [**subsetting**][subsetting] of
    large data sets
  - Intuitive [**merging**][merging] and [**joining**][joining] data
    sets
  - Flexible [**reshaping**][reshape] and [**pivoting**][pivot-table] of
    data sets
  - [**Hierarchical**][mi] labeling of axes (possible to have multiple
    labels per tick)
  - Robust IO tools for loading data from [**flat files**][flat-files]
    (CSV and delimited), [**Excel files**][excel], [**databases**][db],
    and saving/loading data from the ultrafast [**HDF5 format**][hdfstore]
  - [**Time series**][timeseries]-specific functionality: date range
    generation and frequency conversion, moving window statistics,
    date shifting and lagging


   [missing-data]: https://pandas.pydata.org/pandas-docs/stable/user_guide/missing_data.html
   [insertion-deletion]: https://pandas.pydata.org/pandas-docs/stable/user_guide/dsintro.html#column-selection-addition-deletion
   [alignment]: https://pandas.pydata.org/pandas-docs/stable/user_guide/dsintro.html?highlight=alignment#intro-to-data-structures
   [groupby]: https://pandas.pydata.org/pandas-docs/stable/user_guide/groupby.html#group-by-split-apply-combine
   [conversion]: https://pandas.pydata.org/pandas-docs/stable/user_guide/dsintro.html#dataframe
   [slicing]: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#slicing-ranges
   [fancy-indexing]: https://pandas.pydata.org/pandas-docs/stable/user_guide/advanced.html#advanced
   [subsetting]: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#boolean-indexing
   [merging]: https://pandas.pydata.org/pandas-docs/stable/user_guide/merging.html#database-style-dataframe-or-named-series-joining-merging
   [joining]: https://pandas.pydata.org/pandas-docs/stable/user_guide/merging.html#joining-on-index
   [reshape]: https://pandas.pydata.org/pandas-docs/stable/user_guide/reshaping.html
   [pivot-table]: https://pandas.pydata.org/pandas-docs/stable/user_guide/reshaping.html
   [mi]: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#hierarchical-indexing-multiindex
   [flat-files]: https://pandas.pydata.org/pandas-docs/stable/user_guide/io.html#csv-text-files
   [excel]: https://pandas.pydata.org/pandas-docs/stable/user_guide/io.html#excel-files
   [db]: https://pandas.pydata.org/pandas-docs/stable/user_guide/io.html#sql-queries
   [hdfstore]: https://pandas.pydata.org/pandas-docs/stable/user_guide/io.html#hdf5-pytables
   [timeseries]: https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#time-series-date-functionality

## Where to get it
The source code is currently hosted on GitHub at:
https://github.com/pandas-dev/pandas

Binary installers for the latest released version are available at the [Python
Package Index (PyPI)](https://pypi.org/project/pandas) and on [Conda](https://docs.conda.io/en/latest/).

```sh
# conda
conda install pandas
```

```sh
# or PyPI
pip install pandas
```

## Dependencies
- [NumPy - Adds support for large, multi-dimensional arrays, matrices and high-level mathematical functions to operate on these arrays](https://www.numpy.org)
- [python-dateutil - Provides powerful extensions to the standard datetime module](https://dateutil.readthedocs.io/en/stable/index.html)
- [pytz - Brings the Olson tz database into Python which allows accurate and cross platform timezone calculations](https://github.com/stub42/pytz)

See the [full installation instructions](https://pandas.pydata.org/pandas-docs/stable/install.html#dependencies) for minimum supported versions of required, recommended and optional dependencies.

## Installation from sources
To install pandas from source you need [Cython](https://cython.org/) in addition to the normal
dependencies above. Cython can be installed from PyPI:

```sh
pip install cython
```

In the `pandas` directory (same one where you found this file after
cloning the git repo), execute:

```sh
python setup.py install
```

or for installing in [development mode](https://pip.pypa.io/en/latest/cli/pip_install/#install-editable):


```sh
python -m pip install -e . --no-build-isolation --no-use-pep517
```

or alternatively

```sh
python setup.py develop
```

See the full instructions for [installing from source](https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html#installing-from-source).

## License
[BSD 3](LICENSE)

## Documentation
The official documentation is hosted on PyData.org: https://pandas.pydata.org/pandas-docs/stable

## Background
Work on ``pandas`` started at [AQR](https://www.aqr.com/) (a quantitative hedge fund) in 2008 and
has been under active development since then.

## Getting Help

For usage questions, the best place to go to is [StackOverflow](https://stackoverflow.com/questions/tagged/pandas).
Further, general questions and discussions can also take place on the [pydata mailing list](https://groups.google.com/forum/?fromgroups#!forum/pydata).

## Discussion and Development
Most development discussions take place on GitHub in this repo. Further, the [pandas-dev mailing list](https://mail.python.org/mailman/listinfo/pandas-dev) can also be used for specialized discussions or design issues, and a [Slack channel](https://pandas.pydata.org/docs/dev/development/community.html?highlight=slack#community-slack) is available for quick development related questions.

## Contributing to pandas [![Open Source Helpers](https://www.codetriage.com/pandas-dev/pandas/badges/users.svg)](https://www.codetriage.com/pandas-dev/pandas)

All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.

A detailed overview on how to contribute can be found in the **[contributing guide](https://pandas.pydata.org/docs/dev/development/contributing.html)**.

If you are simply looking to start working with the pandas codebase, navigate to the [GitHub "issues" tab](https://github.com/pandas-dev/pandas/issues) and start looking through interesting issues. There are a number of issues listed under [Docs](https://github.com/pandas-dev/pandas/issues?labels=Docs&sort=updated&state=open) and [good first issue](https://github.com/pandas-dev/pandas/issues?labels=good+first+issue&sort=updated&state=open) where you could start out.

You can also triage issues which may include reproducing bug reports, or asking for vital information such as version numbers or reproduction instructions. If you would like to start triaging issues, one easy way to get started is to [subscribe to pandas on CodeTriage](https://www.codetriage.com/pandas-dev/pandas).

Or maybe through using pandas you have an idea of your own or are looking for something in the documentation and thinking ‘this can be improved’...you can do something about it!

Feel free to ask questions on the [mailing list](https://groups.google.com/forum/?fromgroups#!forum/pydata) or on [Slack](https://pandas.pydata.org/docs/dev/development/community.html?highlight=slack#community-slack).

As contributors and maintainers to this project, you are expected to abide by pandas' code of conduct. More information can be found at: [Contributor Code of Conduct](https://github.com/pandas-dev/.github/blob/master/CODE_OF_CONDUCT.md)

<div align="center">
  <img src="https://miro.medium.com/max/765/1*cyXCE-JcBelTyrK-58w6_Q.png"><br>
</div>

[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](
https://numfocus.org)
[![PyPI Downloads](https://img.shields.io/pypi/dm/numpy.svg?label=PyPI%20downloads)](
https://pypi.org/project/numpy/)
[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/numpy.svg?label=Conda%20downloads)](
https://anaconda.org/conda-forge/numpy)
[![Stack Overflow](https://img.shields.io/badge/stackoverflow-Ask%20questions-blue.svg)](
https://stackoverflow.com/questions/tagged/numpy)
[![Nature Paper](https://img.shields.io/badge/DOI-10.1038%2Fs41592--019--0686--2-blue)](
https://doi.org/10.1038/s41586-020-2649-2)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/numpy/numpy/badge)](https://api.securityscorecards.dev/projects/github.com/numpy/numpy)


NumPy is the fundamental package for scientific computing with Python.

- **Website:** https://www.numpy.org
- **Documentation:** https://numpy.org/doc
- **Mailing list:** https://mail.python.org/mailman/listinfo/numpy-discussion
- **Source code:** https://github.com/numpy/numpy
- **Contributing:** https://www.numpy.org/devdocs/dev/index.html
- **Bug reports:** https://github.com/numpy/numpy/issues
- **Report a security vulnerability:** https://tidelift.com/docs/security

It provides:

- a powerful N-dimensional array object
- sophisticated (broadcasting) functions
- tools for integrating C/C++ and Fortran code
- useful linear algebra, Fourier transform, and random number capabilities

Testing:

NumPy requires `pytest` and `hypothesis`.  Tests can then be run after installation with:

    python -c 'import numpy; numpy.test()'

Code of Conduct
----------------------

NumPy is a community-driven open source project developed by a diverse group of
[contributors](https://numpy.org/teams/). The NumPy leadership has made a strong
commitment to creating an open, inclusive, and positive community. Please read the
[NumPy Code of Conduct](https://numpy.org/code-of-conduct/) for guidance on how to interact
with others in a way that makes our community thrive.

Call for Contributions
----------------------

The NumPy project welcomes your expertise and enthusiasm!

Small improvements or fixes are always appreciated. If you are considering larger contributions
to the source code, please contact us through the [mailing
list](https://mail.python.org/mailman/listinfo/numpy-discussion) first.

Writing code isn’t the only way to contribute to NumPy. You can also:
- review pull requests
- help us stay on top of new and old issues
- develop tutorials, presentations, and other educational materials
- maintain and improve [our website](https://github.com/numpy/numpy.org)
- develop graphic design for our brand assets and promotional materials
- translate website content
- help with outreach and onboard new contributors
- write grant proposals and help with other fundraising efforts

For more information about the ways you can contribute to NumPy, visit [our website](https://numpy.org/contribute/). 
If you’re unsure where to start or how your skills fit in, reach out! You can
ask on the mailing list or here, on GitHub, by opening a new issue or leaving a
comment on a relevant issue that is already open.

Our preferred channels of communication are all public, but if you’d like to
speak to us in private first, contact our community coordinators at
numpy-team@googlegroups.com or on Slack (write numpy-team@googlegroups.com for
an invitation).

We also have a biweekly community call, details of which are announced on the
mailing list. You are very welcome to join.

If you are new to contributing to open source, [this
guide](https://opensource.guide/how-to-contribute/) helps explain why, what,
and how to successfully get involved.

<p align="center">
<img src="https://raw.githubusercontent.com/jmv74211/matplotlib/master/images/matplotlib_logo.png" width="50%">
</p>

![Status](https://img.shields.io/badge/Status-building-orange.svg) ![Version](https://img.shields.io/badge/version-3.2.1-blue.svg)


# Introduction to matplotlib

Matplotlib is a Python 2D plotting library which produces publication quality figures in a variety of hardcopy formats and interactive environments across platforms.

**Considerations**:

- The figure is the window or general page in which everything is drawn. You can create multiple independent figures. A figure can have other things, like a subtitle, which is a centered title of the figure, a legend, a color bar...

- Axes are added to the figure. The axes are the area in which the data is graphed with functions such as `plot()` and `scatter()`, and can have associated labels.

- Each axis has an x-axis and a y-axis, and each contains a numbering.

   There are also the labels of the axes, the title, and the legend that must be taken into account when you want to customize the axes, but also taking into account that the scales of the axes and the grid lines can be useful.

- The vertebral lines are lines that connect the axis marks and designate the boundaries of the data area, in other words, they are the simple square that you can see when you have initialized.

- **matplotlib** is the entire Python data display package.

- **pyplot** is a module in the matplotlib package. The module provides an interface that allows you to create shapes and axes implicitly and automatically to achieve the desired frame.

- Machine learning **data** for graphing on matplotlib **should be structured under the numpy library**.

# How to create graphics with matplotlib

`Matplotlib` allows you to create different graphics. The possible types and examples links are mentioned below:

## Line diagram

Create a simple plot.

<p>
<img src="https://raw.githubusercontent.com/jmv74211/matplotlib/master/images/line_diagram_intro.png" width="50%">
</p>

> You can find examples [here](https://github.com/jmv74211/matplotlib/tree/master/1_line_diagram)


# References

- Matplotlib: Visualization with Python, available in https://matplotlib.org/

- Codebasics youtube channel, Matplotlib Tutorial, available in https://www.youtube.com/watch?v=qqwf4Vuj8oM&list=PLeo1K3hjS3uu4Lr8_kro2AqaO6CFYgKOl&index=1

<img src="https://raw.githubusercontent.com/mwaskom/seaborn/master/doc/_static/logo-wide-lightbg.svg"><br>

--------------------------------------

seaborn: statistical data visualization
=======================================

[![PyPI Version](https://img.shields.io/pypi/v/seaborn.svg)](https://pypi.org/project/seaborn/)
[![License](https://img.shields.io/pypi/l/seaborn.svg)](https://github.com/mwaskom/seaborn/blob/master/LICENSE)
[![DOI](https://joss.theoj.org/papers/10.21105/joss.03021/status.svg)](https://doi.org/10.21105/joss.03021)
[![Tests](https://github.com/mwaskom/seaborn/workflows/CI/badge.svg)](https://github.com/mwaskom/seaborn/actions)
[![Code Coverage](https://codecov.io/gh/mwaskom/seaborn/branch/master/graph/badge.svg)](https://codecov.io/gh/mwaskom/seaborn)

Seaborn is a Python visualization library based on matplotlib. It provides a high-level interface for drawing attractive statistical graphics.


Documentation
-------------

Online documentation is available at [seaborn.pydata.org](https://seaborn.pydata.org).

The docs include a [tutorial](https://seaborn.pydata.org/tutorial.html), [example gallery](https://seaborn.pydata.org/examples/index.html), [API reference](https://seaborn.pydata.org/api.html), [FAQ](https://seaborn.pydata.org/faq), and other useful information.

To build the documentation locally, please refer to [`doc/README.md`](doc/README.md).

Dependencies
------------

Seaborn supports Python 3.7+ and no longer supports Python 2.

Installation requires [numpy](https://numpy.org/), [pandas](https://pandas.pydata.org/), and [matplotlib](https://matplotlib.org/). Some advanced statistical functionality requires [scipy](https://www.scipy.org/) and/or [statsmodels](https://www.statsmodels.org/).


Installation
------------

The latest stable release (and required dependencies) can be installed from PyPI:

    pip install seaborn

It is also possible to include optional statistical dependencies (only relevant for v0.12+):

    pip install seaborn[stats]

Seaborn can also be installed with conda:

    conda install seaborn

Note that the main anaconda repository lags PyPI in adding new releases, but conda-forge (`-c conda-forge`) typically updates quickly.

Citing
------

A paper describing seaborn has been published in the [Journal of Open Source Software](https://joss.theoj.org/papers/10.21105/joss.03021). The paper provides an introduction to the key features of the library, and it can be used as a citation if seaborn proves integral to a scientific publication.

Testing
-------

Testing seaborn requires installing additional dependencies; they can be installed with the `dev` extra (e.g., `pip install .[dev]`).

To test the code, run `make test` in the source directory. This will exercise the unit tests (using [pytest](https://docs.pytest.org/)) and generate a coverage report.

Code style is enforced with `flake8` using the settings in the [`setup.cfg`](./setup.cfg) file. Run `make lint` to check. Alternately, you can use `pre-commit` to automatically run lint checks on any files you are committing: just run `pre-commit install` to set it up, and then commit as usual going forward.

Development
-----------

Seaborn development takes place on Github: https://github.com/mwaskom/seaborn

Please submit bugs that you encounter to the [issue tracker](https://github.com/mwaskom/seaborn/issues) with a reproducible example demonstrating the problem. Questions about usage are more at home on StackOverflow, where there is a [seaborn tag](https://stackoverflow.com/questions/tagged/seaborn).

<div align="center">
  <img src="https://raw.githubusercontent.com/scikit-learn/scikit-learn/main/doc/logos/scikit-learn-logo.png"><br>
</div>

  :target: https://scikit-learn.org/

**scikit-learn** is a Python module for machine learning built on top of
SciPy and is distributed under the 3-Clause BSD license.

The project was started in 2007 by David Cournapeau as a Google Summer
of Code project, and since then many volunteers have contributed. See
the `About us <https://scikit-learn.org/dev/about.html#authors>`__ page
for a list of core contributors.

It is currently maintained by a team of volunteers.

Website: https://scikit-learn.org

Installation
------------

Dependencies
~~~~~~~~~~~~

scikit-learn requires:

- Python (>= |PythonMinVersion|)
- NumPy (>= |NumPyMinVersion|)
- SciPy (>= |SciPyMinVersion|)
- joblib (>= |JoblibMinVersion|)
- threadpoolctl (>= |ThreadpoolctlMinVersion|)

=======

**Scikit-learn 0.20 was the last version to support Python 2.7 and Python 3.4.**
scikit-learn 1.0 and later require Python 3.7 or newer.
scikit-learn 1.1 and later require Python 3.8 or newer.

Scikit-learn plotting capabilities (i.e., functions start with ``plot_`` and
classes end with "Display") require Matplotlib (>= |MatplotlibMinVersion|).
For running the examples Matplotlib >= |MatplotlibMinVersion| is required.
A few examples require scikit-image >= |Scikit-ImageMinVersion|, a few examples
require pandas >= |PandasMinVersion|, some examples require seaborn >=
|SeabornMinVersion| and plotly >= |PlotlyMinVersion|.

User installation
~~~~~~~~~~~~~~~~~

If you already have a working installation of numpy and scipy,
the easiest way to install scikit-learn is using ``pip``::

    pip install -U scikit-learn

or ``conda``::

    conda install -c conda-forge scikit-learn

The documentation includes more detailed `installation instructions <https://scikit-learn.org/stable/install.html>`_.


Changelog
---------

See the `changelog <https://scikit-learn.org/dev/whats_new.html>`__
for a history of notable changes to scikit-learn.

Development
-----------

We welcome new contributors of all experience levels. The scikit-learn
community goals are to be helpful, welcoming, and effective. The
`Development Guide <https://scikit-learn.org/stable/developers/index.html>`_
has detailed information about contributing code, documentation, tests, and
more. We've included some basic information in this README.

Important links
~~~~~~~~~~~~~~~

- Official source code repo: https://github.com/scikit-learn/scikit-learn
- Download releases: https://pypi.org/project/scikit-learn/
- Issue tracker: https://github.com/scikit-learn/scikit-learn/issues

Source code
~~~~~~~~~~~

You can check the latest sources with the command::

    git clone https://github.com/scikit-learn/scikit-learn.git

Contributing
~~~~~~~~~~~~

To learn more about making a contribution to scikit-learn, please see our
`Contributing guide
<https://scikit-learn.org/dev/developers/contributing.html>`_.

Testing
~~~~~~~

After installation, you can launch the test suite from outside the source
directory (you will need to have ``pytest`` >= |PyTestMinVersion| installed)::

    pytest sklearn

See the web page https://scikit-learn.org/dev/developers/contributing.html#testing-and-improving-test-coverage
for more information.

    Random number generation can be controlled during testing by setting
    the ``SKLEARN_SEED`` environment variable.

Submitting a Pull Request
~~~~~~~~~~~~~~~~~~~~~~~~~

Before opening a Pull Request, have a look at the
full Contributing page to make sure your code complies
with our guidelines: https://scikit-learn.org/stable/developers/index.html

Project History
---------------

The project was started in 2007 by David Cournapeau as a Google Summer
of Code project, and since then many volunteers have contributed. See
the `About us <https://scikit-learn.org/dev/about.html#authors>`__ page
for a list of core contributors.

The project is currently maintained by a team of volunteers.

**Note**: `scikit-learn` was previously referred to as `scikits.learn`.

Help and Support
----------------

Documentation
~~~~~~~~~~~~~

- HTML documentation (stable release): https://scikit-learn.org
- HTML documentation (development version): https://scikit-learn.org/dev/
- FAQ: https://scikit-learn.org/stable/faq.html

Communication
~~~~~~~~~~~~~

- Mailing list: https://mail.python.org/mailman/listinfo/scikit-learn
- Gitter: https://gitter.im/scikit-learn/scikit-learn
- Logos & Branding: https://github.com/scikit-learn/scikit-learn/tree/main/doc/logos
- Blog: https://blog.scikit-learn.org
- Calendar: https://blog.scikit-learn.org/calendar/
- Twitter: https://twitter.com/scikit_learn
- Twitter (commits): https://twitter.com/sklearn_commits
- Stack Overflow: https://stackoverflow.com/questions/tagged/scikit-learn
- Github Discussions: https://github.com/scikit-learn/scikit-learn/discussions
- Website: https://scikit-learn.org
- LinkedIn: https://www.linkedin.com/company/scikit-learn
- YouTube: https://www.youtube.com/channel/UCJosFjYm0ZYVUARxuOZqnnw/playlists
- Facebook: https://www.facebook.com/scikitlearnofficial/
- Instagram: https://www.instagram.com/scikitlearnofficial/
- TikTok: https://www.tiktok.com/@scikit.learn

Citation
~~~~~~~~

If you use scikit-learn in a scientific publication, we would appreciate citations: https://scikit-learn.org/stable/about.html#citing-scikit-learn
