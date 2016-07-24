Completed. Go to overview.
Manage your app

The web console is convenient, but if you need deeper control you may want to try our command line tools.
Command line tools

Download and install the oc command line tool. After that, you can start by logging in, switching to this particular project, and displaying an overview of it, by doing:

oc login https://10.1.2.2:8443
oc project nodejs-test
oc status

For more information about the command line tools, check the CLI Reference and Basic CLI Operations.
Making code changes

A GitHub webhook trigger has been created for the nodejs-mongodb-example build config.

You can now set up the webhook in the GitHub repository settings if you own it, in https://github.com/marco73f/nodejs-ex/settings/hooks, using the following payload URL:

https://10.1.2.2:8443/oapi/v1/namespaces/nodejs-test/buildconfigs/nodejs-mongodb-example/webhooks/marco73f-secret-0306/github


