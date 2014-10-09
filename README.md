# Use

To use this all you need to do is install or have the package installed and
then inside a phablet-shell do

    sudo network-test-session start

Do all the required network testing, once done

    sudo network-test-session stop

Stopping will collect the logs and print out their location, at any time logs
can be collected by running

    sudo network-test-session collect

this command will also output the location of the tar'ed up logs.

# Building

If you want to build this package, just run

    debuild

# Installing

## Ubuntu Touch

This package is built in a PPA already, you can install the latest from there
by executing the following as root:

    mount -o remount,rw /
    echo "deb http://ppa.launchpad.net/phablet-team/testtools/ubuntu utopic main" > /etc/apt/sources.list.d/phablet-team-testools.list
    apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 5E51A24C
    apt update
    apt install network-test-session
    reboot
