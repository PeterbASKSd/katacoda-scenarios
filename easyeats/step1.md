# Overview of EasyEats (Heading for Step 1)

Overview
Docker compose is a tool for defining and running multi-container Docker application.

In this section, we will use Docker compose to Build and Deploy a "EasyEats" which is available at
https://github.com/polyu21022574x/EasyEats

The app is composed of the following components:

Voting-App: Frontend of the application written in Python, used by users to cast their votes. Each vote cast on the Voting app is stored in the Redis in-memory database.

Katacode: Katacoda scenario

grafana/provisioning: Saving the dashboards and datasources

orderapi: Order API of the application written in Python, used by users to order.

storeapi: Store API of the application written in Python, used by users to order.

tests: unit.py makes use of pytest for unit testing the various endpoints of REST API

webhook_listener: Webhook will be sent to a webhook listener when an order has been created or canceled.

README.md: Detail of the application

docker-compose.yaml: docker compose file for launching the application's services

mongo-init_order.js: mongodb file for order

mongo-init_store.js: mongodb file for store

prometheus.yml: prometheus file for launching the prometheus services


Clone the project from github.
`git clone https://github.com/polyu21022574x/EasyEats'`{{execute}}

View the docker compose file for launching your application's services.
'docker-compose.yaml'