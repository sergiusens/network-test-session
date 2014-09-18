# Use

To use this all you need to do is install or have the package installed and
then inside a phablet-shell do

    sudo netork-test-session start

Do all the required network testing, once done

    sudo netork-test-session stop

Stopping will collect the logs and print out their location, at any time logs
can be collected by running

    sudo network-test-session collect

this command will also output the location of the tar'ed up logs.

# Building

If you want to build this package, just run

    debuild

