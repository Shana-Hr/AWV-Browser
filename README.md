# Awv browser (Android WebView) — Part 1/5: Project setup + Home UI

Open this folder in Android Studio (Koala+ / JDK 17), let Gradle sync, then Run.

Structure
- `ui/theme/Theme.kt`          colors + font hook (Manrope optional)
- `ui/components/AwvIcons.kt`  all SVG icons (same 24x24 path data as the demo) drawn natively
- `ui/components/Wallpaper.kt` sunset/mountain wallpaper (demo SVG, native)
- `ui/components/Pressable.kt` tap + press animation
- `ui/home/HomeScreen.kt`      omnibox, protected card, hero, shortcut grid, bottom bar

Not wired yet (comes in later parts): WebView, tabs, menu, history, ad-block, real stats, shortcuts.


ඔය demo එකේ ඩිසයින් එක use කරලා හදන්න android web veiw හරහා run වෙන kotin app එකක් ඒවගේම ඔයා place holder නොද තියෙන option වලට පමණක් අදාළ දේවල් දාන්න සහ svg icon දාලා හොදට හදලා දෙන්න Awv browser කියලා නම දාන්න ( android web veiw)
ඔක්කොම එකපාර හදන්න යන්න එපා 

1. **Project setup + Home screen UI**: Kotlin + Jetpack Compose project (`com.awv.browser`), Manrope font, demo එකේ color theme, SVG icons ඔක්කොම Vector drawables බවට, sunset wallpaper එක vector එකක් විදිහට, home screen (omnibox, "Protected this week" card, hero text, bottom bar).

2. **WebView engine + Tabs**: URL/search detect කිරීම, page load + progress bar, back/forward, new tab, tabs overlay (Normal/Private switch, tab cards, close, count badge).

3. **Menu sheet + Data**: menu bottom sheet, Bookmarks, History (Room DB), Downloads (DownloadManager), Desktop site toggle (user-agent + viewport).

4. **Privacy features**: ad/tracker blocking (`shouldInterceptRequest` + filter list), shield button + menu toggle, real stats counters (blocked / data saved / time saved), true Private mode (no history, cookies, cache).

5. **Extras + Release**: voice search, QR/code scan, user-added shortcut tiles ("Add" button), Settings screen (search engine, clear data), app icon, final polish, release APK build.

