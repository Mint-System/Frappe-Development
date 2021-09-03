Frappe Development
==================

The Mint System Frappe development environment.

This projects provides a highly opinionated way to develop Frappe sites and apps.

## Requirements

Common:

* bash/zsh alias `task='./task'` with optional [completion](https://github.com/janikvonrotz/dotfiles/blob/master/oh-my-zsh-completions/_task)

Docker:

* [Docker](https://docs.docker.com/engine/install/) and [Docker Compose](https://docs.docker.com/compose/)

Native:

* Install Python 3.6+ with [pyenv](https://github.com/pyenv/pyenv-installer)
* Install Node.js 12+ with [n](https://github.com/tj/n)
* Install yarn 1.12+: `npm install -g yarn`
* [wkhtmltopdf](https://wkhtmltopdf.org/): `sudo apt install wkhtmltopdf`

## Usage

Clone this repository.

```bash
git clone https://github.com/Mint-System/Frappe-Development.git
cd Frappe-Development
```

See command overivew with `task help` or read [task](task.md).

Check if required tools are installed.

```bash
task version
```

### Native

Start Docker database containers.

```bash
task start db
```

Install Frappe dependencies.

```bash
task install
```

Install app.

```bash
task install-app uppsala https://gitlab.com/hfmts/uppsala.git
```

Start frappe development server.

```bash
task start native
```

### Docker

Start Docker containers.

```bash
task start all
```

Install app.

```bash
task docker-install-app uppsala https://gitlab.com/hfmts/uppsala.git
```