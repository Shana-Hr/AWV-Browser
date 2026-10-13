# Awv browser (Android WebView) — Part 1/5: Project setup + Home UI

Open this folder in Android Studio (Koala+ / JDK 17), let Gradle sync, then Run.

Structure
- `ui/theme/Theme.kt`          colors + font hook (Manrope optional)
- `ui/components/AwvIcons.kt`  all SVG icons (same 24x24 path data as the demo) drawn natively
- `ui/components/Wallpaper.kt` sunset/mountain wallpaper (demo SVG, native)
- `ui/components/Pressable.kt` tap + press animation
- `ui/home/HomeScreen.kt`      omnibox, protected card, hero, shortcut grid, bottom bar

Not wired yet (comes in later parts): WebView, tabs, menu, history, ad-block, real stats, shortcuts.
