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

## Version

The installed version of Telegram CLI is the latest one from the [GitHub repository](https://github.com/vysheng/tg), which currently is **1.4.1**.

## Note

This image lets you to start the Telegram CLI yourself.

If you want to be taken directly into the interactive Telegram CLI command-line, you can use, for example, [frankwolf/telegram-cli](https://hub.docker.com/r/frankwolf/telegram-cli/).

## Docker Hub

This image is on Docker Hub as [weibeld/ubuntu-telegram-cli](https://hub.docker.com/r/weibeld/ubuntu-telegram-cli/).
