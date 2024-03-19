# Dockerizing Ruby Tutorial

### RESOURCES
[dockerizing-ruby](https://github.com/TomFern/dockerizing-ruby/tree/master)

### INSTALL

#### install RVM
[ubuntu_rvm](https://github.com/rvm/ubuntu_rvm)
```
sudo apt-get install software-properties-common

sudo apt-add-repository -y ppa:rael-gc/rvm
sudo apt-get update
sudo apt-get install rvm

sudo usermod -a -G rvm $USER

rvm install ruby

```

[![Build Status](https://tomfern.semaphoreci.com/badges/dockerizing-ruby/branches/master.svg?key=a7410866-1910-44a0-8ef2-624794abd900)](https://tomfern.semaphoreci.com/projects/dockerizing-ruby)

[How To Install Ruby on Rails with RVM on Ubuntu 20.04](https://www.digitalocean.com/community/tutorials/how-to-install-ruby-on-rails-with-rvm-on-ubuntu-20-04)
- [Initial Server Setup with Ubuntu 20.04
](https://www.digitalocean.com/community/tutorials/initial-server-setup-with-ubuntu-20-04)

```
sudo su root  

adduser rubyuser
- arjuna11

usermod -aG sudo rubyuser
```

### Create DB

```
rvm install ruby-3.1.2

source ~/.rvm/scripts/rvm
type rvm | head -n 1

rvm --default use ruby-3.1.2

bin/rails db:create
```

## Local setup

Prepare environment, for dev version you can use the example environment:

```bash
$ cp env-example .env
```

Start the server:

```bash
$ docker-compose up --build
```

Browse http://localhost:8020

## License

MIT License

Copyright (c) 2022 Rendered Text

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.



