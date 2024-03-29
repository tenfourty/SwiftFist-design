SwiftFist-design
================
SwiftFist is a Backend-as-a-Service, designed to run in any Java Servlet container.  

## Features
The following features will be made available to an end-user/application developer accessing the SwiftFist website:

* Ability to sign up/create an account
* Define entities via a wizard
* Have REST endpoints generated
* Set up security tokens
* Admin console to query data stored
* Clean up/manage data stored
* Billing

## REST endpoints
REST endpoints will be generated for the following functions related to a given entity.  All of these will be multi-tenant, of the form:

`http://www.server.com/${function}/${org}/${app}/${user}`

* Simple CRUD operations
* Querying/search
* Registration of push notifications
* Placing messages on a queue for push
* User auth and management
* Integration, routing, remote APIs (Camel in the Cloud?)

## Supported clients
Two primary classes of clients will be supported.  Desktop, via browser, and mobile.  

### Desktop
* Plain old Javascript
 * Bindings to Angular and Backbone
* Bindings to high-level development languages
 * Ruby, Python, etc

### Mobile
* iOS
* Android

## Deployment model
A Java WAR file that could be deployed in any servlet container.  This covers standalone containers such as:

* JBoss AS/WildFly
* Apache Tomcat
* Jetty
* ... etc

as well as hosted services such as:

* Amazon Beanstalk
* Red Hat OpenShift
* Google AppEngine
* ... etc
 
Later, using asynchronous event/loop models such as VertX may be explored.
