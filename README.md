# wayshare
Klimaschutz auf dem Weg zur Schule

> [!CAUTION]
> Please note that this project is still in its beta phase and not ready to be used yet.

This is the GitHub repo from the "wayshare" app. The app is used to connect people to come to school more climate-friendly.

For security reasons, the backend of wayshare is not open source. If you want to get access to it, contact us via [E-Mail](mailto:support@wayshare.de).

## Kotlin Multiplatform Notes
This is a Kotlin Multiplatform project targeting Android, iOS and Web.

* `/composeApp` is for code that will be shared across the Compose Multiplatform applications.
  It contains several subfolders:
  - `commonMain` is for code that’s common for all targets.
  - Other folders are for Kotlin code that will be compiled for only the platform indicated in the folder name.

* `/iosApp` contains iOS applications. Even if the UI is being shared with Compose Multiplatform, 
  this entry point is being needed for the iOS app. This is also where SwiftUI code should be added.
