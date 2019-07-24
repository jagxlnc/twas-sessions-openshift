## Traditional WAS Session persistence using DB2 database on OpenShift

By default, WebSphere places session objects in memory. However, the administrator has the option of enabling persistent session management, which instructs WebSphere to place session objects in a Database (persistent store)

*But how can you do that in a Cloud Platform, such as OpenShift, where you usually deploy a stateless application?*

The recommended approach is to revisit your application in order to make it stateless; in this way, you can scale it in a better way without problems. However, a common request, when a customer evaluates the use of an xPaaS environment, is to migrate an application without modifying it.

Learn how to maintain Sessions state configuring **Sessions DB Persistence for a tWAS application running on OpenShift.** using this GitHub Repo


## Sticky Sessions a.k.a Session Affinity in OpenShift
A lot of enterprise applications are not yet cloud-ready or even designed for microservices. Due to this fact, session stickiness is required for a lot of enterprise applications.

By default, sticky sessions for passthrough routes are implemented using the `source`  [load balancing strategy

When you need a cookie session stickiness, out-of-the-box OpenShift is a handy way to go.
