# Serverside checklist

This is a checklist for serverside of the Web App.

## Legal

 - [ ] **My app is compliant according to the organisation standards**
 - [ ] Licences of my application's 3rd-party dependencies are not violated (OPTIONAL)
 - [ ] My application does not violate cryptography policies and laws (OPTIONAL)

## Resiliency 

* [ ] ~~My application can retain reasonable functionality in isolation~~
* [ ] **My application can not cause Cascading Failures to propagate through the system**
* [ ] *My application can recover from being under heavy load (OPTIONAL)*
* [ ] *My application can reestablish all lost connections (OPTIONAL)*
 
## Load balancing

* [ ] *My project can run on multiple CPUs (OPTIONAL)*
* [ ] *My project can run behind the load balancer (OPTIONAL)*
* [ ] *I can add a new node without system downtime (OPTIONAL)*

## Transparent deployment
  
* [ ] *I can add a new node without stopping the application (OPTIONAL)*
* [ ] *I can add a new node without user sessions being lost/destroyed (OPTIONAL)*
* [ ] *I can make a rolling upgrades for my service (OPTIONAL)*

## Supervising

* [ ] **My application can survive a server restart**
* [ ] **My application is restarted automatically after the crash**
  

## Logging

* [ ] **My application logs all errors (even "swallowed")**
* [ ] *My application produces log output to rotated files (OPTIONAL)*
  * *Streams with different log levels are separated from each other*
  
* [ ] *My logs are aggregated to a log analysing service (OPTIONAL)*


## Monitoring

* [ ] *I have configured the alerts for abnormal activity (OPTIONAL)*

  * *Application restart events*
  * *Error rate threshold reached*
  * *Server resources are soon to be exhausted (CPU, memory, IO > 90%)*
  * *HTTP requests timeouts*
  * *HTTP responses with 500 status codes*

* [ ] *I have health checks for all parts of my system (OPTIONAL)*


## Metrics

* [ ] *I can observe different events from my app over time (OPTIONAL)*
  
  * *Number of requests for endpoints*
  * *Duration of requests for endpoints*
  * *Duration of business-logic operations*


## High Availability

* [ ] *I can run my services in different independent Data Centers (OPTIONAL)*


## Testing
  
* [ ] **I have performed stress tests for my application**
* [ ] *I have performed network partitioning tests for my application (OPTIONAL)*


## Backuping

* [ ] *I can restore all my data from backups (OPTIONAL)*


## Security

* [ ] **I have audited my system against OWASP Top 10 Vulnerabilities**
* [ ] **I use TLS/SSL for all endpoints**
* [ ] *I have added relevant security headers to app HTTP endpoints (OPTIONAL)*

  * `X-Frame-Options`
  * `X-Content-Type-Options`
  * `Content-Security-Policy`
  * `X-XSS-Protection`
  * `Strict-Transport-Security`
  * `Public-Key-Pins`
