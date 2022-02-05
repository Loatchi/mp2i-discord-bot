<h1 align="center">MP2I</h1>
<h4 align="center">A Discord bot for MP2I server </h4>

<p align="center">
    <a href="https://github.com/prepas-mp2i/mp2i-discord-bot#overview">Overview</a> •
    <a href="https://github.com/prepas-mp2i/mp2i-discord-bot#softwares">Sofwares</a> •
    <a href="https://github.com/prepas-mp2i/mp2i-discord-bot#installation">Installation</a>
</p>

![GitHub top language: Python](https://img.shields.io/github/languages/top/prepas-mp2i/mp2i-discord-bot) &nbsp;
![Python3.9](https://img.shields.io/badge/python-3.9-red) &nbsp;
[![discord.py](https://img.shields.io/badge/discord-py-orange.svg)](https://github.com/Rapptz/discord.py) &nbsp;
![GitHub repo size](https://img.shields.io/github/repo-size/prepas-mp2i/mp2i-discord-bot) &nbsp;
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE) &nbsp;
![GitHub last commit (branch)](https://img.shields.io/github/last-commit/prepas-mp2i/mp2i-discord-bot) &nbsp;

## Overview

**MP2I** is a Discord bot adapted from [PyBoss](https://github.com/ajayat/pyboss) bot created by [Adridri](https://github.com/ajayat).

It provides somes features like:

- Roles selection
- Music player
- Custom commands (clear, profile ...)
- Moderation

## Softwares

**Python** <br>
It's required to have python 3.9 or more installed on your system.
[Download Python](https://www.python.org/downloads/)

**Docker** <br>
You can also use Docker to deploy the environment in one command.
[Get started with Docker](https://www.docker.com/get-started)

## Installation

First set variables in .env file:

```ini
DISCORD_TOKEN = <discord_bot_token>
# Can be development (More logs)
ENVIRONMENT = production
# Optional, a SQLite database will be created otherwise.
DATABASE_URL = mysql+mysqlconnector://user:password@host:port/database
# For YouTube API (optional).
API_DEVELOPER_KEY = <youtube_api_developer_key>
```

- ### Using Pipenv

Install `pipenv` dependencies:

```sh
python3 -m pip install pipenv
```

Now, you can create an empty `.venv` directory and running `pipenv`
It will install packages in the virtual environment (recommended).

```sh
pipenv install
```

Run the script `mp2i/__main__.py` or run `python3 -m mp2i`

- ### Using Docker

```sh
docker-compose up --build
```