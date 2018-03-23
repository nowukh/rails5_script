# Vagrant Rails 5 (VirtualBox only)

This vagrant box contains the necessary for Ruby on Rails development using PostgreSQL as main database. But other databases can also be installed, the configuration for MySQL and MongoDB is already included in the forwarded ports. The provision script is based on [rails-install-ubuntu.sh](https://raw.githubusercontent.com/railsgirls/installation-scripts/master/rails-install-ubuntu.sh).

### Included Packages

* rvm **>=** 1.29
* ruby **>=** 2.4.1
* bundler **>=** 1.15
* rails **>=** 5.0.6
* nodejs **>=** 6.11
* sqlite **>=** 3.11
* imagemagick **>=** 6.8.9
* heroku CLI **>=** 6.13

### Forwarded Ports

| Service | Guest | Host |
| :---          | :---:    | ---:  |
| rails         | 3000     | 3000  |
| rack          | 9292     | 9292  |
| sinatra       | 4567     | 4567  |
| mailcatcher   | 1080     | 1080  |
| jasmine       | 8888     | 8888  |
| mysql         | 3306     | 3306  |
| node          | 1234     | 1234  |
| postgresql    | 5432     | 5432  |
| redis         | 6379     | 6379  |
| elasticsearch | 9200     | 9200  |
| mongodb       | 27017    | 27017 |
| apache/nginx  | 80       | 8080  |

### Usage

Just download the `Vagrantfile` and `bootstrap.sh` on the root folder on your app, and execute the commands:

```shell
vagrant up
vagrant ssh
```

### Requierements

* Vagrant
* VirtualBox