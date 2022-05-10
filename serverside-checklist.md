# Serverside checklist

This is a checklist for serverside of the Web App.

## Legal

 - [ ] **The app is compliant according to the organisation standards**
 - [ ] Licences of application's 3rd-party dependencies are not violated (OPTIONAL)
 - [ ] The application does not violate cryptography policies and laws (OPTIONAL)

## Resiliency 

* [ ] ~~My application can retain reasonable functionality in isolation~~
* [ ] **The application can not cause Cascading Failures to propagate through the system**
* [ ] *The application can recover from being under heavy load (OPTIONAL)*
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

* [ ] *I can run services in different independent Data Centers (OPTIONAL)*


## Testing
  
* [ ] **I have performed stress tests for the application**
* [ ] *I have performed network partitioning tests for the application (OPTIONAL)*


## Backuping

* [ ] *I can restore all data from backups (OPTIONAL)*


## Security

* [ ] **I have audited the system against OWASP Top 10 Vulnerabilities**
* [ ] **I use TLS/SSL for all endpoints**
* [ ] *I have added relevant security headers to app HTTP endpoints (OPTIONAL)*

  * `X-Frame-Options`
  * `X-Content-Type-Options`
  * `Content-Security-Policy`
  * `X-XSS-Protection`
  * `Strict-Transport-Security`
  * `Public-Key-Pins`
