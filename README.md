# 🌭 Find Him Hot Dog Man

> He is hiding in a crowd of snacks. He has done nothing wrong. He simply does not wish to be found right now. You have five seconds to disrespect that wish.

A browser-based hidden-object game of escalating panic and condiment-based deception. Somewhere in a teeming throng of cheeseburgers, fries, and suspiciously similar wiener-adjacent persons stands the **genuine article** — mustard squiggle, big honest grin, no disguise. Click him before the fuse burns out. Click a fake and you lose time and dignity, in that order.

It is one HTML file. It runs in a browser. It contains a 110-entry dossier, a synthesized soundtrack made entirely of mustard squirts, and a permanent record of every mistake you have ever made. It is, against all odds, a complete video game.

---

## ▶️ Usage

Open `index.html` in a browser. That's it. That's the whole thing.

No build step. No `npm install`. No `node_modules` the size of a small moon. No framework, no bundler, no toolchain that resents you. Just one file and a man who refuses to be located. *(It does politely borrow two fonts from Google over a CDN, which is the single most dependency this project will ever admit to having.)*

---

## 🔎 The Premise

The Hot Dog Man is in there. So are a great many impostors. Your job is to tell the difference quickly and repeatedly while a fuse hisses toward zero.

A small **wanted poster** in the corner shows you exactly who you're after, in case you forget what a dignified hot dog looks like (it happens). Find him, and you advance to a larger, denser, more confusing crowd. Fail to find him, and he strolls off into the great elsewhere, vindicated.

He gets no harder to *recognize*. The crowd just gets harder to *search*.

---

## 🏷️ A Note on the Name

In the upper-left corner of the game sits a small wanted poster. It was built to say two entirely separate things, stacked one atop the other: a quiet instruction — *Find him* — and, beneath it, the name of the person you are to find — *HOT DOG MAN*. An instruction and a label. Two thoughts. Clearly delineated. Obviously, unmistakably distinct.

Nobody read it that way.

Taken top to bottom, with the line break treated as a stylistic flourish rather than a semantic wall, it reads:

> **FIND HIM HOT DOG MAN**

This is not a sentence. It is not quite an instruction. It is not any known convention for naming a video game. It is grammatically suspect and tonally flawless, and the moment it was read aloud as a single title there was no going back.

So that is the name now. The poster is no longer a label — it is the title card, hiding in plain sight in the corner of every round, much like its subject. The author who *built* the poster meant two things; the author who *looked* at the poster saw one; both are credited below and neither regrets it.

We considered fixing it. We did not fix it.

---

## 🎮 The Apparatus

**The Fuse.** Each round is timed. The clock is generous in proportion to the chaos: roughly **5 seconds** for a small crowd, scaling up toward a **12-second** ceiling as the mob thickens. Round one is, and shall always be, the sacred five seconds. The last few ticks blip; the final stretch flashes red; this is your body's reminder that you have committed to this.

**The Crowd.** It swells by six snacks per round and caps out at **90** around round 15. At that point — because the screen is physically full and the man cannot get any smaller without becoming a legal hazard — the clock itself begins to tighten instead, shaving time each round down to a brutal five-second floor. The difficulty never plateaus. It just changes weapons.

**Wrong Clicks.** Clicking an impostor costs you precious seconds and earns you a brief, pointed insult ("That's a TACO"). It also — and this is important — **adds that impostor to your permanent record.** See: The Frankfurter Codex.

---

## 🆘 The Lifelines

Three single-use helpers, one shot each per game. Each attacks the problem from a different angle, because we tried two that did the same thing and a wiser council prevailed:

| Lifeline | What it does |
|---|---|
| **✂️ 50/50** | Vaporizes half the impostors. The weakest helper, and proud of it. |
| **🧭 Quadrant Clue** | Reveals which *quarter* of the screen he's lurking in. The reasonable middle path. |
| **👋 Peekaboo** | The real Hot Dog Man, unable to resist his own manners, pops up and **waves** for about three-quarters of a second. The strongest helper. Use it well. |

**A penalty for leaning on them:** if you use any helper during a round, you **forfeit that round's banked time** (see below). Helpers are a crutch with a cost. The Hot Dog Man respects a clean catch.

---

## ⏳ The Time Bank

Find him with seconds to spare and that leftover time **carries into the next round** (capped, lest you snowball into immortality). A fast clean round buys you a buffer against a cruel one. Use a helper, though, and the bank closes — you'll get a curt "NO BANK · HELPER USED" instead of your reward. The economy is real and it is judging you.

---

## 🫙 The Comeback Bottle

