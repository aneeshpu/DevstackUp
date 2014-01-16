# Devstack with Vagrant

## Features

* 3GB Vagrant VM
* Horizon forwarded to `localhost:8080`
* Verbose mode and logging enabled

## Usage


### Step 1: [Install Vagrant](http://vagrantup.com/v1/docs/getting-started/index.html)

### Step 2: `git clone git://github.com/jogo/DevstackUp.git`

### Step 3 Vagrant up: `cd DevstackUp; vagrant up`

### Step 4: Vagrant ssh

#### Tests:

* `~/devstack/exercise.sh`
* `cd /opt/stack/tempest ;  nosetests --attr=type=smoke tempest`

#### Notes:

* If you have another box named `precise`, you must remove it first with `vagrant box remove precise`
* To build, vagrant box that has most of the devstack dependencies pre-installed:
  * `cd build_box`
  * `./build.sh`
