# Profitware Education

[![CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by/4.0/)


## Linux, Git and Vagrant

You are expected to create three virtual machines, setup network and services on each of them. The whole stand (including specified services) should be accessible from your local machine using Web Browser via Reverse Proxy according to the image below. [Vagrant](https://www.vagrantup.com/) and Vagrantfile description should be used to setup the whole stand.

Source code should be put into your corporate Git repository except files larger than 5mb. Start by cloning this repository to your local machine and use this particular branch and commit for your results.

1. Reverse Proxy. Machine name: education-reverse-proxy. Should contain [NGINX](https://nginx.org/) reverse proxy web server which gives access to the Application (below) and Database Admin Interface (below).
2. Application. Machine name: education-application. Should contain [PostgreSQL](https://www.postgresql.org/) database and [WildFly](https://www.wildfly.org/) application server with arbitrary WAR-application (capable of talking to PostgreSQL via JDBC) deployed to the server.
3. Database Admin Interface. Machine name: education-database-admin. Should contain [pgAdmin](https://www.pgadmin.org/) to ensure administration capabilities for PostgreSQL (above).

<img src="/img/education-linux-git-and-vagrant.png"
    alt="Education: Linux, Git and Vagrant Diagram" />


## License

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
