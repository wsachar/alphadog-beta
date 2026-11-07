# AlphaDog Beta 1

**Test software, for invited beta testers only.**

AlphaDog works on your Rekordbox library: it repairs and tidies the collection, edits cues and grids,
builds playlists, and prepares USB sticks. This is the first beta. It is not finished, and **it has not
been comprehensively tested on professional DJ equipment.**

> **Before you use it, every time:** back up your Rekordbox library (in Rekordbox: *File > Library >
> Backup Library*) and keep a copy of your music files.
>
> **Playing out:** carry a backup USB exported **directly from Rekordbox**, not from AlphaDog, and check
> that it plays.
>
> The developer takes no responsibility for any loss, including incorrect or damaged libraries, files or
> USB sticks. You'll read and sign the full [Beta Test Agreement](AGREEMENT.md) in the app before you can
> use it.

## What you need

- A Mac with Apple silicon (M1 or newer), macOS 13 or later. (Intel Macs are not supported in this beta.)
- Rekordbox 6 or 7 with your library on the same computer.
- An internet connection when you first set it up. After that, AlphaDog Beta checks its licence when it
  starts and every few hours; it keeps working offline for up to 14 days.

A Windows build is offered only if `AlphaDog-Beta-1-Setup.exe` is listed on the
[release page](https://github.com/wsachar/alphadog-beta/releases/tag/beta-1).

## 1. Download

From the [Beta 1 release page](https://github.com/wsachar/alphadog-beta/releases/tag/beta-1):

- Mac: **AlphaDog-Beta-1-arm64.dmg**

## 2. Install (Mac)

1. Open the downloaded `.dmg` and drag **AlphaDog Beta** into **Applications**.
2. Open **AlphaDog Beta** from Applications. Because this beta is not signed by Apple, macOS stops it the
   first time ("Apple could not verify…" or "cannot be opened"). Click **Done** (not *Move to Bin*).
3. Open **System Settings > Privacy & Security**, scroll down to the message about *AlphaDog Beta*, and
   click **Open Anyway**. Enter your password, then click **Open**.

You only do this once. If macOS says the app "is damaged and can't be opened", open **Terminal** and run
this line, then open the app again:

```
xattr -dr com.apple.quarantine "/Applications/AlphaDog Beta.app"
```

AlphaDog Beta keeps its own settings, separate from any other copy of AlphaDog.

### Windows (only if a Windows download is listed)

Run `AlphaDog-Beta-1-Setup.exe`. If Windows shows "Windows protected your PC", click **More info**, then
**Run anyway**.

## 3. Sign the agreement and get your licence

AlphaDog Beta needs a licence that works on your computer only.

1. When AlphaDog Beta opens, read the **Beta Test Agreement**, tick every point, type your full name and
   e-mail address, and click **Sign and create my access request**.
2. Click **E-mail it** (or **Copy the request**) and send the access request to the address the app
   shows. It contains your name, e-mail address, the signed agreement and an ID for your computer.
3. You'll get a licence key back that starts with `ADB1-`. Paste all of it into **Paste your licence
   key** and click **Activate AlphaDog Beta**.

You can close the app while you wait; your signature is kept.

## 4. First steps

1. Back up your library in Rekordbox (*File > Library > Backup Library*). AlphaDog reminds you each time it
   starts.
2. Close Rekordbox while AlphaDog changes your library.
3. Follow the setup screen to point AlphaDog at your Rekordbox library. **Help & Guide** in the sidebar has
   a guided tour and the manual.

Everything in the beta carries a faint *AlphaDog Beta 1 · test build* watermark, and the sidebar shows
**Beta 1** with the build ID. Click **Test build** in the sidebar to see your licence, when it ends, and
when it was last checked.

## Reporting a problem

Please include:

- the **build ID** (under *Beta 1* at the top of the sidebar, for example `B1-20261106-1a2b3c4`),
- what you did, what you expected, and what happened (a screenshot helps),
- the log folder for anything that went wrong: *Settings > Diagnostics > Open logs folder*.

## When the beta ends

A licence ends on the date shown in the app, or earlier if it is withdrawn or this beta is replaced by a
newer one. AlphaDog Beta then stops opening the app and says why. **Your Rekordbox library and music files
are left exactly as they are** and keep working in Rekordbox.

## Removing it

Drag **AlphaDog Beta** from Applications to the Bin. To remove its settings and licence too, delete the
folder `~/Library/Application Support/alphadog-beta` (in Finder: *Go > Go to Folder…*). Neither touches
your Rekordbox library.

---

AlphaDog is independent. It is not made, endorsed or supported by AlphaTheta, Pioneer DJ or Rekordbox.
Rekordbox is a trademark of AlphaTheta Corporation.
