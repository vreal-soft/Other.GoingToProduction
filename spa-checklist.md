# Single Page App Checklist

This is a checklist for browser-based Web App **without the backend** or with a 3rd-party backend.

## Access
 - [ ] **Only the production team should have access to production environments**
 - [ ] **Developers may have access to logs and monitoring information**

## Legal

 - [ ] **The app is compliant according to the organisation standards**
 - [ ] *Licences of app's 3rd-party dependencies are not violated (OPTIONAL)*
 - [ ] *The app does not violate cryptography policies and laws (OPTIONAL)*

## Accessibility
 
 - [ ] *The app is accessible (OPTIONAL)*
    - [ ] *Colors and contrast are color-blind friendly OR there is a possiblity to switch to high-contrast mode (OPTIONAL)*
    - [ ] *The app is screenreader-friendly (OPTIONAL)*
    - [ ] *The app has keyboard navigation (OPTIONAL)*

## Capacity planning

- [ ] **The application has enough required resources for each component in the system**
- [ ] **The application has configured all limits for the services. To avoid situations when because of the memory leak in one service you kill everything around.**

## Deployment

 - [ ] **The app is served from CDN or cookie-less subdomain (CloudFront, etc)**
 - [ ] **The app is served with forever cache headers for static assets**
 - [ ] **The app static resources are gzipped**
 - [ ] **Code is automatically scanned, formatted, or linted according to coding standards. (Static code analysis)**
 - [ ] **When engineers commit their changes, the system kicks off automated builds, tests, and deployment to a lower-level environment. (CI / Continuous integration)**
 - [ ] **Deploying to production involves nothing more than approval and a click of a button. (CD / Continuous delivery)**
 - [ ] *The automated deployment strategy has been documented. For example, strategies include blue-green, canary, or others to create safer zero-downtime deployments. (OPTIONAL)*

## Loading optimization

 - [ ] **The app can load it's assets in parallel (css, images and scripts)**
 - [ ] **The app does not hit [browser HTTP requests limit per host](http://stackoverflow.com/questions/985431/max-parallel-http-connections-in-a-browser)**
 - [ ] *The app uses modern formats of images (OPTIONAL)*
 - [ ] *The app uses lazy loading of components to optimize chunk size and load speed. [Lazy loading](https://reactjs.org/docs/code-splitting.html#reactlazy)*

## Versioning

 - [ ] **The app manage title and description meta tags**
 - [ ] *The app has a cache-busting implemented (assets, object cache etc.) (OPTIONAL)*

## Assets

 - [ ] **Have a 404-page**
 - [ ] **Have a [maintenance page](https://www.smashingmagazine.com/2009/06/effective-maintenance-pages-examples-and-best-practices/)**
 - [ ] *Images support HDPI screens (Retina, etc) (OPTIONAL)*


## Testing

 - [ ] **The app does not have memory leaks**
 - [ ] **The app is loading in less than 3 seconds**
 - [ ] *The app is passing performance tests with high grades (OPTIONAL)*
    - [ ] *[PageSpeed](https://developers.google.com/speed/pagespeed/)*
    - [ ] *[YSlow](http://yslow.org/)*
    - [ ] *Chrome Dev Tools Audit*

## Debugging

 - [ ] *Thrown exceptions are handled and passed to storage ([Sentry](https://sentry.io/), [Track.js](https://trackjs.com/), etc) (OPTIONAL)*

## Tracking

 - [ ] *The app gathers metrics about usage behaviour (OPTIONAL)*

## Security

 - [ ] **The app using [Secure encrypted storage](https://www.npmjs.com/package/secure-ls)**
 - [ ] **I have audited the system against:**
    - [ ] [OWASP Top 10](https://www.owasp.org/index.php/OWASP_Top_Ten_Cheat_Sheet) Vulnerabilities
    - [ ] [Observatory](https://observatory.mozilla.org/)
    - [ ] [securityheaders.io](https://securityheaders.io/)
- [ ] **Secrets are secured properly in a vault or secret store.**

## Disaster recovery

 - [ ] *The app have a disaster recovery plan with different levels of details and ETAs for example: how to recover one service, how to recover a database, how to recover the whole cluster, how to recover the whole region (OPTIONAL)*

## SEO

 - [ ] **The app manage title and description meta tags**
 - [ ] *The app using Server Side Rendering (SSR) (OPTIONAL)*
 - [ ] *The app using third-party Dynamic Rendering middleware ([Prerender.io](https://prerender.io/), etc) (OPTIONAL)*
 - [ ] *The app manages social media meta tags (OPTIONAL)*
 - [ ] *App 100% verified by Chrome Dev Tools (SEO) (OPTIONAL)*

## Support documentation

* [ ] **The structure of the project and the description of the approaches are documented. (README.md)**
