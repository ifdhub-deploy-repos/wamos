# wamos

This is a repo that is connected to the Azure web app containing 2 instances (each having its own stage deployment slot) and a DNS traffic manager profile.

Final domain: `http://wamos.ifdhub.com`

Instances:

1.Europe West `eu-west-wamos-1.azurewebsites.net`

* Stage Deployment Slot `http://eu-west-wamos-1-stage.azurewebsites.net`

2. Europe North `eu-north-wamos-1.azurewebsites.net`

* Stage Deployment Slot `http://eu-north-wamos-1-stage.azurewebsites.net`

When the new commit is made to this repo, the staging deployment slots will be automatically updated, as follows: `http://eu-west-wamos-1-stage.azurewebsites.net` `http://eu-north-wamos-1-stage.azurewebsites.net`

Next step involves swapping the deployment slots (production<->stage) for both instances at Azure.
