Frappe Development
==================

The Mint System Frappe development environment.

This projects provides a highly opinionated way to develop Frappe sites and apps.

## Requirements

* [Docker](https://docs.docker.com/engine/install/) and [Docker Compose](https://docs.docker.com/compose/)
* Install Python 3.6+ with [pyenv](https://github.com/pyenv/pyenv)
* Install Node.js 12+ with [n](https://github.com/tj/n)
* Install yarn 1.12+: `npm install -g yarn`
* [wkhtmltopdf](https://wkhtmltopdf.org/): `sudo apt install wkhtmltopdf`
* bash/zsh alias: `task='./task'`

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

Init Frappe app.

```bash
task new-app demo
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

Install Frappe Docker dependencies.

```bash
task docker-install
```

Start Docker frappe development server.

```bash
task start docker
```