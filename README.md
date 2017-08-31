pyzip-demo-apb
======================

An apb for deploying a simple [Python Zip App Demo](https://hub.docker.com/r/ansibleplaybookbundle/pyzip-demo/) app that can bind to Postgres for testing purposes.

## What it does
* Deploys a bindable web app.

## Requirements

## Parameters
* NAMESPACE: Optional, default 'pyzip-demo', Namespace to deploy the cluster in.
* OPENSHIFT_TARGET: Required, target openshift deployment
* OPENSHIFT_TOKEN: Required, openshift login token to authenticate with

## Running the application
`docker run -e "OPENSHIFT_TARGET=<openshift_target>" -e "OPENSHIFT_TOKEN=<token>" ansibleplaybookbundle/pyzip-demo-apb provision`

## Tearing down the application
`docker run -e "OPENSHIFT_TARGET=<openshift_target>" -e "OPENSHIFT_TOKEN=<token>" ansibleplaybookbundle/pyzip-demo-apb deprovision`
