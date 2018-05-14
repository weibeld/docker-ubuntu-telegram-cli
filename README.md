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

The main mode of Telegram CLI has an interactive command-line. The available commands in this command-line are listed [here](https://github.com/vysheng/tg#supported-commands)

## Version

The installed version of [telegram-cli](https://github.com/vysheng/tg) is the latest one from the GitHub repository, which currently is **1.4.1**.

## Note

This image lets you to start the Telegram CLI yourself.

If you want to be taken directly into the interactive Telegram CLI command-line, use [frankwolf/telegram-cli](https://hub.docker.com/r/frankwolf/telegram-cli/) instead.
