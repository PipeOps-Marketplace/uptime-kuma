# uptime-kuma on PipeOps


A fancy self-hosted monitoring tool

[![Deploy on PipeOps](https://pub-a1fbf367a4cd458487cfa3f29154ac93.r2.dev/Default.png)](#)


![](https://user-images.githubusercontent.com/1336778/212262296-e6205815-ad62-488c-83ec-a5b0d0689f7c.jpg)


# Tags
Tag(s) 	Description
latest, 1, 1.*	latest stable - debian
debian, 1-debian, 1.*-debian	latest stable - debian
❌alpine, 1-alpine, 1.*-alpine	(❌Deprecated due to DNS issues) latest stable - alpine
beta, *-beta.*	Beta. New features preview or help to test. It could be unstable.
nightly*	development build, very unstable


# How to Use

## Docker

     # Create a volume
     docker volume create uptime-kuma

     # Start the container
     docker run -d --restart=always -p 3001:3001 -v uptime-kuma:/app/data --name uptime-kuma louislam/uptime-kuma:1

Uptime Kuma is now running on http://localhost:3001

Change Port and Volume

     docker run -d --restart=always -p <YOUR_PORT>:3001 -v <YOUR_DIR OR VOLUME>:/app/data --name uptime-kuma louislam/uptime-kuma:1

# Source Code or Non-Docker Installation

https://github.com/louislam/uptime-kuma
