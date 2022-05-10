# Single Page App Checklist

This is a checklist for browser-based Web App **without the backend** or with a 3rd-party backend.

## Legal

 - [ ] **App is compliant according to the organisation standards**
 - [ ] *Licences of app's 3rd-party dependencies are not violated (OPTIONAL)*
 - [ ] *App does not violate cryptography policies and laws (OPTIONAL)*

## Accessibility
 
 - [ ] *App is accessible (OPTIONAL)*
    - [ ] *Colors and contrast are color-blind friendly OR there is a possiblity to switch to high-contrast mode (OPTIONAL)*
    - [ ] *App is screenreader-friendly (OPTIONAL)*
    - [ ] *App has keyboard navigation (OPTIONAL)*

## Deployment

 - [ ] **App is served from CDN or cookie-less subdomain**
 - [ ] **App is served with forever cache headers for static assets**
 - [ ] **App static resources are gzipped**

## Loading optimization

 - [ ] **App can load it's assets in parallel (css, images and scripts)**
 - [ ] **App does not hit [browser HTTP requests limit per host](http://stackoverflow.com/questions/985431/max-parallel-http-connections-in-a-browser)**
 - [ ] *App uses modern formats of images (OPTIONAL)*
 - [ ] ~~My app uses icon sprites (OPTIONAL)~~
 - [ ] ~~My app loads all well-known javascript libraries from CDN~~

## Versioning

 - [ ] *My app has a cache-busting implemented (assets, object cache etc.) (OPTIONAL)*

## Assets

 - [ ] **Have a 404-page**
 - [ ] **Have a [maintenance page](https://www.smashingmagazine.com/2009/06/effective-maintenance-pages-examples-and-best-practices/)**
 - [ ] *Images support HDPI screens (Retina, etc) (OPTIONAL)*


## Testing

 - [ ] **App does not have memory leaks**
 - [ ] **App is loading in less than 3 seconds**
 - [ ] *My app is passing performance tests with high grades (OPTIONAL)*
    - [ ] *[PageSpeed](https://developers.google.com/speed/pagespeed/)*
    - [ ] *[YSlow](http://yslow.org/)*
    - [ ] *Chrome Dev Tools Audit*

## Debugging

 - [ ] *Thrown exceptions are handled and passed to storage ([Sentry](https://sentry.io/), [Track.js](https://trackjs.com/), etc) (OPTIONAL)*
 - [ ] ~~Minified JavaScript files contain URL for source maps~~
 - [ ] ~~Error storage process sourcemaped files~~

## Tracking

 - [ ] *App gathers metrics about usage behaviour (OPTIONAL)*

## Security
 - [ ] **I have audited the system against:**
    - [ ] [OWASP Top 10](https://www.owasp.org/index.php/OWASP_Top_Ten_Cheat_Sheet) Vulnerabilities
    - [ ] [Observatory](https://observatory.mozilla.org/)
    - [ ] [securityheaders.io](https://securityheaders.io/)
