# Quick install

Installing Odoo 14 with one command.

(Supports multiple Odoo instances on one server)

Install [docker](https://docs.docker.com/get-docker/) and [docker-compose](https://docs.docker.com/compose/install/) yourself, then run:


``` bash
curl -s https://ghproxy.com/https://raw.githubusercontent.com/zhengr/docker-odoo-14/master/run.sh | sudo bash -s odoo-one 10014 20014
```

``` bash
curl -s https://raw.githubusercontent.com/zhengr/docker-odoo-14/master/run.sh | sudo bash -s odoo-one 10014 20014
```

to set up first Odoo instance @ `localhost:10014` (default master password: `######`)

and

``` bash
curl -s https://ghproxy.com/https://raw.githubusercontent.com/zhengr/docker-odoo-14/master/run.sh | sudo bash -s odoo-two 11014 21014
```

``` bash
curl -s https://raw.githubusercontent.com/zhengr/docker-odoo-14/master/run.sh | sudo bash -s odoo-two 11014 21014
```

to set up another Odoo instance @ `localhost:11014` (default master password: `######`)

Some arguments:
* First argument (**odoo-one**): Odoo deploy folder
* Second argument (**10014**): Odoo port
* Third argument (**20014**): live chat port

If `curl` is not found, install it:

``` bash
$ sudo apt-get install curl
# or
$ sudo yum install curl
```
