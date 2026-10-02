# Operator X Console

A thousand years after the Great Fall, humanity is preparing to leave Earth aboard the ship that nearly destroyed it.

Within the ship's Artifact, millions share an existence beyond the lives they once knew. Joining them requires a state of consciousness few could attain until A-HAVA was built from the old world's surviving VR technology. Guided by AI and human operators, the remaining people work through simulated lifetimes so they too can integrate into the Artifact. Only then can the ship depart.

Operator X is the last operator. She remembers neither her name nor her life before the Artifact, but the work comes naturally—until she is assigned Prisoner 285, a man driven by chaos, violence, and addiction.

X must walk through his recorded lives to reach a mind that has defeated every attempt to help him. As she searches his worlds for a way forward, the other operators reach their limits and retreat into the Artifact. Eventually, only X, the robots, and one unfinished life remain.

**Can she guide the last person into the Artifact before she loses her own way back?**

Told through her recovered console, *The Many Lives of Operator X* follows humanity's journey into the unknown, X's search for her past, and the lives she must enter along the way.

This early preview includes **seven mission days, 21 journal entries, and 23 supporting documents**. The experience runs through conversation with an AI that can read the supplied text file. There is no application to compile, server to start, or dependency to install. Your chosen AI service supplies the model and may have its own costs or usage limits.

## Get the console

Clone this repository:

```sh
git clone https://github.com/wundarous/op-x-console.git
cd op-x-console
```

Alternatively, download the repository as a ZIP from GitHub and extract it. For the attachment route below, download `operator-x-week-one.txt`, `LICENSE`, and the four PNGs in `media/`. Avoid reading through the package itself if you want to discover the records in order—it contains the whole preview.

## Start in an AI console with local folder access

1. Open the cloned `op-x-console` folder as your local project or working folder.
2. Start a new AI conversation in that folder.
3. Send this prompt:

```text
Read operator-x-week-one.txt and run its fictional recovered-console experience.
Boot at Day 1. Use only the included records for story facts. Follow the package's
reading and document-unlock rules. Do not summarize the package or reveal later
entries. Output only the console screen—no preamble, rule explanations, state
calculations, or implementation commentary. Show the opening console and wait
for my choice.
```

The included `AGENTS.md` provides startup guidance for tools that support that file. The prompt and text package contain everything needed even when your tool does not read `AGENTS.md` automatically.

The AI only needs permission to read this folder. Running the experience does not require editing files, shell commands, web browsing, or access to another project.

## Start in an AI chat using an attachment

If your AI chat can read text attachments, you do not need local project support:

1. Start a fresh conversation.
2. Attach **[operator-x-week-one.txt](operator-x-week-one.txt)** and the four PNG images in **[media](media/)**: `campus-orientation.png`, `ship-orientation.png`, `hava-pod.png`, and `bring-purpose-back-advertisement.png`.
3. Send the same startup prompt above, referring to the attached file.

This route is intended for services such as ChatGPT or Grok when text-file attachments are available in your account. File support and model behavior vary; compatibility with every service is not guaranteed. If the AI cannot read the file, resolve that before beginning rather than asking it to invent the experience.

For a clean test, use a conversation separate from any discussion of the story's development. Do not include authoring files or earlier story discussions. A new folder does not itself isolate account-level memory or other context your AI service may supply.

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

All three graphics have PNG viewing copies. The two map diagrams also have SVG originals; the pod is a rendered equipment illustration. A local reader should use the files in `media/`; in an attachment-based chat, upload the PNGs alongside the text package. Display support varies by app. Each diagram record includes an authored text description as a fallback. The diagrams are schematics, not measured floor plans.

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