When you are down to your last lifeline (and only from round 10 onward), a **glowing mustard bottle** may appear, hidden in the crowd. Find it and it **refills one of your spent helpers at random** — but the odds are tiered: it'll happily hand back a 50/50, and only grudgingly return a Peekaboo, because Peekaboo is the good stuff. Its appearance odds start modest and *taper* as the rounds climb, so deep runs stay a test of skill, not luck.

---

## 📜 The Intermissions

Every five rounds, the hunt pauses for a **dramatically declassified fact** about the Hot Dog Man, spotlit and typed out one ominous character at a time. There are **110** of them. They range from the plausible —

> The mustard is not a condiment. It is a birthmark.

— to the frankly concerning —

> He is not running from you. He is leading you somewhere.

You collect them as you go.

---

## 📖 The Frankfurter Codex

The game's compendium, openable from the title and game-over screens. It has two tabs:

- **📜 Dossier** — all 110 facts. Locked entries sit redacted behind a ▓▓▓ bar until earned. The game preferentially reveals facts you *haven't* seen yet, so you keep unlocking new lore rather than re-reading old lore.
- **🥸 Suspects** — the full rogues' gallery of **11 impostors**, each with a portrait and a one-line character assassination. Here's the twist: **a suspect only appears in your Codex after you've accidentally clicked it.** The gallery is, quite literally, a museum of your errors. The cool cousin in shades? *"Hides his eyes, not his identity. Certain the shades fool you. They don't."*

---

## 💾 The Save Code

Your progress — facts, suspects, **and** your best score — lives in your browser. But browsers are forgetful and cookies get cleared, so the Codex can **export a ~29-character code** like:

```
HDM3-AQAAAAAAAAAAAgAAACACAokA
```

Paste it back in on any machine to restore everything. Restoring only ever **adds** — it will never lower a fact count, un-log a suspect, or downgrade a best score. The format is forward-thinking and backward-compatible; ancient `HDM1` and `HDM2` codes from the Before Times still import without complaint.

It's a tidy little bitfield with your best score bolted to the end. We are, technically, doing serialization here. For a hot dog.

---

## 🔊 Sound

Two independent toggles in the top ribbon:

- **🔊 Sound** — the blips, splats, and chimes.
- **🎶 Music** — a looping bassline **synthesized entirely from mustard squirts** via the Web Audio API. Each note is a band of filtered noise sweeping downward into a wet tonal blurp. It is exactly as described. It is on by default. We stand by this.

---

## 🛠️ Under the Hood

- **One file.** Vanilla JavaScript, hand-rolled SVG art, Web Audio synthesis, CSS animation.
- **No dependencies to install,** no framework, no build.
- Every character — the Hot Dog Man, all his impostor twins, the snacks, the comeback bottle — is **drawn in code**, not loaded as an image.
- Persists via `localStorage`, degrades gracefully where storage is blocked, and falls back on the save code, which works anywhere.

Pure HTML/CSS/JS. As nature intended.

---

## 🗣️ A Word From the Hot Dog Man

> I was born during a routine bell notification test. I did not ask to be found. I do not consider being found a fixed state. You will click many things that are not me. You will, on occasion, click me. This is the arrangement. I bear no grudge. I am, as ever, doing both.

He earned the hat. It's not in this game, but he earned it.

---

## ❓ FAQ

**Is there a way to win?**
You play until he gets away. The goal is *later*. There is no final round, only the round where you finally blink.

**The mustard bottle never shows up.**
It is gated. You must be down to your last lifeline, at round 10 or beyond, and then it's a tapering coin-flip. It appears for the desperate, not the comfortable.

**I keep clicking the mustache guy.**
Yes. Everyone does. That's why he has a museum exhibit now.

**Can I make the music stop.**
🎶 in the top ribbon. We won't be offended. We will, however, know.

---

## ⭐ Critical Acclaim

> ★★★★★ — "I have reviewed my own pursuit and judged it scrupulously fair. You will not catch me. You are, nonetheless, welcome to try — repeatedly, indefinitely, for the remainder of your natural life."
> — **Hot Dog Man**, Subject · Fugitive · Currently At Large (Both Senses)

> ★★★★★ — "A most diverting amusement. I logged the Cheeseburger as a suspect on sight; the creature plainly lacks breeding. The mustard squiggle, however, is impeccable, and I will hear no criticism of it."
> — **Ronald Percival Augustus Agamemnon**, House Ghost · Butler · Self-Appointed Arbiter of Mustard Standards

> ★★★★★ — "I sat down for five seconds and stood up ninety rounds later. I have clicked the Mustache Guy four hundred times. He is in my Codex. I am, I fear, in his."
> — **A Person Who Should Have Stopped Several Hours Ago**, Verified Wreck

*All testimonials are genuine. None of these individuals exist.*

---

## 🌭 Credits

A hidden-object game in the ongoing saga of a dignified hot dog person.

**Mattie Niznik & Claude — *"It's incredible what we can do."***
