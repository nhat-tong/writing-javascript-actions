### Workflow

![workflow](https://camo.githubusercontent.com/fd0a925f56ff417c793c7b84e3cd3998cfff191e6cc2a897f184c42c1ae9c6af/68747470733a2f2f692e696d6775722e636f6d2f437778476f62682e706e67)

## Action metadata
Filename: action.yml
This file contains 3 required fields:

* name
* description
* runs
  * using
  * main

## Input

Input parameter for an action:

* description: required
* required: (true or false)
* default
* core.getInput("[name]")

## Output

Output parameter of an action:

* core.setOutput("[name]")
* reference to output parameter of previous action in a workflow: @steps.[step_id].outputs.[name]

## get rid of node_modules
* npm install command
* ncc build index.js

## error handling
* core.setFailed(err.message);