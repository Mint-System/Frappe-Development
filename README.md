Frappe Development
==================

The Mint System Frappe development environment.

This projects provides a highly opinionated way to develop Frappe sites and apps. It provides three ways to run Frappe.

* **Native**: Frappe is downloaded to the project folder. Use bench natively to run the development server.
* **Docker Production**: This approach uses Docker Compose to the setup a Frappe project as it would be running in production.
* **Docker Development**: The production setup is complex. Use this approach run Frappe Bench within a container.

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

### Docker Development

Start Docker development containers.

```bash
task start dev
```

Install Frappe and setup site.

```bash
task docker-install-dev
```

Start the Docker development server.

```bash
task start bench
```