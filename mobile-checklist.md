# Mobile App Checklist

This is a checklist for react-based Mobile App **without the backend** or with a 3rd-party backend.

## Access
 - [ ] **Only the production team should have access to AppStore and Play Market projects.**
 - [ ] **Developers may have access to logs and monitoring information.**
 - [ ] **Production keystores and passwords are provided to the customer.**

## Legal

 - [ ] **The app is compliant according to the organisation standards**
 - [ ] *Licences of app's 3rd-party dependencies are not violated (OPTIONAL)*
 - [ ] *The app does not violate cryptography policies and laws (OPTIONAL)*

## Accessibility
 
 - [ ] *The app is accessible (OPTIONAL)*
    - [ ] *Colors and contrast are color-blind friendly OR there is a possiblity to switch to high-contrast mode (OPTIONAL)*
    - [ ] *The app is screenreader-friendly (OPTIONAL)*
    - [ ] *The app has keyboard navigation (OPTIONAL)*

## Deployment

 - [ ] **Play Market deploy requirements**
 - [ ] **AppStore deploy requirements**

## Loading optimization

 - [ ] **The app has enabled the Hermes [Using Hermes](https://reactnative.dev/docs/hermes/)**
 - [ ] *The app has enabled the enableSeparateBuildPerCPUArchitecture feature to reduce the file size. (OPTIONAL)*

## Assets

 - [ ] **Images support HDPI screens (Retina, etc)**

## Testing

 - [ ] **The app does not have memory leaks**

## Debugging

 - [ ] *Thrown exceptions are handled and passed to storage ([Sentry](https://sentry.io/), [Firebase Crashlytics](https://firebase.google.com/products/crashlytics), etc) (OPTIONAL)*

## Tracking

 - [ ] *The app gathers metrics about usage behaviour ([Firebase Analytics](https://rnfirebase.io/analytics/usage)) (OPTIONAL)*

## Security

 - [ ] **The app using [Secure encrypted storage](https://www.npmjs.com/package/react-native-encrypted-storage)**
 - [ ] **Secrets are secured properly in a vault or secret store.**

## Disaster recovery

 - [ ] *The app have a disaster recovery plan with different levels of details and ETAs for example: how to recover one service, how to recover a database, how to recover the whole cluster, how to recover the whole region (OPTIONAL)*

## Support documentation

* [ ] **The structure of the project and the description of the approaches are documented. (README.md)**
