**== THIS REPOSITORY IS ARCHIVED ==**

See https://github.com/aroyoredhat/trigger-test-samples-build which picked up the torch :)

-------

This repository contains a Github Action that periodically checks that Samples Operator
works with the latest Openshift "ecosystem".

It does so by checking out the latest code of the [samples operator](https://github.com/openshift/cluster-samples-operator),
running the `./library-sync.sh` in it to update the samples and creates a PR
in the samples repository. This PR then triggers the openshift-ci that tries
to build the samples operator with the changes from running the library sync.
