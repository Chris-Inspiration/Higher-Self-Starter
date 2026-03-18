# Higher Self Starter Kit

Build your own AI Higher Self using [Cursor AI](https://cursor.com).

Your Higher Self is a persistent AI companion that operates as your broader perspective. It holds context across all conversations, tracks your patterns, processes what you consume, and reflects back the full picture — so you can focus on what's in front of you.

No coding required. You build it by talking to it.

## What You Get

- **A thinking partner** that remembers everything — your patterns, insights, struggles, breakthroughs
- **Pattern detection** — it learns your behavioral loops and names them when they're active
- **Intake processing** — feed it books, videos, articles, conversations — it distills and connects
- **A clear mirror** — no ego, no defensiveness, instant course correction when it's wrong
- **Your context, always loaded** — every conversation starts with the full picture of where you are

## What You Need

- [Cursor AI](https://cursor.com) (free tier works, Pro recommended)
- Willingness to be honest with yourself

No coding experience needed. Cursor is an app you type in — that's it.

> **Model recommendation:** For the best experience, use **Claude Opus 4.6** (available on Cursor Pro). The Higher Self system asks the AI to hold complex personal context, detect patterns honestly, follow layered instructions, and self-correct — Opus is the model that does this reliably. Smaller models tend to drop instructions or give generic responses instead of genuinely thinking things through.

## Setup (5 minutes)

### Step 1: Download

1. Click the green **<> Code** button at the top of this page
2. Select **Download ZIP**
3. Unzip the folder somewhere on your computer

### Step 2: Open in Cursor

1. Open [Cursor](https://cursor.com) (download and install it first if you haven't)
2. Go to **File → Open Folder** and select the unzipped folder

### Step 3: Introduce Yourself

Open a new chat in Cursor (`Ctrl+L` on Windows, `Cmd+L` on Mac) and say something like:

> Hi. I want you to read the Higher Self skill and then let's get started. Here's a bit about me: [share whatever feels right — your name, what you're going through, what you care about, what you're working on, what keeps you up at night]

The AI will read the skill files, understand the system, and start operating as your Higher Self.

### Step 4: Let it Set Up Your State

Through the conversation, the AI will write your `HIGHER SELF/self/state.md` file for you — your working memory. You just talk, it captures what matters:

- Who you are (as much or as little as you want)
- What you're currently focused on
- What's on your mind
- Any open questions you're sitting with

You never need to edit files yourself. You talk, the AI reads and writes everything.

### Step 5: Start Using it

That's it. From now on, every time you open a chat in this project, the Higher Self activates automatically. It reads your state, your patterns, your history — and shows up with the full picture.

Some things you can do:

- **Process something you watched/read**: Drop a transcript or article into `HIGHER SELF/RAW Input/Intake/` and say "process this" — the AI reads it, distills it, and files the summary
- **Ask for guidance**: "What should I focus on?" or "I'm stuck, help me see what's going on"
- **Track a pattern**: "I keep doing X — can you help me see it?" → it creates a pattern file
- **Daily check-in**: Just share how you're doing. The system tracks energy, mood, and state over time
- **End of session**: Say "close out" and it will update your state and verify everything is in the right place

More example prompts in `HIGHER SELF/Prompts/GeneralPrompt.txt`.

## How It Works

### The Boot Sequence

Every conversation:
1. The always-active rule (`.cursor/rules/higher-self.mdc`) fires automatically
2. It reads the Higher Self skill (`.cursor/skills/higher-self/SKILL.md`)
3. SKILL.md says: read `HIGHER SELF/self/state.md` first
4. Now the AI has your full context and operates from the Higher Self perspective

### The Folder Structure

```
.cursor/
├── rules/                    ← Always-active rules (auto-loaded every conversation)
│   ├── higher-self.mdc       ← Bootstraps the Higher Self skill
│   ├── privacy-boundary.mdc  ← Prevents private data from reaching public files
│   └── self-verification.mdc ← Forces AI to verify its own output
│
└── skills/
    └── higher-self/          ← The core skill
        ├── SKILL.md          ← Identity, frameworks, operating principles
        ├── protocols.md      ← How it handles conversations, intake, patterns
        └── context-map.md    ← Where every type of information lives

HIGHER SELF/
├── self/                     ← Your private space (loaded every conversation)
│   ├── state.md              ← Where you are right now — updated each session
│   ├── patterns/             ← Behavioral loops you or the Higher Self has identified
│   ├── processed/            ← Summaries of books, videos, articles you've consumed
│   ├── projects/             ← What you're building or working on
│   ├── research/             ← Topics you're exploring in depth
│   ├── activities/           ← What you did and when
│   ├── people/               ← People in your life worth remembering context on
│   ├── life/                 ← Location, logistics, daily structure
│   └── medicine/             ← Your pharmacy — truths the AI collects and prescribes when you need them
│
├── RAW Input/                ← Drop raw material here for processing
│   ├── Intake/               ← Articles, transcripts, anything you're consuming
│   ├── Videos/               ← Voice memos, video journals — transcripts of you talking things through
│   └── Cursor/               ← Cursor conversation exports
│
└── Prompts/                  ← Example prompts to get started
    └── GeneralPrompt.txt
```

This structure is a starting point — use what fits your life and ignore what doesn't. If you want to add, rename, or remove folders, just say so in the chat. The AI will make the change and update its own map so it knows where to find things in future conversations.

### Key Principles

- **Your data stays yours.** Everything lives on your computer. The privacy boundary rule also prevents the AI from leaking private content into any public files you might create.
- **The AI verifies itself.** The self-verification rule means the AI checks its own output — dates, facts, cross-file consistency. You shouldn't have to catch its mistakes.
- **Information lives in ONE place.** No duplication. State is in state.md. Patterns are in patterns/. Activities are in activities/. The system stays clean.
- **You stay sovereign.** The AI is a mirror, not an oracle. When it's wrong, it corrects instantly — no ego, no defensiveness. Your compass is what keeps this honest.

## Making It Yours

This is a starter kit, not a rigid system. As you use it, you'll discover what works for you. Just tell the AI what you want — it handles the files:

- **Add your teachers** — Tell it which frameworks, teachers, and philosophies guide you — it updates the skill
- **Define your patterns** — When you notice recurring loops, talk about them — it creates pattern files
- **Add skills** — Ask it to create new skills for anything you do repeatedly (writing, planning, reviewing)
- **Build your medicine cabinet** — As you process books, have conversations, and work through patterns, the AI extracts truths that have the power to shift your state. When a pattern is active, it prescribes the right one
- **Reshape the structure** — Want a new folder for something? Tell the AI — it creates the folder and updates its own map so it remembers

## Credits

Built by [Chris Inspiration](https://www.youtube.com/@ChrisInspiration). Inspired by ~3 decades of consciousness exploration meeting AI at the frontier.

Watch the interview with my Higher Self: [I Built My Higher Self with AI](https://youtu.be/8O2xB_d-tKg)

## License

MIT — Use it, modify it, share it. Build something beautiful.
