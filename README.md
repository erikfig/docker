# Local Docker

This Docker service is used in my local environment to start the most common services used by me.

> This is for my personal use, if i could help i will be happy!
> Sorry for my english, i'm trying very hard

Tested in 

- [x] Fedora Linux
- [x] Windows 11 WSL2
- [x] MacOS

## Services available

 - postgres
 - rabbit
 - nats
 - redis
 - aws


## AWS

To configure AWS Service, add an alias to you terminal (`.zshrc` in my case):

```cli
alias aws="docker run --rm -ti -v ~/.aws:/root/.aws -v $(pwd):/aws amazon/aws-cli"
```

Reload your configurations (`source .zshrc` in my terminal or close all terminals and reopen).

Test:

```cli
aws --version
```

And configure:

```
aws configure
```

All informations can be found or generated in AWS Console > Your user (top-right) > Security Credentials.
