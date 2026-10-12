# Sankalp Sandeep Singh

Mobile engineer in Fort Worth, Texas. I write Kotlin and Swift, and I've built the
same audio-streaming product natively on both platforms.

I've also shipped Flutter and React Native apps, and then rewritten one of them
natively from scratch — which is why I have specific opinions about when the
cross-platform trade pays for itself and when it quietly costs more than it saves.

The hard part of streaming was never the UI. It's playback that survives
backgrounding, call interruptions, Bluetooth route changes and a network that drops
mid-buffer. Building it twice also means making every product decision twice against
two different frameworks — and occasionally concluding that one platform has no
equivalent at all, so the screen should honestly work differently there rather than
pretend.

### What I work on

- **Media pipelines** — Media3 `MediaLibraryService` and `MediaSession`, background
  playback, lock-screen and notification controls, Android Auto
- **Device integration** — BLE GATT, HealthKit, WatchConnectivity, WidgetKit,
  Live Activities
- **Both platforms in parallel** — Kotlin/Compose and Swift/SwiftUI, including
  porting a `Flow`-based architecture onto Swift Concurrency without translating it
  line for line

### Worth reading

**[smart-calories](https://github.com/sankalp047/smart-calories)** — nutrition and
body-composition tracking across iPhone, Apple Watch and the Home Screen. ~13,000
lines of Swift, **zero third-party dependencies**. That's a design position, not a
boast: it's why state is `@Observable` rather than Combine, and why there's no Core
Data. It also pairs with Bluetooth kitchen scales that implement no standard profile,
by solving their frame layout from two known weights.

**[engineering-notes](https://github.com/sankalp047/engineering-notes)** —
architecture write-ups on production work whose source isn't mine to publish:
patterns, public APIs and my own illustrative code, no employer source. Currently one
service and one player for all audio, and what actually breaks when you port Kotlin
`Flow` to Swift Concurrency.

### Elsewhere

Co-author of a peer-reviewed county-level COVID-19 dataset covering all 3,142 US
counties.

M.S. Computer Science, University of Texas at Arlington.

Shipped: BigFan (Android — Kotlin, Compose, Media3) · Radio Sangam · FPK Pass.

---

<sankalpsandeepsingh@gmail.com> · [LinkedIn](https://linkedin.com/in/sankalpsandeepsingh)
