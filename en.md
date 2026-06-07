# Phrabbit User Guide

🌐 [한국어](ko.md) · **English** · [日本語](ja.md) · [简体中文](zh-Hans.md) · [繁體中文](zh-Hant.md)

An iOS app for practicing a foreign language with A/B loop audio. Load an audio file, loop any section freely on the waveform, and automatically turn the speech into text so you can read along while you listen.

---

## Contents

1. [Getting Started](#1-getting-started)
2. [Home Screen](#2-home-screen)
3. [Importing Files](#3-importing-files)
4. [Player: Basic Playback](#4-player-basic-playback)
5. [A-B Loop](#5-a-b-loop)
6. [Bookmarks](#6-bookmarks)
7. [Speech-to-Text (STT)](#7-speech-to-text-stt)
8. [Editing and Adding Segments](#8-editing-and-adding-segments)
9. [Wordbook](#9-wordbook)
10. [Podcasts](#10-podcasts)
11. [Settings](#11-settings)
12. [Free vs Premium](#12-free-vs-premium)
13. [FAQ](#13-faq)

---

## 1. Getting Started

### 1-1. First Launch — Onboarding
The first time you open the app, three intro slides appear.

1. **Pick sections precisely with the waveform** — see the audio as a graph and point to exactly the part you want.
2. **Loop endlessly between A and B points** — set a start point (A) and an end point (B), and only that section repeats automatically.
3. **Real-time speech-to-text** — the audio you're listening to is automatically turned into text so you can read along.

Use the **"Skip"** button at the top right to skip, or the **"Get Started"** button on the last slide to begin.

![Onboarding slide](images/01-onboarding.PNG)
*▲ `images/01-onboarding.PNG` — The first onboarding slide (with waveform animation)*

### 1-2. Free Trial
A **3-day free trial** starts automatically on first launch. For three days you can freely try every feature. While the trial is active, an orange banner reading **"🎁 Trial — D-N"** appears at the top of the player.

---

## 2. Home Screen

This is the app's main screen. Every audio file you add is collected here.

![Home screen](images/02-home.PNG)
*▲ `images/02-home.PNG` — The full home screen (top search bar + horizontally scrolling "Recently Played" + the full file list)*

### 2-1. Screen Layout

| Location | Element | Description |
|---|---|---|
| Top left | ⚙️ gear | Open Settings |
| Top right | ➕ purple circle | File-add menu |
| Top | 🔍 search bar | Search by file name |
| Upper middle | "Recently Played" | The last 5 files you played (horizontal scroll) |
| Middle | "All Files (count)" | The full file list |

### 2-2. Reading a File Row
The color of the icon on the left of each file tells you where it came from.

- 🟦 **Teal waveform icon** — a local file imported from the Files app
- 🟪 **Purple music-note icon** — a track imported from your Music library
- 🟧 **Orange antenna icon** — a podcast download

To the right of the icon you'll see the title, total duration, last playback position (if any), and the date added.

### 2-3. Actions

- **Tap a file once** → opens the player
- **Swipe a file left** → a red 🗑 **Delete** button appears; tapping it removes the file, its waveform cache, and its segment data all together.

![Swipe to delete a file](images/03-home-swipe-delete.PNG)
*▲ `images/03-home-swipe-delete.PNG` — A file row swiped left to reveal the red Delete button*

---

## 3. Importing Files

Tap the **➕ button** at the top right of the home screen to open the menu.

![Add menu](images/04-add-menu.PNG)
*▲ `images/04-add-menu.PNG` — The menu after tapping ➕ (Add from Files / Add from Music / Subscribe to Podcast)*

### 3-1. Add from the Files App
**Add from Files** → the system file picker opens. You can pick audio files such as mp3, m4a, wav, and aac. You may select several at once.

### 3-2. Add from the Music Library
**Add from Music** → the list of music stored on your iPhone opens.

- 🟢 **Green check mark** — a track already added to Phrabbit
- 🔒 **Gray lock + "DRM" label** — a track downloaded via an Apple Music subscription (blocked by copyright protection, so it cannot be imported). Only tracks you purchased outright or ripped from a CD can be used.

![Music library picker](images/05-music-picker.PNG)
*▲ `images/05-music-picker.PNG` — The music library picker (showing both a green check and a DRM lock)*

When you tap a track, it is automatically converted to m4a, added to Phrabbit, and the player opens right away.

### 3-3. Subscribe to a Podcast (Premium)
While Premium is active, tapping **Subscribe to Podcast** shows your Apple Podcasts subscriptions.
In the free version a 🔒 lock appears at the top right of the antenna icon, and tapping it takes you to the purchase screen.

See [10. Podcasts](#10-podcasts) for full details.

---

## 4. Player: Basic Playback

Tap a file on the home screen and the player opens full-screen.

![Player full screen](images/06-player-main.PNG)
*▲ `images/06-player-main.PNG` — The full-screen player (top ⌄ button + waveform + A-B info bar + bottom controls + the STT text area, all visible at once)*

### 4-1. Two Ways to Close the Screen

| Method | Description |
|---|---|
| Top-left ⌄ button | Tap once to lower the player and return home |
| Swipe down from the top | Grab the header and drag down to close it |

Playback continues even after you close the player. A **mini player** stays at the bottom of the screen; tap it to reopen the player.

![Mini player](images/07-mini-player.PNG)
*▲ `images/07-mini-player.PNG` — The mini player floating at the bottom of the home screen*

### 4-2. The Waveform Area
Next to the time display (e.g., `0:00`), the waveform spreads out horizontally in 5-second units, and during playback a black vertical line (the playhead) moves along with it. The screen also scrolls automatically to follow the playback position.

- **Tap the waveform once** → jump to that position
- **Long-press the waveform (0.5s)** → set point A or B (see [5. A-B Loop](#5-a-b-loop))

### 4-3. Bottom Controls — Top Row

![Bottom controls, top row](images/08-controls-top-row.jpg)
*▲ `images/08-controls-top-row.jpg` — Just the top row of the bottom controls (left to right: A-B / undo / eraser / divider / loop count / playback speed)*

| Button | Function |
|---|---|
| **A-B** capsule | Tap to set the A then B points in order |
| ↶ **Undo** | Jump to the current A point |
| 🧹 **Eraser** | Clear the A-B range |
| 🔁 **Loop count** | Each tap cycles ∞ → 1 → 2 → 3 → 5 → 10 → ∞ |
| **1x / 0.75x …** | Change playback speed. Cycles 0.5 → 0.75 → 1 → 1.25 → 1.5 → 2 → 0.5 |

### 4-4. Bottom Controls — Bottom Row

![Bottom controls, bottom row](images/09-controls-bottom-row.jpg)
*▲ `images/09-controls-bottom-row.jpg` — Just the bottom row of the bottom controls (left: star & list / center: back 5s ▶ forward 5s / right: the transcript mic button)*

| Button | Function |
|---|---|
| ⭐ **Star** | Save the current A-B range as a bookmark (Premium) |
| 📋 **List** | Open the saved bookmark list (Premium) |
| ⏪ **Back 5s** | Rewind 5 seconds |
| ⏯ **Large play button** | Play / pause |
| ⏩ **Forward 5s** | Skip ahead 5 seconds |
| 💬 **Transcript / mic** | Speech-to-text (Premium) |

---

## 5. A-B Loop

The core feature: endlessly loop any section so you can listen and repeat after it.

### 5-1. Set with the A-B Button (the easiest way)
Tap the **"A-B"** capsule at the far left of the bottom controls once and the current playback position becomes A. Tap again and that moment becomes B, and the loop starts immediately.

The capsule's appearance changes with its state.

| State | Capsule shows |
|---|---|
| Before A is set | Gray **"A-B"** |
| Only A is set | Purple outline **"A→B"** (waiting for B) |
| Both A and B set | Filled purple **"A-B"** (looping) |

![A-B capsule — not set](images/10a-ab-none.PNG)
*▲ `images/10a-ab-none.PNG` — Gray "A-B" (before A is set)*

![A-B capsule — waiting for B](images/10b-ab-waiting.PNG)
*▲ `images/10b-ab-waiting.PNG` — Purple outline "A→B" (waiting for B)*

![A-B capsule — looping](images/10c-ab-active.PNG)
*▲ `images/10c-ab-active.PNG` — Filled purple "A-B" (both A and B set, looping)*

When only A is set, a hint bubble reading **"👇 Tap A-B again to set the end"** briefly appears over the waveform and then fades.

### 5-2. Set by Long-Pressing the Waveform (precise)
**Long-press for 0.5 seconds** on the spot you want in the waveform to set point A. Long-press another spot to set point B and start the loop.

An **A handle (purple)** and a **B handle (orange)** appear over the waveform, and you can drag them with your finger to fine-tune their positions.

![Waveform A/B handles](images/11-ab-handles.PNG)
*▲ `images/11-ab-handles.PNG` — The A and B handles shown on the waveform with the span between them highlighted in purple*

### 5-3. The A-B Info Bar
When an A-B range is set, the info appears in purple text just below the waveform.

```
🔁  A: 0:12 → B: 0:18 (6.0s loop)
```

### 5-4. Loop Behavior and Controls

- **Loop-count button (🔁)**: Infinite loop (∞) is the default. Set a count and it repeats that many times, then stops automatically.
- **Undo button (↶)**: Jumps to point A immediately.
- **Eraser button (🧹)**: Clears the A-B range.

---

## 6. Bookmarks

Save sections you want to practice often. This is a **Premium feature**; free users can save up to 3 per file.

### 6-1. Saving
1. Set an A-B range first.
2. Tap the ⭐ **Star button** in the bottom controls.
3. Enter a name and tap **Save**.

![Bookmark save dialog](images/12-bookmark-save.PNG)
*▲ `images/12-bookmark-save.PNG` — The bookmark naming dialog*

If you tap the star without an A-B range set, a *"Set an A-B range first."* alert appears.

### 6-2. Loading from the List
Tap the 📋 **List button** next to the star to open this file's saved bookmarks in a sheet. Tap an item and its A-B range is set automatically and starts playing right away.

![Bookmark list sheet](images/13-bookmark-list.PNG)
*▲ `images/13-bookmark-list.PNG` — The bookmark list sheet*

Swipe an item left in the list to delete it.

---

## 7. Speech-to-Text (STT)

Automatically turn audio into text so you can check the words as you listen. This is a **Premium feature**.

### 7-1. Starting a Conversion
1. Tap the **💬 transcript button** at the bottom right of the player.
2. On first use, a **language selection** sheet appears. Choose the language you're studying — English, Korean, Japanese, etc.
3. Tap **Done** to start the conversion.

![STT language selection sheet](images/14-stt-language.PNG)
*▲ `images/14-stt-language.PNG` — The STT language selection sheet*

### 7-2. Conversion Progress
When the conversion starts, a progress bar and a **"Converting…  N/total"** indicator appear above the transcript area.

![Converting in progress](images/15-stt-converting.PNG)
*▲ `images/15-stt-converting.PNG` — Converting — the progress bar and Cancel button visible*

- Because it processes **in 45-second chunks**, longer audio takes more time (about a few minutes for an hour of audio).
- You can **cancel** mid-conversion with the ❌ button. Cancelling discards this run's results and **keeps your existing transcript** unchanged.
- The conversion keeps running in the background. It does not stop even if you close the player.

### 7-3. Viewing the Converted Text
When the conversion finishes, cards appear in chronological order in the transcript area at the bottom.

Each card contains:
- Start time (e.g., `0:32`)
- A source indicator (no mark for auto-generated, ✅ for an official transcript, 🖊 for user-edited, 📝 for manual entry)
- An ⚠️ orange warning if recognition confidence is low
- A 🕒 orange **Approx. position** badge when the position is approximate — the text was recognized but its exact timing couldn't be determined. Tapping seeks nearby, and you can edit it with ✏️
- The **body text**
- Small buttons on the right: 🌐 translate / ➕ wordbook / ✏️ edit / 🗑 delete

![Transcript card list](images/16-transcript-cards.PNG)
*▲ `images/16-transcript-cards.PNG` — The transcript card list (several rows, with the currently playing card outlined in orange)*

### 7-4. Card Actions

- **Tap a card** → sets that section as the A-B range and immediately starts looping it.
- **🌐 Translate**: On iOS 17.4+ devices the system translation popup appears.
- **➕ Wordbook**: Pick a word from the card and save it to your wordbook (see [9. Wordbook](#9-wordbook)).
- **✏️ Edit**: Edit the text.
- **🗑 Delete**: Delete the card.

The currently playing card is highlighted with an **orange border**. Cards that fall inside the A-B range are shown with a **light purple background**.

### 7-5. Sections That Couldn't Be Recognized — Gap Cards
A section with no recognized result for 30 seconds or more is shown as a gray card reading *"Could not recognize."* You can type the text yourself with the **📝 Enter Manually** button.

![Gap card](images/17-gap-card.PNG)
*▲ `images/17-gap-card.PNG` — A Gap card — "Could not recognize" + the Enter Manually button*

### 7-6. Re-running or Changing the Language
Tapping the 💬 button on an already-converted file brings up a menu.

- **🔄 Re-run with current language** — convert again in the current language
- **🌐 Change Language and Re-run** — convert again in a different language
- **🗑 Clear Script** — delete only the auto-generated transcript (your manual edits are kept)

![STT manage menu](images/18-stt-manage-menu.PNG)
*▲ `images/18-stt-manage-menu.PNG` — The STT manage menu (3 options)*

> 💡 **Tip**: If recognition accuracy is too low, a "Speech recognition accuracy may be low" alert appears. This often happens when the audio's actual language differs from the one you selected. Use the **Change Language** button to switch and try again.

---

## 8. Editing and Adding Segments

### 8-1. Add a Segment Manually
Tap the **➕ Add Segment** button at the top of the transcript area to create a new segment based on the current playback position. Enter text in the sheet and tap **Add** to add the card.

![Add Segment sheet](images/19-add-segment.PNG)
*▲ `images/19-add-segment.PNG` — The Add Segment sheet (time range + text entry + ▶ preview button)*

The **▶ preview button** in the sheet lets you briefly listen to just that section.

### 8-2. Edit a Segment
Tap the ✏️ button on a card to open the edit sheet and **edit the segment's text**. With the ▶ **Loop button** at the top you can listen to the section on repeat while you transcribe, and if you've edited an STT-generated transcript, an **Original** and a **Reset** button appear below so you can revert to the original at any time. (The segment's time range cannot be changed here; it is shown at the top for reference only.)

![Segment edit sheet](images/19-edit-segment.PNG)
*▲ `images/19-edit-segment.PNG` — The segment edit sheet (text editing + Loop preview)*

---

## 9. Wordbook

A space that collects the words you saved from transcript cards. This is a **Premium feature**.

![Wordbook list mode](images/20-wordbook-list.PNG)
*▲ `images/20-wordbook-list.PNG` — The Wordbook tab — list mode*

### 9-1. Saving Words
From a transcript card in the player, tap the ➕ button → on the **word selection** screen:

- Words automatically extracted from the card body are shown as capsules. Tap to pick them, or type your own under **Custom Input**.
- You can add a memo (optional).
- Tap **Save** to store them in your wordbook.

![Word save screen](images/20-wordbook-save.PNG)
*▲ `images/20-wordbook-save.PNG` — Picking and saving a word from a transcript card*

### 9-2. Two Viewing Modes
Switch modes with the segmented control at the top of the screen.

- **List** — see the word, its sentence context, the source file, the date added, and your memo at a glance. Swipe an item left to delete it.
- **Flashcards** — tap a card to flip between front and back (front: the word, back: sentence + memo). Swipe left or right to move to the next card.

![Flashcard — front](images/21a-wordbook-flashcard.PNG)
*▲ `images/21a-wordbook-flashcard.PNG` — Flashcard front (the word)*

![Flashcard — back](images/21b-wordbook-flashcard.PNG)
*▲ `images/21b-wordbook-flashcard.PNG` — Flashcard back (sentence + memo)*

---

## 10. Podcasts

Bring podcasts you subscribe to in Apple Podcasts in as study material. This is a **Premium feature**.

### 10-1. Opening
Home screen ➕ menu → **Subscribe to Podcast**.

### 10-2. Importing from Apple Podcasts
On first use you'll see a **"Load from Apple Podcasts"** button. Tapping it requests media library permission, and once allowed, your subscribed podcasts appear as horizontally scrolling cards.

![Podcast screen](images/22-podcast.PNG)
*▲ `images/22-podcast.PNG` — The podcast screen — Apple Podcasts subscription cards scrolling horizontally*

Tap a channel card to open its episode list in a sheet.

![Episode list sheet](images/23a-podcast-episodes.PNG)
*▲ `images/23a-podcast-episodes.PNG` — The episode list sheet (regular episodes with no official transcript)*

For each episode:
- Title, publish date, length
- **Script** badge (purple) — an episode that provides an official, time-synced transcript
- **Text only** badge (gray) — an episode with text only
- No badge — an episode that provides no transcript
- Status on the right:
  - ⬇ download icon — not downloaded yet
  - 🟣 progress ring — downloading
  - ✅ green check — download complete

Tap a checked episode to open the player right away.

![Episode with a Script badge](images/23b-podcast-episodes-script.PNG)
*▲ `images/23b-podcast-episodes-script.PNG` — An episode list with the purple **Script** badge*

> 💡 **Why we recommend Script episodes**: Episodes with the **Script** badge do not use iOS speech recognition (STT) to build the transcript — they **pull in the official transcript the podcast provides directly**. Because it's an accurate, human-written transcript, it has far fewer typos and misrecognitions than STT, and there's no conversion to wait for. When choosing study material, we recommend picking Script episodes first.

### 10-3. Importing Directly via an RSS URL
Expand **"Add via RSS URL (advanced)"** near the bottom of the screen to enter an RSS address directly. Use this to import a podcast that isn't in Apple Podcasts.

### 10-4. A Note on Cellular Data
The default setting is **download over Wi-Fi only**. If you've allowed cellular downloads in Settings, a confirmation alert appears before downloading a large episode.

---

## 11. Settings

Open it with the ⚙️ gear icon at the top left of the home screen.

![Settings screen](images/24-settings.jpg)
*▲ `images/24-settings.jpg` — The Settings screen*

### 11-1. Podcast Downloads
- **Download over Wi-Fi only** — when on, downloads happen only over Wi-Fi (default: on). This setting also applies to STT (speech-to-text) timestamp-recovery server recognition — on means Wi-Fi only, off allows it over cellular too.
- **Ask before cellular download** — shown when Wi-Fi-only is off; decides whether to ask each time before downloading over cellular.

---

## 12. Free vs Premium

### Free Forever
- Waveform view + A-B loop
- Playback speed control
- Import local files (Files app)
- Import from the Music library
- Bookmarks (up to 3 per file)

### Premium
- Speech-to-text (STT)
- Real-time transcript ↔ waveform sync
- Wordbook
- Unlimited bookmarks
- Podcast downloads

### How Payment Works
**A 3-day free trial → a one-time purchase.** Pay once and use it for life — it is not a subscription. Even if you change devices, **"Restore Purchases"** with the same Apple ID carries it over.

---

## 13. FAQ

**Q. Why can't I import a track I listened to on Apple Music?**
A. Tracks downloaded via an Apple Music subscription are locked by copyright protection (DRM) so they can't be used in other apps. Only tracks purchased from the iTunes Store or ripped from a CD will work.

**Q. Speech recognition is too inaccurate.**
A. Check two things: ① whether the audio's actual language matches the one you selected, and ② whether there's a lot of background music or noise. For sections that are too hard to recognize, just type them in yourself with ➕ Add Segment or Enter Manually.

**Q. What happens if I tap another file during a conversion?**
A. A confirmation reading *"Switch to ...? Conversion will be interrupted. Partial results will be saved."* appears. The part completed so far is preserved.

**Q. Is my data sent over the internet?**
A. Speech recognition runs **on-device** by default. However, when on-device recognition can't determine exact timing for some parts, Phrabbit sends just those audio segments to **Apple's speech recognition servers — only while on Wi-Fi (or any connection, if you've allowed cellular in Settings)** — to recover their position. No third-party servers are used, and your wordbook, bookmarks, and transcripts are all stored on your device. When you're offline, all recognition stays fully on-device.

**Q. What happens to my data if I change devices?**
A. The current version (v1.0) stores data only on the device. Installing the app on a new device and doing **Restore Purchases** with the same Apple ID unlocks Premium, but your wordbook, bookmarks, and transcripts do not transfer.

---

If you need support, please contact the developer via the contact details on the App Store page.
