# genhosts

genhosts - generate hosts file from /etc/hosts.d/*.conf

## Installation

    $ curl -O https://raw.github.com/kohkimakimoto/genhosts/master/genhosts
    $ chmod 755 genhosts
    $ sudo mv genhosts /usr/local/bin/

## Usage

Create separated hosts files.

    $ mkdir /etc/hosts.d
    $ cd /etc/hosts.d

Write hosts settings `hosts.conf`

    127.0.0.1   localhost localhost.localdomain localhost4 localhost4.localdomain4 devel.localdomain
    ::1         localhost localhost.localdomain localhost6 localhost6.localdomain6 devel.localdomain

Write another hosts settings `devel.hosts.conf`

    127.0.0.1   my.development.service.localdomain

Run `genhosts` command to generate `/etc/hosts`.

    $ genhosts

See `/etc/hosts`

    $ vim /etc/hosts








