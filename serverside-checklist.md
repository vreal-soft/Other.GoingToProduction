# Serverside checklist

This is a checklist for serverside of the Web App.

## Access
 - [ ] **Only the production team should have access to production environments**
 - [ ] **Developers may have access to logs and monitoring information**

## Legal

 - [ ] **The app is compliant according to the organisation standards**
 - [ ] Licences of application's 3rd-party dependencies are not violated (OPTIONAL)
 - [ ] The application does not violate cryptography policies and laws (OPTIONAL)

## Resiliency 

* [ ] **The application can not cause Cascading Failures to propagate through the system**
* [ ] *Load tests are automated or occur on a regular cadence. You document and publish the results. (OPTIONAL)*
* [ ] *Stress tests are automated or occur on a regular cadence. You document and publish the results. (OPTIONAL)*
* [ ] *Once the applications have proven the ability to stand up to load and stress, chaos engineering is integrated to identify weak points and opportunities to reduce failures. (OPTIONAL)*
* [ ] *The application can reestablish all lost connections (OPTIONAL)*
 
## Load balancing

* [ ] *The project can run on multiple CPUs (OPTIONAL)*
* [ ] *The project can run behind the load balancer (OPTIONAL)*
* [ ] *I can add a new node without system downtime (OPTIONAL)*

## Transparent deployment
  
* [ ] *I can add a new node without stopping the application (OPTIONAL)*
* [ ] *I can add a new node without user sessions being lost/destroyed (OPTIONAL)*
* [ ] *I can make a rolling upgrades for the service (OPTIONAL)*

## Supervising

* [ ] **The application can survive a server restart**
* [ ] **The application is restarted automatically after the crash**
  

## Logging

* [ ] **The application logs all errors (even "swallowed")**
* [ ] *The application produces log output to rotated files (OPTIONAL)*
  * *Streams with different log levels are separated from each other*
  
* [ ] *The logs are aggregated to a log analysing service (OPTIONAL)*


## Monitoring

* [ ] *I have configured the alerts for abnormal activity (OPTIONAL)*

  * *Application restart events*
  * *Error rate threshold reached*
  * *Server resources are soon to be exhausted (CPU, memory, IO > 90%)*
  * *HTTP requests timeouts*
  * *HTTP responses with 500 status codes*

* [ ] *I have health checks for all parts of the system (OPTIONAL)*


## Metrics

* [ ] *I can observe different events from the app over time (OPTIONAL)*
  
  * *Number of requests for endpoints*
  * *Duration of requests for endpoints*
  * *Duration of business-logic operations*


## High Availability

* [ ] *I can run services in different independent Data Centers, Multi-AZ (OPTIONAL)*


## Backuping

* [ ] *Owner can manually restore all data from backups (OPTIONAL)*
* [ ] *Application rollback process is automated and tested (OPTIONAL)*


## Disaster recovery

* [ ] *The app have a disaster recovery plan with different levels of details and ETAs for example: how to recover one service, how to recover a database, how to recover the whole cluster, how to recover the whole region (OPTIONAL)*


## Security

* [ ] **I have audited the system against OWASP Top 10 Vulnerabilities**
* [ ] **I use TLS/SSL for all endpoints**
* [ ] **Secrets are secured properly in a vault or secret store.**
* [ ] **Each service or application requires proper authentication and authorization.**
* [ ] **Databases are available only from the production network**
* [ ] **All  usernames for DBs or any other third party apps must be changed from the default** 
* [ ] **All passwords must be not less then "strong" in this service [Password Strength Meter](https://www.passwordmonster.com/)**
* [ ] *I have added relevant security headers to app HTTP endpoints (OPTIONAL)*

  * `X-Frame-Options`
  * `X-Content-Type-Options`
  * `Content-Security-Policy`
  * `X-XSS-Protection`
  * `Strict-Transport-Security`
  * `Public-Key-Pins`

## Capacity planning

- [ ] **The application has enough required resources for each component in the system.**
- [ ] **The application has configured all limits for the services. To avoid situations when because of the memory leak in one service you kill everything around.**

## Deployment

* [ ] **Code is automatically scanned, formatted, or linted according to coding standards. (Static code analysis)**
* [ ] **When engineers commit their changes, the system kicks off automated builds, tests, and deployment to a lower-level environment. (CI / Continuous integration)**
* [ ] **Deploying to production involves nothing more than approval and a click of a button. (CD / Continuous delivery)**
* [ ] *The automated deployment strategy has been documented. For example, strategies include blue-green, canary, or others to create safer zero-downtime deployments. (OPTIONAL)*

## Health checks
 - [ ] **The app provides health check endpoints**
 - [ ] *3rd party services health check should be either checked by application service itself or has his health check endpoints or needs to make some scripts that check the health of 3rd party service. (OPTIONAL)*

## Support documentation

* [ ] **Integration instructions for APIs are documented. ([Swagger](https://swagger.io/), etc)**
* [ ] *A database schema represents the logical configuration of all or part of a relational database. ([dbdiagram.io](https://dbdiagram.io/), etc) (OPTIONAL)*
