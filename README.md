# Docker composition of Jira Software/Code

## How to set up

Clone repository

    git clone git@github.com:EvilFreelancer/docker-compose-jira.git

Switch work directory to root of project

    cd docker-compose-jira

Copy composition config from example

    cp docker-compose.yml.dist docker-compose.yml

Run composition

    docker-compose up -d

Add DNS records to your `/etc/hosts` file

    sudo nano /etc/hosts

Insert lines

    127.0.0.1 core
    127.0.0.1 software

Then save changes

After that, if you'll open http://software in your browser, you'll see
Jira Software installation page, and if http://core then Jira Core, respectively.

By the way, mounting the directory does not work on Windows and MacOS X,
so I strongly recommend that you configure everything on Linux, for example on [Ubuntu Linux](https://ubuntu.com/).

Good luck!

## Links

* https://www.youtube.com/watch?v=es9PJl_3RDw - Original video instruction (on Russian language) about this project with additional details
