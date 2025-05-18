A [deployment](https://docs-3.prefect.io/3.0rc/deploy/infrastructure-examples/docker) is used to determine when, where, and how a flow function should run. Deployments elevate flows to remotely configurable entities that have their own API.
We create a deployment by callin a method on our flow - ***serve***
Running the script with the .serve method will do two things:
- create a deployment called "my-first-deployment" for your flow in the Prefect API
- stay running to listen for flow runs for this deployment; when a run is found, it will be _asynchronously executed within a subprocess_
## Why deployments?[¶](https://docs.prefect.io/latest/tutorial/deployments/#why-deployments "Permanent link")

Some of the most common reasons to use an orchestration tool such as Prefect are for [scheduling](https://docs.prefect.io/concepts/schedules/) and [event-based triggering](https://docs.prefect.io/concepts/automations/). Up to this point, we’ve demonstrated running Prefect flows as scripts, but this means _you_ have been the one triggering and managing flow runs. You can certainly continue to trigger your workflows in this way and use Prefect as a monitoring layer for other schedulers or systems, but you will miss out on many of the other benefits and features that Prefect offers.

Deploying a flow exposes an API and UI so that you can:

- trigger new runs, [cancel active runs](https://docs.prefect.io/concepts/flows/#cancel-a-flow-run), pause scheduled runs, customize parameters, and more
- remotely configure schedules and automation rules for your deployments
- dynamically provision infrastructure using [workers](https://docs.prefect.io/tutorials/workers/)

Lots of concepts like running multiple deployments [here](https://docs.prefect.io/latest/tutorial/deployments/)



#datascience #datapipelines #prefect #coding #python