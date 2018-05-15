# Ubuntu Telegram CLI

Docker image with Ubuntu 16.04 and [telegram-cli](https://github.com/vysheng/tg) installed.

## Usage

Just run:

~~~bash
docker run -ti weibeld/ubuntu-telegram-cli
~~~

This takes you into a Bash session on Ubuntu in the `/root/tg` directory.

You can now run the Telegram CLI like this:

~~~bash
bin/telegram-cli --help
~~~

The main mode of the Telegram CLI consists of an interactive command-line. The usage of the commands available in this command-line are listed [here](https://github.com/vysheng/tg#supported-commands).

### Persist Authentication

By default, each time you run the Docker image and start the Telegram CLI, you have to type in your phone number and authenticate yourself with an SMS code.

The Telegram CLI saves this authentication information in the directory `/root/.telegram-cli`.

To persist this data across runs of the Docker image on your machine, you can use a Docker volume:

~~~bash
docker run -ti -v ubuntu-telegram-cli:/root/.telegram-cli weibeld/ubuntu-telegram-cli
~~~

In this way, when you run the Docker image another time, you can log in to your Telegram account without a verification SMS code.

*Note: you can list all Docker volumes with `docker volume ls`.*

## Version

The installed version of Telegram CLI is the latest one from the [GitHub repository](https://github.com/vysheng/tg), which currently is **1.4.1**.

## Note

This image lets you to start the Telegram CLI yourself.

If you want to be taken directly into the interactive Telegram CLI command-line, you can use, for example, [frankwolf/telegram-cli](https://hub.docker.com/r/frankwolf/telegram-cli/).

## Docker Hub

This image is on Docker Hub as [weibeld/ubuntu-telegram-cli](https://hub.docker.com/r/weibeld/ubuntu-telegram-cli/).
