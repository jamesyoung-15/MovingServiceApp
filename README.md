# Project Research

- Main Goal: Create an application similar to TaskRabbit, mainly focus on IOS development
	- Services required:
		- Ability for client to make appointment with a worker
		- Show location of client and also when the worker will arrive with live tracking on map
		- Ability for worker to send notification for updates to client (eg. when worker has arrived)
		- Notification for appointment
		- Show availability of workers to avoid conflict of scheduling
		- Show services provided from workers
		- Payment

- Example Architecture
	- ![Architecture Diagram](https://d33wubrfki0l68.cloudfront.net/a7fe9d1aea6327529684a1c814b187346b052c75/4a156/static/70a81168d8ee88cb23c48107a1c70c1b/ae694/food-delivery-architecture.png)
		- Example of delivery service Flow:
			- **Front-end :** This is the interface customers use to generate menus, browse menus, place orders, and track delivery status.
			- **Backend server** This component handles requests from the front end, communicates with the database, and coordinates with delivery partners.
			- **Database:** This stores information about menus, orders, customers, and delivery partners.
			- **API Gateway:** This is responsible for request 
			  routing, composition, and protocol translation, among other things,   
			  between an application and a set of microservices.  
			- **Messaging Queue:** An asynchronous communication 
			  between systems that allows multiple systems to send and receive   
			  messages reliably and efficiently without needing to be constantly   
			  connected.  
			- **Notification Service:** To send notifications to users, typically through email or push notifications.
			- **Tracking Engine:** This will constantly watch for changes in the DB, update the elastic search index, and notify the messaging queue.

	- ![saas_example.jpg](../assets/saas_example_1687178482052_0.jpg)
		- An example architecture from a solo dev on Reddit
		- His archeticture:
			- Amplify - host the application written in react w/ typescript, next and tailwinds
			- Cognito - AWS identity access manager i.e. authentication server that ztores user accounts
			- API gateway - validate incoming requests and verify the access token (authorization) via an authorizer lambda
			- Lambda - serverless backend
			- Cloudwatch - monitoring service
			- Dynamo DB - database
			- SES - smtp server for email
			- Stripe - 3rd party payment API
-
- Example Tech Stack:
	- ![](https://miro.medium.com/v2/resize:fit:700/1*YPX2w3eWYxxdlkXbidfTzQ.png){:height 217, :width 700}
	-
-
- Resources
	- https://pratapsharma.com.np/architecture-of-food-delivery-app
	-# Wills_Project
