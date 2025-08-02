# 🤖 CSSE3200 Discord Bot

## 📚 Description

This project is a custom discord bot for CSSE3200 which will help students
 during the course.

### ✨ Features

- Auto role management  
- Helpful integration with the studio's github repo
- More to come - if you think of any, lemme know

## Authors

- [Lucas Hicks](https://github.com/lucashicks1)

## 🚀 Getting Started

### Prerequisites

- Python 3.13 (uv can install this in its our venv for you)
- [`uv`](https://github.com/astral-sh/uv#installation) installed

### Installation/Setup

- Make sure to set all required environment variables, see `.env.example` and `src/csse3200bot/config.py`.

- For dev, `docker compose up` will probably be your go to.
- Otherwise, you can use the provided Dockerfile to build the image for the bot and host it as you like.


### Deployment
- Currently GitHub Actions is used to build the docker image and then publish that to a container registry. I then have [fluxcd](https://fluxcd.io/) setup on my homelab to automatically update the k8s manifest with the new container image.
