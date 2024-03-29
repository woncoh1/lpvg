# Linux, Python, Vim and Git
Timeless, muscle-memory tools inspired by [Mike Levin](https://github.com/miklevin). The so-called canonical technologies responsible for covering 80 percent of all use cases using only 20 percent of investable effort (the 80-20 rule). Free/libre infrastructure that is disruption-proof and obsolescence-resistant.

- Linux: operating system
- Python: programming language
- Vim: text editor (IDE)
- Git: version control

## Linux
- Windows: [WSL](https://docs.microsoft.com/en-us/windows/wsl/)
- MacOS: [Lima](https://github.com/lima-vm/lima)

## Python
- [Python Management System](https://ealizadeh.com/blog/guide-to-python-env-pkg-dependency-using-conda-poetry)
    - [`conda`](https://docs.conda.io/en/latest/): environment manager
        - [Conda Guide](https://towardsdatascience.com/a-guide-to-conda-environments-bc6180fc533)
            - [conda environment.yml + pip requirements.txt](https://stackoverflow.com/q/35245401)
        - [Miniconda vs Anaconda](https://www.reddit.com/r/Python/comments/lvr85n/i_want_to_use_python_commercially_for_free_is/)
        - [Miniforge vs Miniconda](https://stackoverflow.com/q/60532678)
            - [conda-forge vs conda](https://stackoverflow.com/q/39857289)
        - [**Mambaforge**](https://github.com/conda-forge/miniforge/#mambaforge) ([Miniforge](https://github.com/conda-forge/miniforge/))
            - [Micromamba](https://github.com/mamba-org/mamba#micromamba) ([Mamba](https://github.com/mamba-org/mamba))
    - [`pip`](https://pip.pypa.io/en/stable/): package installer
    - [`poetry`](https://python-poetry.org/): dependency resolver

## Vim
- [Neovim](https://neovim.io/)

### [Emacs](https://www.reddit.com/r/emacs/comments/6s6uyr/emacs_evil_or_spacemacs/)
- [Evil](https://github.com/emacs-evil/evil)
- [Spacemacs](https://www.spacemacs.org/)
- [Doom Emacs](https://github.com/hlissner/doom-emacs)

### Jupyter
- Conda Environment
    - [The Usual Way](https://stackoverflow.com/a/53546634)
    - [The Easy Way](https://towardsdatascience.com/get-your-conda-environment-to-show-in-jupyter-notebooks-the-easy-way-17010b76e874)
- Docker Image
    - [Jupyter Docker Stacks](https://github.com/jupyter/docker-stacks)
    - [Saturn Cloud Images](https://github.com/saturncloud/images)

Mastering Vim takes a while and effort, so meanwhile we use JupyterLab for literate and exploratory programming. The desktop (stand-alone) version of JupyterLab is particularly useful since there is no need to use a web browser and open a new terminal window for Jupyter server.

- [JupyterLab Desktop](https://github.com/jupyterlab/jupyterlab-desktop)
- [JupyterLite](https://jupyterlite.readthedocs.io/en/latest/)
- [Saturn Cloud](https://saturncloud.io/)

### JupyterLab Desktop (Windows)
1. Install [mambaforge](https://github.com/conda-forge/miniforge)
    - Add conda to PATH environment variable
3. Install [JupyterLab Desktop](https://github.com/jupyterlab/jupyterlab-desktop)
4. If you use OneDrive from non-English speaking country, follow [this link](https://support.microsoft.com/en-us/topic/operation-to-change-a-personal-folder-location-fails-in-windows-ffb95139-6dbb-821d-27ec-62c9aaccd720) to change the name of the "personal" folder to "Documents"
5. Run PowerShell and execute the following commands:
   ```
   conda init powershell
   conda create -n py310 python=3.10 jupyterlab
   ```
6. Run JupyterLab Desktop, and set the default kernel path to `mambaforge/envs/py310/python.exe`
7. Enjoy

## Git

### GitHub
- Badges
    - [Shields](https://shields.io/)
    - [Badgen](https://badgen.net/)

## TODO
- Hardware
    - [QNAP](https://www.qnap.com)
    - [Raspberry Pi](https://www.raspberrypi.org/)
- Nix (Multics, Unix, Minix, Linux, etc)
    - [Minix](https://www.minix3.org/)
        - [Arch](https://archlinux.org/)
        - [Gentoo](https://www.gentoo.org/)
    - [Tiny Core Linux](http://tinycorelinux.net/)
        - [QEMU](https://www.qemu.org/)
    - [LXD](https://linuxcontainers.org/lxd/introduction/)
    - [systemd](https://systemd.io/)
- HTML
    - [htmx](https://htmx.org/)
- Regex
    - [Awesome Regex](https://github.com/aloisdg/awesome-regex)
- SQL
    - [SQLite](https://www.sqlite.org/)
    - [PostgreSQL](https://www.postgresql.org/)
- Python
    - [Reference](https://docs.python.org/3/reference/)
    - [Tutorial](https://docs.python.org/3/tutorial/)
        - [Hitchhiker's Guide](https://docs.python-guide.org/)
    - [Standard Library](https://docs.python.org/3/library/)
        - [Built-in Functions](https://docs.python.org/3/library/functions.html)
    - [Packaging User Guide](https://packaging.python.org/en/latest/)
        - [Book](https://py-pkgs.org/)
        - [src](https://github.com/pypa/packaging.python.org/issues/320)
        - [src2](https://hynek.me/articles/testing-packaging/)
        - [sampleproject](https://github.com/pypa/sampleproject)
        - [sampleproject: attrs](https://github.com/python-attrs/attrs)
        - [sampleproject: flask](https://github.com/pallets/flask)
        - [pyscaffold](https://github.com/pyscaffold/pyscaffold/)
        - [pyscaffold: streamlit](https://github.com/pyscaffold/pyscaffold/)
        - [pip](https://pip.pypa.io/en/stable/)
        - [Wheel](https://pythonwheels.com/)
            - [Tutorial](https://realpython.com/python-wheels/)
        - [Setuptools](https://setuptools.pypa.io/en/latest/)
    - [Pandas](https://pandas.pydata.org/)
        - [Docs](https://pandas.pydata.org/docs/)
        - [Book](https://github.com/wesm/pydata-book)
        - [Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/03.00-introduction-to-pandas.html)
        - [Beyond Pandas](https://github.com/astrojuanlu/talk-dataframes)
            - [lbis](https://ibis-project.org/docs/dev/)
            - [Polars](https://www.pola.rs/)
            - [pyarrow](https://arrow.apache.org/docs/python/index.html)
            - [datafusion](https://arrow.apache.org/datafusion/specification/roadmap.html)
    - [fast.ai](https://www.fast.ai/)
    - [nbdev](https://nbdev.fast.ai/)
    - [nbprocess](https://github.com/fastai/nbprocess)
    - [sqlitedict](https://github.com/RaRe-Technologies/sqlitedict)
    - [re](https://docs.python.org/3/library/re.html)
    - [rich](https://github.com/Textualize/rich)
    - [tabulate](https://github.com/astanin/python-tabulate)
    - [PrettyTable](https://github.com/jazzband/prettytable)
    - [tabulate](https://github.com/astanin/python-tabulate)
    - [stockholm](https://github.com/kalaspuff/stockholm)
    - [docs](https://realpython.com/documenting-python-code/#documentation-tools-and-resources)
        - [markdown](https://www.markdownguide.org/) (Web)
        - [reStructuredText](https://docutils.sourceforge.io/rst.html) (Python)
            - [Sphinx](https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html)
            - [Write the Docs](https://www.writethedocs.org/guide/writing/reStructuredText/)
        - [myST](https://myst-parser.readthedocs.io/en/latest/) (Jupyter)
    - [Sphinx](https://www.sphinx-doc.org/en/master/)
        - [Furo](https://github.com/pradyunsg/furo)
        - [myST](https://myst-parser.readthedocs.io/en/latest/)
        - [Material](https://bashtage.github.io/sphinx-material/)
        - MkDocs
            - [httpx](https://github.com/encode/httpx/discussions/1220)
            - [Hacker News](https://news.ycombinator.com/item?id=27283521)
    - Configuration
        - [pyproject.toml](https://snarky.ca/what-the-heck-is-pyproject-toml/)
        - [requirements.txt](https://towardsdatascience.com/requirements-vs-setuptools-python-ae3ee66e28af)
        - [environment.yml](https://carpentries-incubator.github.io/introduction-to-conda-for-data-scientists/04-sharing-environments/index.html)
        - [setup.py vs setup.cfg](https://towardsdatascience.com/setuptools-python-571e7d5500f2)
        - [setup.ini](https://docs.python.org/3/library/configparser.html)
    - Logging
        - [logging](https://docs.python.org/3/library/logging.html)
        - [loguru](https://github.com/Delgan/loguru)
    - [Dependency Injector](https://python-dependency-injector.ets-labs.org/)
    - [Pendulum](https://pendulum.eustace.io/)
        - [Tutorial](https://towardsdatascience.com/pendulum-one-of-the-most-useful-python-libraries-you-have-ever-seen-e2ecc365c8c0)
    - [Tornado](https://www.tornadoweb.org/en/stable/)
    - Visualize Stream
        - [streamz](https://streamz.readthedocs.io/en/latest/plotting.html)
        - [HoloViews](https://holoviews.org/user_guide/Streaming_Data.html)
        - [Panel](https://colab.research.google.com/github/justinbois/bootcamp/blob/gh-pages/2021/lessons/l29_dashboards.ipynb)
- Lisp
    - Python:Lisp=Yang:Yin
    - Emacs
- Notebook
    - [JupyterLab Desktop](https://github.com/jupyterlab/jupyterlab-desktop)
    - [Data Science Notebooks](https://datasciencenotebook.org/)
- Figure
    - https://r-graph-gallery.com/
- Table
    - https://www.ag-grid.com/
    - https://perspective.finos.org/
    - https://datatables.net/
- Misc
    - [Awesome Awesomeness](https://github.com/bayandin/awesome-awesomeness) 
    - [ZeroMQ](https://zeromq.org/)
    - [FreeCAD](https://www.freecadweb.org/)
    - [Microsoft Playwright](https://github.com/microsoft/playwright)
    - [GNU Screen](https://www.gnu.org/software/screen/)
        - [tmux](https://github.com/tmux/tmux/wiki)
    - [Google Fonts](https://fonts.google.com/)
        - [Google Icons](https://fonts.google.com/icons)
        - [Bootstrap Icons](https://icons.getbootstrap.com/)
    - [Adblock Plus](https://namu.wiki/w/Adblock%20Plus)
    - [Customize GitHub's code font](https://alexsaveau.dev/blog/tips/github/customize-github-code-font)
    - [Serverless Computing](https://en.wikipedia.org/wiki/Serverless_computing)
    - [API Throttling and Rate Limiting](https://beabetterdev.com/2020/12/12/what-is-api-throttling-and-rate-limiting/)
    - [Baeldung Linux](https://www.baeldung.com/linux/)
    - [Boolean Biotech](http://blog.booleanbiotech.com/)
    - [Mail Avenger](https://www.mailavenger.org/)
    - [Dark](https://darklang.com/)
    - [FinRL](https://medium.datadriveninvestor.com/finrl-meta-a-universe-of-near-real-market-en-vironments-for-data-driven-financial-reinforcement-e1894e1ebfbd)
    - [ArchiveBox](https://archivebox.io/)
    - [curlconverter](https://curlconverter.com/)
    - [Epoch Converter](https://www.epochconverter.com/)
