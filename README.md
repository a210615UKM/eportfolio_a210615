# e-Portfolio — Muhammad Aniq Haikal Bin Mustazar

> **TTTM2213 — Mobile App Programming · Software Engineering 2SE2 · Universiti Kebangsaan Malaysia**
> Instructor: **Mr. Nelson** · Matric No: **A210615** · Session 2025/2026

This repository is my personal e-Portfolio for the Mobile App Programming course. It documents the full journey from foundational Jetpack Compose labs to the final Android capstone — **Humanity**, an app aligned with **SDG 1 — No Poverty**.

🌐 **Live site:** `https://<your-username>.github.io/eportfolio_a210615/`
📱 **Flagship project:** Humanity — donations, jobs, and volunteering in one Android app
🌍 **SDG focus:** Goal 1 — No Poverty

---

## 📑 Table of Contents

1. [About the Author](#about-the-author)
2. [SDG Statement](#sdg-statement)
3. [Lab Submissions](#lab-submissions)
   - [Lab 1 — UI with Jetpack Compose](#lab-1--ui-with-jetpack-compose)
   - [Lab 2 — Interaction in Compose](#lab-2--interaction-in-compose)
   - [Lab 3 — Material Design](#lab-3--material-design)
   - [Lab 4 — Navigation & ViewModel](#lab-4--navigation--viewmodel)
   - [Lab 5 — Room Local Database](#lab-5--room-local-database)
4. [Project Submissions](#project-submissions)
   - [Project 1 — Humanity (Foundation Build)](#project-1--humanity-foundation-build)
   - [Project 2 — Humanity (Final Capstone)](#project-2--humanity-final-capstone)
5. [Skills & Tech Stack](#skills--tech-stack)
6. [Repository Structure](#repository-structure)
7. [Running the Site Locally](#running-the-site-locally)
8. [Deploying to GitHub Pages](#deploying-to-github-pages)
9. [References](#references)
10. [AI Assistance Acknowledgement](#ai-assistance-acknowledgement)

---

## About the Author

I'm a Software Engineering student at UKM exploring how mobile technology can carry social weight. Through this course I learned to design with Jetpack Compose, manage state intentionally, follow Material 3 guidelines, structure flow with ViewModels, and persist data with Room.

My goal is simple: **build software that quietly helps people.** The labs taught me the craft; the project gave me the cause.

---

## SDG Statement

**SDG 1 — No Poverty.** Poverty in Malaysia and around the world is fed by unemployment, disasters, and limited access to support. Help exists, but it's scattered across many platforms — donors don't know who to trust, job-seekers waste time searching, and willing volunteers can't find the right cause.

> **Humanity** is a mobile app that fights poverty by uniting **donations, jobs, and volunteer activities** into one trusted platform — empowering anyone to give, work, and serve with a single tap.

---

## Lab Submissions

Five hands-on labs that build the foundations for modern Android development with Kotlin and Jetpack Compose.

### Lab 1 — UI with Jetpack Compose

| | |
|---|---|
| **Topic** | Basic Layout · Composables · Modifiers |
| **YouTube Demo** | https://youtu.be/Tl4JIM3wbEg |
| **Due Date Reference** | 9 March 2026 |

**What I built**
A static UI screen using only Jetpack Compose primitives — `Column`, `Row`, `Text`, `Image`, and `Modifier` chains — to recreate a multi-section layout with proper spacing, alignment, and reusable composables.

**Key concepts applied**
- Declarative UI with `@Composable` functions
- Layout containers: `Column`, `Row`, `Box`
- `Modifier` chaining for padding, size, alignment, background
- Typography and color via `MaterialTheme`
- Composable previews with `@Preview`

**What I learned**
Jetpack Compose felt different from XML — declarative, predictable, and fast to iterate. Building this layout taught me that **spacing and alignment carry as much weight as the words on the screen**. Re-using small composables keeps the code clean and lets the UI scale naturally.

---

### Lab 2 — Interaction in Compose

| | |
|---|---|
| **Topic** | State · Events · `remember` & `mutableStateOf` |
| **YouTube Demo** | https://youtu.be/PJfO1lZNfQA |
| **Due Date Reference** | 29 March 2026 |

**What I built**
An interactive Compose screen that responds to user input. Buttons mutate state, the UI reacts immediately, and values survive recomposition through `remember`.

**Key concepts applied**
- State holders: `mutableStateOf`, `remember`, `rememberSaveable`
- Event handlers: `onClick`, `onValueChange`
- **State hoisting** — lifting state up to the composable that owns it
- **Unidirectional data flow** — events go up, state comes down
- Recomposition behaviour and how Compose decides what to re-render

**What I learned**
This was the lab where state finally clicked for me. The UI is not a thing you change — **it's a function of the state you hold.** Once that mindset landed, every subsequent lab felt easier. State hoisting also made my composables more testable and reusable.

---

### Lab 3 — Material Design

| | |
|---|---|
| **Topic** | Theming · Typography · Material 3 Components |
| **YouTube Demo** | https://youtu.be/EVDgd5Efd_w |
| **Due Date Reference** | 6 April 2026 |

**What I built**
A polished UI built entirely with Material 3 components — `Scaffold`, `TopAppBar`, `Card`, `Button`, `FilledTonalButton`, `Icon` — bound to a custom `ColorScheme` and `Typography` definition.

**Key concepts applied**
- Material 3 (`androidx.compose.material3`) component library
- Custom `ColorScheme` with dynamic light/dark variants
- `Typography` scale (display, headline, title, body, label)
- `Shape` system for consistent corner radii
- Theming applied through `MaterialTheme { ... }` wrapper
- Accessibility considerations (contrast, touch target size)

**What I learned**
Material 3 isn't a constraint — it's a contract with the user. Following the guidelines means following the user's expectations. I stopped fighting the system and started designing inside it: **colour, scale, and rhythm**. The UI immediately began to feel professional and accessible.

---

### Lab 4 — Navigation & ViewModel

| | |
|---|---|
| **Topic** | NavHost · Routes · MVVM Architecture |
| **YouTube Demo** | https://youtu.be/lFIhNWZ4sMI |
| **GitHub Repo** | https://github.com/a210615UKM/a210615_aniqhaikal_drnelson_lab4 |
| **Due Date Reference** | 13 April 2026 |

**What I built**
A multi-screen Compose app with proper navigation between routes, backed by ViewModels that survive configuration changes (rotation, theme switch). This served as the **architectural skeleton for Project 1**.

**Key concepts applied**
- `NavHost` and `NavController` for routing
- Typed routes with arguments (`composable("detail/{id}")`)
- `viewModel()` factory and `ViewModel` lifecycle
- MVVM separation: View (Compose) ↔ ViewModel ↔ Repository/Model
- `StateFlow` / `mutableStateOf` exposed from ViewModel
- Back-stack management with `popBackStack()` and `navigate()`

**What I learned**
My apps stopped being single screens and **started being stories**. `NavHost` gave them flow, `ViewModel` gave them memory across rotations. This was the lab where my code began to feel like an actual production app — separated, testable, and scalable.

---

### Lab 5 — Room Local Database

| | |
|---|---|
| **Topic** | Entities · DAO · Coroutines · Flow |
| **YouTube Demo** | https://youtu.be/RO1mBf4ttIM |
| **GitHub Repo** | https://github.com/a210615UKM/A210615_AniqHaikal_DrNelson_Lab05 |

**What I built**
A persistent CRUD app using Room as the local database. Data survives app restarts, and the UI updates **reactively** as the database changes — no manual refresh needed.

**Key concepts applied**
- `@Entity`, `@PrimaryKey`, `@ColumnInfo` for table definition
- `@Dao` interfaces with `@Insert`, `@Update`, `@Delete`, `@Query`
- `RoomDatabase` singleton via `Room.databaseBuilder`
- `suspend fun` + Coroutines for non-blocking I/O
- `Flow<List<Entity>>` for reactive observation in Compose
- Repository pattern bridging DAO and ViewModel

**What I learned**
Persistence changed everything. Once Room was wired up with `Flow`, the data layer felt **alive** — the database whispered, Compose listened, and the UI updated like a quiet conversation. Setting up entities, DAOs, and the database forced me to think about schema design and migrations seriously.

---

## Project Submissions

The two capstone projects are different stages of the **same app — Humanity** — building progressively from a navigation-based prototype into a full-featured platform with API, sensors, and cloud.

### Project 1 — Humanity (Foundation Build)

| | |
|---|---|
| **Built on** | Lab 4 (Navigation + ViewModel) |
| **YouTube VSR** | https://youtu.be/Nl0O3pdzt1Q |
| **GitHub Repo** | https://github.com/a210615UKM/a210615_aniq_drnelson_project1 |
| **Lab 4 Repo** | https://github.com/a210615UKM/a210615_aniqhaikal_drnelson_lab4 |

**Problem statement**
Many willing donors and volunteers don't know where to give, how to find verified causes, or how to access poverty-reducing job opportunities. Existing platforms scatter these touchpoints across multiple apps, creating friction at the exact moment someone is willing to help.

**What I built**
A multi-screen Android app that brings all three pillars — **donating, working, volunteering** — into a single navigation flow.

- 🏠 **Home screen** — entry point with three primary actions
- � **Donation flow** — browse trusted causes and donate
- 💼 **Jobs screen** — list opportunities for poverty-affected users
- 🤝 **Volunteer screen** — discover community activities
- 👤 **Profile screen** — view personal info and history

**Architecture**
- Jetpack Compose + Material 3 throughout
- `NavHost` routes for every screen
- `ViewModel` per major feature for state management
- Repository layer for data access (in-memory at this stage)
- Clear MVVM separation: Compose UI is dumb, logic lives in ViewModels

**Lessons learned**
- **Architecture matters early.** Separating screens, view models, and data sources from day one paid off when Project 2 added complexity.
- **Good UX means cutting features, not adding them.** I removed three screens during iteration because they didn't earn their place.
- **Refactor without fear.** I refactored the navigation graph three times before it felt right — each pass made the code shorter and clearer.

---

### Project 2 — Humanity (Final Capstone)

| | |
|---|---|
| **Built on** | Lab 5 (Room) + Project 1 |
| **YouTube VSR** | https://youtu.be/luE9yQ4tGuE |
| **Project 2 Repo** | https://github.com/a210615UKM/a210615_aniq_drnelson_project2 |
| **Lab 5 Repo** | https://github.com/a210615UKM/A210615_AniqHaikal_DrNelson_Lab05 |

**Problem statement**
Poverty in Malaysia is fueled by unemployment, disaster, and limited access to support — yet the help that exists is fragmented across NGOs, job boards, and volunteer registries. **Humanity** unites donations, jobs, and volunteer activities so anyone can take meaningful action with a single tap, online or offline.

**Mandatory features delivered (per Project 2 guidelines)**

| Requirement | Implementation |
|---|---|
| **2 core screens** | Donation flow + Jobs & Volunteer hub |
| **API integration** | REST API calls (Retrofit + Coroutines) for live opportunities and charities |
| **Sensors** | Location sensor for nearby volunteer matching; optional accelerometer / orientation for UX touches |
| **Cloud backend** | Firebase Authentication + Firestore for user data and content |
| **Local persistence** | Room database for offline-first reliability |

**Tech stack**
- **Language:** Kotlin
- **UI:** Jetpack Compose, Material 3
- **Navigation:** Compose Navigation
- **Architecture:** MVVM + Repository pattern
- **Async:** Coroutines + `Flow`
- **Network:** Retrofit + Gson/Moshi
- **Cloud:** Firebase Auth, Firestore, Cloud Storage
- **Local:** Room (entities, DAOs, migrations)
- **Sensors:** Android `LocationManager` + `SensorManager`

**Key feature flow**
1. User signs in via Firebase Auth.
2. App loads cached data from Room (offline-first), then syncs from API/Firestore in the background.
3. Sensor reads device location to suggest nearby volunteer activities.
4. User donates, applies for a job, or joins a volunteer event — all written to Firestore and mirrored locally in Room.
5. Donation history and joined activities appear instantly in the Profile screen via reactive `Flow`.

**Lessons learned**
- **Real apps are integration problems.** Wiring up an API, sensors, cloud, and a local database forced me to handle errors, timeouts, and edge cases gracefully.
- **Design for offline.** Room as a single source of truth meant the app stayed usable even on bad networks — and the cloud sync just caught up later.
- **Permissions are UX.** Asking for location at the right moment (and explaining why) doubled my acceptance rate during testing.
- **Ship small, ship often.** Each weekly increment beat trying to build everything at once.

---

## Skills & Tech Stack

**Languages**
Kotlin · Java · SQL · XML · HTML / CSS · JavaScript

**Android**
Jetpack Compose · Material 3 · Compose Navigation · ViewModel · Room · Flow · Coroutines · Sensor APIs

**Backend & Cloud**
Firebase Auth · Firestore · Cloud Storage · REST APIs · Retrofit · Gson / Moshi · JSON

**Tools**
Android Studio · Gradle (Kotlin DSL) · Git · GitHub · GitHub Pages · Figma · Postman

**Concepts**
MVVM · State Management · Reactive UI · Offline-first design · Material Design · SDG-driven development

---

## 🔗 Quick Links

| Submission | YouTube | GitHub |
|---|---|---|
| Lab 1 — UI | [▶ Watch](https://youtu.be/Tl4JIM3wbEg) | — |
| Lab 2 — Interaction | [▶ Watch](https://youtu.be/PJfO1lZNfQA) | — |
| Lab 3 — Material Design | [▶ Watch](https://youtu.be/EVDgd5Efd_w) | — |
| Lab 4 — Navigation & VM | [▶ Watch](https://youtu.be/lFIhNWZ4sMI) | [Repo](https://github.com/a210615UKM/a210615_aniqhaikal_drnelson_lab4) |
| Lab 5 — Room | [▶ Watch](https://youtu.be/RO1mBf4ttIM) | [Repo](https://github.com/a210615UKM/A210615_AniqHaikal_DrNelson_Lab05) |
| Project 1 — Humanity (Foundation) | [▶ VSR](https://youtu.be/Nl0O3pdzt1Q) | [Repo](https://github.com/a210615UKM/a210615_aniq_drnelson_project1) |
| Project 2 — Humanity (Final) | [▶ VSR](https://youtu.be/luE9yQ4tGuE) | [Repo](https://github.com/a210615UKM/a210615_aniq_drnelson_project2) |

---

## References

- **Android Developers — Jetpack Compose** — official Compose docs and codelabs
- **Material 3 Guidelines** — theming, typography, components
- **Room Persistence Library** — local database with SQLite abstraction
- **Retrofit + Gson / Moshi** — type-safe HTTP client for REST APIs
- **Firebase** — Authentication, Firestore, and Cloud Storage
- **Coil** — lightweight image loading for Compose
- **Kotlin Coroutines & Flow** — async and reactive primitives
- **Android Sensor APIs** — `LocationManager`, `SensorManager`
- **UN Sustainable Development Goals** — SDG 1 framework
- **UKM TTTM2213 Course Materials** — lectures and lab guides by Mr. Nelson

---

## AI Assistance Acknowledgement

Drafts of writing, reflections, and parts of the supporting documentation in this repository were refined with the help of **ChatGPT** and **Gemini**. All design decisions, source code, and final wording were reviewed, validated, and personalised by the author.

---

© 2026 **Muhammad Aniq Haikal Bin Mustazar** · A210615 · Software Engineering 2SE2 · UKM
Built with intent for **SDG 1 — No Poverty**.
