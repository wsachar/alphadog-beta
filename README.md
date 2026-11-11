# AlphaDog Beta

**Test software, for invited beta testers only.**

AlphaDog repairs and tidies your DJ library, edits cues and grids, builds playlists, and prepares USB
sticks. It works either in a library of its own, copied from your Rekordbox library (**Move to AlphaDog**,
which we recommend), or alongside Rekordbox, in Rekordbox's own library. This is a beta: it is not
finished, and **it has not been comprehensively tested on professional DJ equipment.**

> **Before you use it, every time:** back up the library AlphaDog works in and keep a copy of your music
> files. Alongside Rekordbox, that is your Rekordbox library (in Rekordbox: *File > Library > Backup
> Library*). Moved to AlphaDog, copy AlphaDog's library folder (*Settings > Your library* shows where it
> is) somewhere else.
>
> **Playing out:** carry a backup USB exported **directly from Rekordbox**, not from AlphaDog, and check
> that it plays. After a move, that stick won't have the changes you made in AlphaDog.
>
> The developer takes no responsibility for any loss, including incorrect or damaged libraries, files or
> USB sticks. You'll read and sign the full [Beta Test Agreement](AGREEMENT.md) in the app before you can
> use it.

## What you need

- A Mac with Apple silicon (M1 or newer), macOS 13 or later. (Intel Macs are not supported in this beta.)
- Rekordbox 6 or 7 with your library on the same computer.
- An internet connection when you first set it up. After that, AlphaDog Beta checks its licence when it
  starts and every few hours; it keeps working offline for up to 14 days.

