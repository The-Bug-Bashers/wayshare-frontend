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


Learn more about [Kotlin Multiplatform](https://www.jetbrains.com/help/kotlin-multiplatform-dev/get-started.html),
[Compose Multiplatform](https://github.com/JetBrains/compose-multiplatform/#compose-multiplatform),
[Kotlin/Wasm](https://kotl.in/wasm/)…

**Note:** Compose/Web is Experimental and may be changed at any time. Use it only for evaluation purposes.
We would appreciate your feedback on Compose/Web and Kotlin/Wasm in the public Slack channel [#compose-web](https://slack-chats.kotlinlang.org/c/compose-web).
If you face any issues, please report them on [GitHub](https://github.com/JetBrains/compose-multiplatform/issues).

You can open the web application by running the `:composeApp:wasmJsBrowserDevelopmentRun` Gradle task.
