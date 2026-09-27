# Bloop

Translate selected text in any app with a double-tap. Bloop is a macOS menu-bar utility: select
some text, double-tap the modifier key you chose, and the translation appears in a popover beside
the selection. The app you were in stays in front.

**[Download the latest release →](../../releases/latest)**

Requires **macOS 26** or later, Apple silicon or Intel. This repository holds the downloads only.

---

## Installing it

Open the DMG, drag Bloop to your Applications folder, and open it. Bloop is signed with an Apple
Developer ID and notarized by Apple, so macOS opens it like any other app.

On first run Bloop asks for one permission, **Accessibility**, so it can read the text you have
selected in other apps. It reads a selection only when you double-tap.

### If "Launch at Login" says it is unavailable

macOS sometimes runs a freshly downloaded app from a temporary copy of itself rather than from
where you put it — a security measure called app translocation. Bloop works normally, but it
cannot register a login item from there. Make sure Bloop is in **Applications** and open it from
there, not from the disk image. If it still says so, drag Bloop out of Applications and back in,
then reopen it.

## What leaves your Mac

- **Nothing, for Apple's languages.** Translation runs on your Mac. Language packs are downloaded
  from Apple once, the first time a language is used.
- **The selected text, only if you turn on Google Translate.** That setting is off by default. When
  it is on, text in languages Apple cannot translate is sent to Google, and the result is labelled
  "via Google".
- **Your licence key, once.** When you paste it, Bloop sends it to the licence server with your
  Mac's name and a one-way hash that identifies this Mac to Bloop only. That is how a licence knows
  which three Macs it is on. Once a day Bloop asks whether the licence is still valid; if the
  server cannot be reached, Bloop carries on working.
- **An update check, once a day.** Bloop downloads a small public file from this repository's
  GitHub Pages listing the latest version. It carries nothing about you or your Mac, and Bloop
  asks before installing an update.

There is no analytics, no telemetry, and no account. Your history stays in a file on your Mac.

## What it does

- **Double-tap to translate.** Any modifier key, at your own speed; it never collides with the
  shortcuts of the app you are in.
- **Write back.** A compose field in the popover translates the other way.
- **Pinned languages.** `⇥` steps the target through them, `⌥⇥` the source.
- **History** on `⌥⌘Y`, searchable, without taking focus from where you are typing.
- **Light, dark, or follow the Mac.**