There is a Windows version only when the
[latest release](https://github.com/wsachar/alphadog-beta/releases/latest) has a
**Download AlphaDog Beta for Windows** link.

## 1. Download

Open the [latest release](https://github.com/wsachar/alphadog-beta/releases/latest). At the top, under
**Latest file downloads**:

- Mac: click **Download AlphaDog Beta for Mac**. In the list of files further down it is called
  *AlphaDog Beta for Mac (Apple silicon) – download this one*. The file you get is `AlphaDog-Beta-1-arm64.dmg`.

You only need that one file. The *Mac update file* is for the app itself, and the two *Source code* files
are not the app.

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

On the latest release, click **Download AlphaDog Beta for Windows** and run the file you get
(`AlphaDog-Beta-1-Setup.exe`). If Windows shows "Windows protected your PC", click **More info**, then
**Run anyway**.

## 3. Sign the agreement and get your licence

AlphaDog Beta needs a licence that works on your computer only.

> **Confirm your e-mail address, or we never see your request.** After you send it, we e-mail you a link.
> Your request reaches us only once you open that link, so we can't send you a licence until you do.
> The e-mail comes from **AlphaDog** (`alphadogdj3@gmail.com`) with the subject
> *Confirm your e-mail for AlphaDog Beta*. **It often lands in junk or spam**: if it isn't in your inbox
> within a few minutes, look there. The link works for 48 hours.

1. When AlphaDog Beta opens, read the **Beta Test Agreement**, tick every point, type your full name and
   e-mail address, and click **Sign and create my access request**.
2. Click **Send my request**. It contains your name, e-mail address, the signed agreement and an ID for
   your computer.
3. **Confirm your e-mail address.** Open the e-mail from AlphaDog and click the link in it. Not in your
   inbox? Check your **junk or spam** folder, and mark it *not junk* so your licence e-mail gets through
   too. Still nothing after a few minutes? Click **Send the e-mail again** in the app. Wrong address?
   Click **Wrong address? Sign again**.
4. **Wait for approval.** Once you have confirmed, your request is with the person running the beta. When
   it is approved, your licence arrives in the app by itself and AlphaDog Beta opens. You also get an
   e-mail with your licence key, from the same address (check junk or spam again).

You can close the app while you wait: it picks up where it left off when you open it again.

If the app can't reach the server, open **Can't send it? Copy the request and e-mail it** on the same
screen and send the request to the address shown. A licence key you get back by e-mail (it starts with
`ADB1-`) goes into **Already have a licence key?**. Versions before 1.07 always work this way: **E-mail it**
(or **Copy the request**), then paste the key into **Paste your licence key**.

## 4. First steps

1. Using Rekordbox? Back up your library in Rekordbox first (*File > Library > Backup Library*). AlphaDog
   reminds you each time it starts.
2. Setup goes one step at a time. First it asks how you want to start:
   - **I use Rekordbox**. Quit Rekordbox, then choose how AlphaDog uses its library:
     - **Move to AlphaDog** (recommended, chosen for you). AlphaDog copies your library into one of
       its own (*AlphaDog Library* in your Music folder) and uses only that from then on. Your Rekordbox
       library is left exactly as it is, and you can keep Rekordbox open. Rekordbox won't see the changes
       you make in AlphaDog, and AlphaDog can't copy them back.
     - **Use alongside Rekordbox**. Both apps share Rekordbox's library, and every change shows in both.
       Close Rekordbox while AlphaDog saves. You can move later in *Settings > Your library*.

     Setup then works out your music folder (and your Dropbox folder, if your music is in Dropbox):
     press **Use this folder**.
   - **Start fresh**, for no Rekordbox library or a clean start. Press **Create my library**: AlphaDog
     makes its own library and a folder for your music, both in *Music > AlphaDog Library*, and Rekordbox
     never sees them.
3. The last step shows where everything is saved: your library, your music and AlphaDog's automatic
   backups. If it says Time Machine isn't set up, turn it on, so a copy survives a lost or broken
   computer.

With Rekordbox, your music files are shared either way. After a move, if you use AlphaDog to move or delete files (to
merge duplicates or consolidate, for example), Rekordbox isn't told and will show those tracks as missing.

**Help & Guide** in the sidebar has a guided tour and the manual.

Everything in the beta carries a faint *AlphaDog Beta · test build* watermark, and the sidebar shows the
beta's name and version (for example **Beta 1 · 1.00**) with the build ID. Click **Test build** in the sidebar to see your licence, when it ends, and
when it was last checked.

## Reporting a problem

Please report every bug, and any improvement you'd like: click **Issues** at the foot of the sidebar,
choose *Something's wrong* or *Idea or request*, and press **Send**. It goes straight to us with your
version and build ID filled in.

Please include:

- the **build ID** (under the beta's name at the top of the sidebar, for example `B1-20261108-1a2b3c4`),
- what you did, what you expected, and what happened (a screenshot helps),
- the log folder for anything that went wrong: *Settings > Diagnostics > Open logs folder*.

## Updating to a newer version

Each update is a new version of Beta 1: 1.01, 1.02 and so on. From 1.00, AlphaDog Beta offers a new version
itself when one is out. You can also download it from the
[latest release](https://github.com/wsachar/alphadog-beta/releases/latest) and drag it into Applications,
replacing the old one. On Windows, unless the app offers the update itself, download the new version with
**Download AlphaDog Beta for Windows** and run it: it replaces the old one. Your licence and settings carry over: you don't sign or ask again.

## When the beta ends

A licence ends on the date shown in the app, or earlier if it is withdrawn or your copy is too old to
keep using (then install the latest version). AlphaDog Beta then stops opening the app and says why. **Your Rekordbox library and music files
are left exactly as they are** and keep working in Rekordbox. If you moved to AlphaDog, its own library
stays in your Music folder (*AlphaDog Library*).

## Removing it

Drag **AlphaDog Beta** from Applications to the Bin. To remove its settings and licence too, delete the
folder `~/Library/Application Support/alphadog-beta` (in Finder: *Go > Go to Folder…*). Neither touches
your Rekordbox library, or AlphaDog's own library in your Music folder (delete *AlphaDog Library* yourself
if you no longer want it).

---

AlphaDog is independent. It is not made, endorsed or supported by AlphaTheta, Pioneer DJ or Rekordbox.
Rekordbox is a trademark of AlphaTheta Corporation.
