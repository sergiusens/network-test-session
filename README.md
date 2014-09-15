# Use

To use this all you need to do is install or have the package installed and
then inside a phablet-shell do

    sudo start netork-test-session

Do all the required network testing, once done

    sudo stop netork-test-session

And to get a copy of the needed files run

    sudo network-test-session-tar

that last command will output the location of the tar'ed up logs.

# Building

If you want to build this package, just run

    debuild

