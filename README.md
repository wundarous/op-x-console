# Operator X Console

A thousand years after the Great Fall, humanity is preparing to leave Earth aboard the ship that nearly destroyed it.

Within the ship's Artifact, millions share an existence beyond the lives they once knew. Joining them requires a state of consciousness few could attain until A-HAVA was built from the old world's surviving VR technology. Guided by AI and human operators, the remaining people work through simulated lifetimes so they too can integrate into the Artifact. Only then can the ship depart.

Operator X is the last operator. She remembers neither her name nor her life before the Artifact, but the work comes naturally—until she is assigned Prisoner 285, a man driven by chaos, violence, and addiction.

X must walk through his recorded lives to reach a mind that has defeated every attempt to help him. As she searches his worlds for a way forward, the other operators reach their limits and retreat into the Artifact. Eventually, only X, the robots, and one unfinished life remain.

**Can she guide the last person into the Artifact before she loses her own way back?**

Told through her recovered console, *The Many Lives of Operator X* follows humanity's journey into the unknown, X's search for her past, and the lives she must enter along the way.

This early preview includes **seven mission days, 21 journal entries, and 23 supporting documents**. The experience runs through conversation with an AI that can read the supplied package. There is no application to compile, server to start, or dependency to install. Your chosen AI service supplies the model and may have its own costs or usage limits.

## Start in an AI chat

1. On this GitHub page, choose **Code → Download ZIP**.
2. Attach the ZIP to a fresh AI chat.
3. Say **“Open the console.”**

That's it. The ZIP includes the story, console instructions, and images—you don't need to unzip it or attach the images separately when your chat can read ZIP files.

If your chat asks what to do with the archive, say: **“Open the ZIP, read operator-x-week-one.txt, and run the console.”**

If your app cannot read ZIPs, extract it and attach `operator-x-week-one.txt` plus the PNGs from `media/` instead. Use a fresh conversation so earlier story discussions don't influence the experience.

## Use a local AI console instead

Download and extract the ZIP, or clone the repository:

```sh
git clone https://github.com/wundarous/op-x-console.git
cd op-x-console
```

Open that folder in your AI tool, start a fresh conversation, and say **“Open the console.”** The included `AGENTS.md` supplies startup guidance for tools that support it. If needed, ask the AI to read `operator-x-week-one.txt` and run its console experience.

## Use the console

Once the console opens, say **Open journal**.

| Command | What happens |
| --- | --- |
| **Open journal** | Displays the next unread journal part. |
| **Continue** | Does the same: advances by one part. |
| **Open document** | Opens the newly announced document, or asks which one you mean. You can also give a title. |
| **Ask a question** | Lets you ask about the story using the records available so far. You can simply type your question. |

A first reading follows this order:

```text
Day 001 · Entry 1 → Entry 2 → Entry 3 → Day 002 · Entry 1
```

After a journal part, the console displays:

---

🔵 **New documents available:** [newly unlocked titles, or none]

🟡 **Available commands**

- Open document
- Open journal
- Continue
- Ask a question

The horizontal divider separates the record from navigation. Blue markers identify new documents, yellow marks the command menu, and red marks errors or unavailable records. These are colored markers; actual text colors depend on the AI app's renderer.

Documents unlock after their associated journal entry is displayed. The console announces only new documents; previously unlocked documents remain accessible by name. Ask to list available documents if you want the full catalog.

To reread a completed day, say **Open journal day 003**. The console shows the full day only if you have already read all three parts. Otherwise, it opens your next unread part in sequence. Rereading does not reset your progress.

The preview ends after Day 007. You can revisit records and ask questions afterward; the AI should not invent Day 008. Asking about the records does not change X's story.

## Orientation diagrams

The campus overview includes a lobby wayfinding panel, library and archive, fitness and sports facilities, a pub, gardens, and walking paths. It unlocks after Day 2 Entry 1. The ship schematic unlocks after Entry 2. A labeled HAVA pod illustration also opens after Entry 1, showing the cover, biofeedback harness, cradle and wired connection. A new “What Is A-HAVA?” introduction follows Entry 3.

All three graphics have PNG viewing copies. The two map diagrams also have SVG originals; the pod is a rendered equipment illustration. The ZIP includes the images in `media/`; no separate image uploads are needed when your chat can read them from the archive. Display support varies by app. Each diagram record includes an authored text description as a fallback. The diagrams are schematics, not measured floor plans.

The **Bring Purpose Back — Advertisement** unlocks after Day 7 Entry 1. Its supplied artwork is `media/bring-purpose-back-advertisement.png`; the archive record also includes the exact advertising copy and an image description.

## Save and resume

Say **Save my position**. Copy the bookmark code the console returns somewhere you can find it later.

To resume in a new conversation:

1. Open the same folder or attach the same package again.
2. Send:

```text
Use operator-x-week-one.txt to resume the Operator X console from this bookmark:
[paste your saved code here]
Show my current status and wait for my choice.
```

The code preserves your reading position and which journal parts have been read. It is a copyable bookmark, not an account login or a server save. Keep it even if you plan to continue in the same chat.

## If the AI gets off track

This is a prototype driven by instructions, so different models may handle it differently. If it prints a whole unread day, repeats a part, or invents information, try:

```text
Follow the package's console instructions. Open journal and Continue display
only one next unread entry. Mark only the entries actually shown as read.
Use the authored record text, and answer story questions only from unlocked
records. Output only the console screen; apply progression and unlock rules
silently. Do not invent missing content.
```

If its progress tracking is unclear, start a new conversation with your last reliable bookmark. An explicit request for unrestricted reading can bypass the intended reveal order within this preview. The narrative locks are not encryption: all seven days are present in the file.

For feedback, note the AI service/model, what you asked, and what it returned. Especially useful: confusing navigation, repeated entries, premature document unlocks, unsupported story answers, and whether you wanted to keep reading.

## Files

| File | Purpose |
| --- | --- |
| [operator-x-week-one.txt](operator-x-week-one.txt) | Complete console instructions and first-week story records. |
| [AGENTS.md](AGENTS.md) | Startup guidance for local AI tools. |
| [START-HERE.txt](START-HERE.txt) | Short version of the startup instructions. |
| [media](media/) | Campus and ship diagrams (PNG/SVG), plus the HAVA pod illustration and Day 7 advertisement (PNG). |
| [LICENSE](LICENSE) | Permissions for using and sharing this package. |

## License

Copyright © 2026 **Six Sided Industries LLC**.

The [Operator X Personal Use License](LICENSE) permits personal, noncommercial use, including use through a paid AI service, and direct free sharing of the unchanged package with friends. Commercial use and public adaptations require separate written permission. This is not an open-source license. See the full license for its scope, exceptions, and terms.
