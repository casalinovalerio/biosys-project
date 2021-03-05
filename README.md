# Biometric Systems Project

![GitHub](https://img.shields.io/github/license/casalinovalerio/biosys-project)
![GitHub deployments](https://img.shields.io/github/deployments/casalinovalerio/biosys-project/github-pages?label=gh-pages)

## Members

- Shaahin ([@shaahin-sabeti](https://github.com/shaahin-sabeti))
- Tobi ([@TobMTV](https://github.com/TobMTV))
- Valerio ([@5amu](https://github.com/5amu))

## Introduction

This student group project is assigned for the [Biometric Systems course](https://sites.google.com/a/di.uniroma1.it/biometric-systems/) of the [MSc in Cybersecurity](https://cybersecurity.uniroma1.it/home) @ [Sapienza Università di Roma](https://www.uniroma1.it/en/). Our group had to decide, design and realize an authentication system aggregating software and deploying our solutions with the aim of **testing** its performance in the end.

We decided to use the following tools and software:

* [@ageitgey/face_recognition](https://github.com/ageitgey/face_recognition) Python API running in a Docker.
* [Bigchaindb](https://bigchaindb.com) as Blockchain database running in a Docker.
* [Ubuntu Server 18.04 LTS](https://ubuntu.com/download/server) as OS to deploy our API server running on a VPS.
* [Digital Ocean](https://www.digitalocean.com/) as platform to rent our VPS.
* [Github Pages](https://pages.github.com) as web interface to demonstrate our method.
* [LaTex](https://www.latex-project.org/) to write our presentation.

## Steps to reproduce

Clone the repo in your db-server, api-server and on the pc where you want to work on the website:

```bash
git clone "https://github.com/casalinovalerio/biosys-project.git"
```

On db-server:

```bash
# You'll need Docker installed
./install.sh db
```

On api-server:

```bash
# Default is /var/www/html
./install.sh api /path/to/webroot
```

On your pc:

```bash
# Both args are optional, if no arg is supplied it will print the usage
./install.sh pc -w /path/to/web-devel-folder -t /path/to/presentation/folder
```

## Get the presentation

```bash
git clone "https://github.com/casalinovalerio/biosys-project.git" \
	&& cd biosys-project \
	&& ./get-presentation.sh
```

Your presentation is in the same folder with name `bs-presentation.pdf`.

Or just click here: [https://git.io/JvGRm](https://git.io/JvGRm)
