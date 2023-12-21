![Maintained by Hassan](https://img.shields.io/badge/maintained%20by-Hassan.com-blue)


# Certbot

Generate and renew SSL certificate using `certbot` and `Let's Encrypt` based on DNS names (Route53).

## Requirements

* AWS `access` and `secret` keys
* Domain(s) managed by AWS route 53
* `Python >= 3.7`

## Install

* `pip install pipenv`
* `pipenv install`

## Usage

* Create a new file (`.env`) based on `env.template` file
* In file you created (`.env` file), add your AWS `access`, `secret` keys, replace `DOMAIN` value with yours and save it
* Run `pipenv run ./generate.sh` command for generating SSL certificates
* You will find all generated certificates in `~/local/letsencrypt/live/[DOMAIN_NAME]` path.

