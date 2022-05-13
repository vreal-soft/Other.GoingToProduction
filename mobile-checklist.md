# Mobile App Checklist

This is a checklist for react-based Mobile App **without the backend** or with a 3rd-party backend.

## Support platforms
 - [ ] **Versions of operating system support are discussed with the customer, or it depends on the support of their third-party services used by the program.**
 
## Access
 - [ ] **Only the production team should have access to AppStore and Play Market projects.**
 - [ ] **Developers may have access to logs and monitoring information.**
 - [ ] **Production keystores, certificates, and passwords are provided to the customer.**

## Legal
 - [ ] **The app is compliant according to the organisation standards**
 - [ ] *Licences of app's 3rd-party dependencies are not violated (OPTIONAL)*
 - [ ] *The app does not violate cryptography policies and laws (OPTIONAL)*

## Permissions
 - [ ] **For each permission access there must be a button that re-requests access or if access is blocked redirects the user to the settings page**

## Accessibility
 - [ ] *The app is accessible (OPTIONAL)*
    - [ ] *Colors and contrast are color-blind friendly OR there is a possiblity to switch to high-contrast mode (OPTIONAL)*
    - [ ] *Support for different languages (OPTIONAL)*
    - [ ] *Change program theme (OPTIONAL)*

## Deployment
 - [ ] **Play Market deploy requirements**
 - [ ] **AppStore deploy requirements**

## Loading optimization
 - [ ] **The app has enabled the Hermes [Using Hermes](https://reactnative.dev/docs/hermes/)**
 - [ ] *The app has enabled the enableSeparateBuildPerCPUArchitecture feature to reduce the file size. (OPTIONAL)*

## Assets
 - [ ] **Image format is supported by all platforms (Android, IOS)**

## Testing
 - [ ] **The app does not have memory leaks**
 - [ ] **The application looks according to the design on all devices with different screen extensions**

## Debugging
 - [ ] *Thrown exceptions are handled and passed to storage ([Sentry](https://sentry.io/), [Firebase Crashlytics](https://firebase.google.com/products/crashlytics), etc) (OPTIONAL)*

## Tracking
 - [ ] *The app gathers metrics about usage behaviour ([Firebase Analytics](https://rnfirebase.io/analytics/usage)) (OPTIONAL)*

## Security
 - [ ] **The app using [Secure encrypted storage](https://www.npmjs.com/package/react-native-encrypted-storage)**
 - [ ] **Secrets are secured properly in a vault or secret store.**

## Application support
 - [ ] *The application has a help page to contact the moderator or administrator of the program (OPTIONAL)*

## Support documentation
* [ ] **The structure of the project and the description of the approaches are documented. (README.md)**
