# Roni Setiawan - Portofolio

## Special Thanks (Giving wonderful framework & template)

- [**Mkdocs**, click here to see more detail!](https://www.mkdocs.org/)
- [**Mkdocs Material**, click here to see more detail!](https://squidfunk.github.io/mkdocs-material/)

> This project was created to show an easy way to create a web using `frameworks` & `theme`. The **main programming language** used is `Markdown` and it's quite easy to **publish our web** to a server using `GitLab Page` _(using `.gitlab-ci.yml` called as **GitLab CI Pipeline**)_ and/or `GitHub Page` _(using `.github/workflows/ci.yml` called as **GitHub Workflow**)_.

## Requirement Tools

|  Name  |   Version  |
|  :----------  |  :---------  |
|  **Python**  |   [**Minimum `3.0.0`**, click here!](https://www.python.org/downloads/)  |
|  **Python PIP**  |   [**`LTS/Stable`**, click here!](https://pip.pypa.io/en/stable/installation/)  |
|  **Git**  |   [**`LTS/Stable`**, click here!](https://git-scm.com/downloads)  |
|  **Editor/IDE**  |   _Compatible for view `markdown` text_. <br></br> Example: `Visual Studio Code` / _other editor you are familiar_  |

Validation your installation using **Command Prompt / Terminal**.

1. Validate `python` installation

    a. **OS Windows**
    ```bash
    python --version
    ```

    b. **OS Unix (Linux/Mac)**
    ```bash
    python3 --version
    ```

    > _Sample output `Python 3.8.9`_

2. Validate `pip` installation

    a. **OS Windows**
    ```bash
    pip --version
    ```

    b. **OS Unix (Linux/Mac)**
    ```bash
    pip3 --version
    ```

    > _Sample output `pip 23.1.2 from .../Python/3.8/lib/python/site-packages/pip (python 3.8)`_

3. Validate `git` installation

    a. **OS Windows**
    ```bash
    git --version
    ```

    b. **OS Unix (Linux/Mac)**
    ```bash
    git --version
    ```

    > _Sample output `git version 2.32.1`_

## Environment Preparation

1. Install `python library` needed by running command line below using **Command Prompt / Terminal**

    a. **OS Windows**
    ```bash
    pip install -r requirement.txt
    ```

    b. **OS Unix (Linux/Mac)**
    ```bash
    pip3 install -r requirement.txt
    ```

2. Validate `python library` installation

    a. **OS Windows**
    ```bash
    pip freeze

    pip list
    ```

    b. **OS Unix (Linux/Mac)**
    ```bash
    pip3 freeze

    pip3 list
    ```

    > Sample output 
    > ```bash
    > mkdocs==1.3.1
    > mkdocs-material==8.5.2
    > mkdocs-material-extensions==1.0.3
    > ```

3. Validate `mkdocs` command

    ```bash
    mkdocs --version

    mkdocs --help
    ```

    > If you find `command not found: mkdocs`, it's mean your `mkdocs` not setting up at **Environment Variable**. But don't worry if you not wanna setting up you can use other option command

    a. **OS Windows**
    ```bash
    python -m mkdocs --version
    
    python -m mkdocs --help
    ```

    b. **OS Unix (Linux/Mac)**
    ```bash
    python3 -m mkdocs --version
    
    python3 -m mkdocs --help
    ```

## How To Running?

1. Clone repository from **GitLab** / **GitHub** using `git` command

    ```
    git clone <<url_repository>>.git
    ```

    |  Name  |   URL Repository  |
    |  :----------  |  :---------  |
    |  **GitLab**  |   [**https://gitlab.com/setiawanroni120/portofolio**](https://gitlab.com/setiawanroni120/portofolio.git)  |
    |  **GitHub**  |   [**https://github.com/setiawanroni120/portofolio**](https://github.com/setiawanroni120/portofolio.git)  |

2. Change into directory `portofolio`

    ```
    cd portofolio
    ```

3. Running at local using `mkdocs` command

    ```
    mkdocs serve

    python -m mkdocs serve

    python3 -m mkdocs serve
    ```

> **Default** project will running at `localhost:8000` atau `127.0.0.1:8000`

## How To Build & Deploy?

1. Build this project using command `mkdocs`

    ```
    mkdocs build --site-dir public

    python -m mkdocs build --site-dir public

    python3 -m mkdocs build --site-dir public
    ```

2. Deploy **all content under directory `public`** into web server you have

    |  Sample Web Server  |
    |  :----------  |
    |  Apache  |
    |  Tomcat  |
    |  IIS  |
    |  Nginx  |

You can also deploy your **Mkdocs Project** into `GitLab Page` or `GitHub Page`

a.  Using **Gitlab CI Pipeline** to deploy into `GitLab Page`. **[See detail `.gitlab-ci.yml`](/.gitlab-ci.yml)**

b.  Using **GitHub Workflow** to deploy into `GitHub Page`. **[See detail `.github/workflows/ci.yml`](/.github/workflows/ci.yml)**