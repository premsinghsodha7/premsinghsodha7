# Hi, I'm Prem Singh 👋

**Lead Mobile Engineer · Android & Kotlin · Jetpack Compose · Kotlin Multiplatform**

Based in Dubai, UAE · Building Android and cross-platform apps at **Synechron**

[LinkedIn](https://www.linkedin.com/in/premsinghsodha7/) · [Medium](https://premsinghsodha7.medium.com/) · [DEV](https://dev.to/prem_singh_1997) · [Hashnode](https://hashnode.com/@prem1997)

I build mobile applications with clear architecture boundaries, reusable interface components, and testable application rules. My core specialization is native Android with Kotlin and Jetpack Compose, complemented by Kotlin Multiplatform and Compose Multiplatform projects.

My engineering focus spans application structure, UI state management, component reuse, data persistence, and automated verification. My public portfolio brings these concerns together through runnable applications, a reusable component library, focused unit tests, and documented build workflows.

Finance interfaces are a recurring theme in my work here, including account dashboards, transfer validation, transaction activity, and payment-related UI components.

## Engineering focus

- **Application architecture:** explicit boundaries between domain rules, data implementations, ViewModels, and Compose UI.
- **Reusable components:** shared presentation APIs packaged separately from their consuming application.
- **State management:** reactive data flows and read-only state exposed to the UI.
- **Data handling:** local persistence where required, with clear limits for in-memory demonstrations.
- **Delivery discipline:** documented setup, focused unit tests, and automated build workflows.
- **Multiplatform development:** shared Compose UI and app behavior with platform-specific entry points.

## Featured projects

### [FintechFlow](https://github.com/premsinghsodha7/FintechFlow)

**Android architecture and finance interactions**

A fictional banking application demonstrating an account dashboard, transaction filters, validated transfers, spending insights, and card controls.

**Engineering highlights**

- Separates domain models and the repository contract from the in-memory data implementation and Compose screens.
- Uses a ViewModel to expose read-only dashboard state backed by StateFlow.
- Parses transfer input into integer minor currency units using decimal arithmetic.
- Validates missing recipients, invalid amounts, and insufficient funds before updating demo account state.
- Includes repository tests covering successful transfers and rejected operations.
- Configures GitHub Actions to run unit tests and assemble the debug APK.

**Stack:** Kotlin · Jetpack Compose · Material 3 · ViewModel · StateFlow · JUnit

**Scope:** Local, fictional data held in memory. No backend, authentication, bank connection, or payment processing.

[Architecture and setup](https://github.com/premsinghsodha7/FintechFlow#readme) · [App preview](https://raw.githubusercontent.com/premsinghsodha7/FintechFlow/main/screenshots/app-preview.jpg)

### [ComposeKit](https://github.com/premsinghsodha7/ComposeKit)

**Reusable finance UI and library boundaries**

A Jetpack Compose component library with a separate runnable demo application. The project demonstrates how finance presentation components can be packaged for integration into another Android app.

**Engineering highlights**

- Separates the reusable `composekit` library from the consuming `demo` module.
- Provides balance cards, amount fields, transaction rows, account rows, budget summaries, and payment card previews.
- Includes transfer status and fee breakdown components.
- Supports enabled and loading action states, amount validation feedback, and selectable theme palettes.
- Keeps payment execution and financial data storage outside the presentation library.
- Includes amount-input policy tests.
- Configures GitHub Actions to run unit tests and assemble the demo APK.

**Stack:** Kotlin · Jetpack Compose · Material 3 · Android Library · Gradle · JUnit

**Scope:** A portfolio UI library with fictional sample values. Components do not process payments or connect to a backend.

[Component catalog and integration](https://github.com/premsinghsodha7/ComposeKit#readme) · [App preview](https://raw.githubusercontent.com/premsinghsodha7/ComposeKit/main/screenshots/app-preview.jpg)

### [PantryPal](https://github.com/premsinghsodha7/PantryPal)

**Local persistence and reactive Android state**

An offline pantry companion with expiry tracking, item search, category filters, shopping lists, and meal planning.

**Engineering highlights**

- Persists pantry entries through Room entities and a DAO.
- Observes database changes through Flow and exposes entries as ViewModel StateFlow.
- Uses coroutines for database writes.
- Separates expiry summaries and display rules into domain functions.
- Includes unit tests for expiry windows and date labels.
- Configures GitHub Actions to run unit tests and assemble the debug APK.

**Stack:** Kotlin · Jetpack Compose · Room · Coroutines · Flow · StateFlow · ViewModel

**Scope:** Pantry entries are stored locally on the device, without an account or cloud service.

[Implementation and setup](https://github.com/premsinghsodha7/PantryPal#readme) · [App preview](https://raw.githubusercontent.com/premsinghsodha7/PantryPal/main/screenshots/app-preview.jpg)

## Kotlin Multiplatform projects

### [FintechFlow KMP](https://github.com/premsinghsodha7/FintechFlowKMP)

**Shared finance UI and platform integration**

A Compose Multiplatform finance dashboard with sample account activity, demo transfers, card controls, and light and dark themes.

- Places shared Compose UI and application behavior in `commonMain`.
- Includes Android and desktop entry points.
- Provides an iOS Compose controller and device/simulator framework targets.
- Configures GitHub Actions to assemble Android and compile the desktop UI.

**Stack:** Kotlin Multiplatform · Compose Multiplatform · Material 3 · Gradle

**Scope:** Fictional data held in memory. Building and launching an iOS application requires Xcode.

[Project details](https://github.com/premsinghsodha7/FintechFlowKMP#readme) · [Android preview](https://raw.githubusercontent.com/premsinghsodha7/FintechFlowKMP/main/screenshots/app-preview.png)

### [HabitGarden KMP](https://github.com/premsinghsodha7/HabitGardenKMP)

**Shared habit interactions and Compose UI**

A multiplatform habit companion with daily check-ins, weekly progress, streak insights, and selectable Meadow, Sky, and Dusk themes.

- Shares Compose UI and habit behavior in `commonMain`.
- Includes Android and desktop entry points and an iOS Compose controller.
- Keeps the demonstration self-contained with session-based, in-memory state.

**Stack:** Kotlin Multiplatform · Compose Multiplatform · Gradle

**Scope:** Habit progress lasts for the current app session. Building and launching an iOS application requires Xcode.

[Project details](https://github.com/premsinghsodha7/HabitGardenKMP#readme) · [Android preview](https://raw.githubusercontent.com/premsinghsodha7/HabitGardenKMP/main/screenshots/app-preview.png)

## More Android work

### [HabitGarden](https://github.com/premsinghsodha7/HabitGarden)

**On-device storage and testable habit rules**

A native Android habit tracker with daily check-ins, consecutive-day streaks, weekly insights, and selectable themes.

- Stores habit data in private app preferences across app restarts.
- Separates local storage from habit and progress rules.
- Includes unit tests for consecutive streak behavior and progress calculations.
- Configures GitHub Actions to run unit tests and assemble the debug APK.

**Stack:** Kotlin · Jetpack Compose · ViewModel · Local Preferences · JUnit

[Project details](https://github.com/premsinghsodha7/HabitGarden#readme) · [App preview](https://raw.githubusercontent.com/premsinghsodha7/HabitGarden/main/screenshots/app-preview.jpg)

## Technical toolkit

| Area | Technologies and practices |
| --- | --- |
| Core language | Kotlin |
| Android UI | Jetpack Compose, Material 3 |
| Application structure | Repository contracts, ViewModels, separated domain rules |
| Asynchronous work and state | Coroutines, Flow, StateFlow |
| Local storage | Room, app preferences |
| Multiplatform | Kotlin Multiplatform, Compose Multiplatform |
| Testing | JUnit, domain-rule tests, repository behavior tests |
| Build and workflow | Gradle, Git, GitHub Actions, Android Studio |

## Explore and connect

The repositories include implementation details, setup instructions, screenshots, and documented limitations. Finance projects use fictional data and demonstrate UI and application behavior.

[Browse all repositories](https://github.com/premsinghsodha7?tab=repositories) · [Connect on LinkedIn](https://www.linkedin.com/in/premsinghsodha7/)

[Medium](https://premsinghsodha7.medium.com/) · [DEV](https://dev.to/prem_singh_1997) · [Hashnode](https://hashnode.com/@prem1997)
