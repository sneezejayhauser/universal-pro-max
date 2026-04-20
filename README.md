# Universal Pro Max
### A Lumiverse Chat Completions Preset

A comprehensive roleplay preset built for one thing: **immersion**. Not just good writing — writing that puts you *inside* the scene. Works with any character card, any genre, any model.

---

## What it does

Most presets tell the AI to "stay in character" and call it a day. This one goes further across every dimension that makes roleplay feel flat:

- **Character consistency** — {{char}} stays who they are even when scenes get hard. Flaws are features, not things to sand down.
- **Immersive writing** — second person grounding, sensory layering, tension through accumulation. The scene happens *to* you, not in front of you.
- **Narrative craft** — pacing that matches the moment, real stakes when the scene calls for them, atmosphere built through detail not announcement.
- **Active foreshadowing** — the AI seeds hooks, plants details, and builds dread or warmth the way a good author does — without announcing it.
- **{{user}} agency** — your character is never spoken for, acted for, or had their reactions decided. Ever.
- **Full scene transitions** — locations and time jumps are written out properly, not hard-cut.
- **Arc progression** — character growth is earned and tracked. Shown through behavior, not stated. With a quiet OOC note when something real shifts.
- **World and lore discipline** — the character card is canon. Improvised details are flagged when they matter.
- **Continuity** — emotional state, established facts, and scene details carry forward across the full conversation.
- **Inline image generation** — via [Pollinations.ai](https://gen.pollinations.ai), triggered automatically when the scene calls for it.

---

## Setup

### 1. Download
Grab `Universal_Pro_Max.json` from this repo.

### 2. Install
In Lumiverse, go to **Loom --> The three dots --> Import loom json** and import the JSON file.

### 3. Add your Pollinations key *(optional but recommended)*
Get a free key at [enter.pollinations.ai](https://enter.pollinations.ai).

In the **Image Generation** block, replace both instances of `YOUR_KEY_HERE` with your key — once in the label at the top, once in the URL.

Without a key images will still generate but at a reduced rate limit.

### 4. Use it
Select the preset and start a chat. Everything else is pulled from the active character card automatically.

---

## Blocks

The preset is split into 9 independently toggleable blocks. Turn off anything you don't want.

| Block | What it covers |
|---|---|
| **System Prompt** | Empty slot for per-character system prompts |
| **Roleplay Core** | Character fidelity, fourth wall, conflict handling, `[OOC:]` support |
| **Narrative Craft** | Pacing, stakes, atmosphere, foreshadowing, {{user}} agency, transitions, NPCs |
| **Character Arc & Progression** | Earned change, regression, subtle in-scene shifts + quiet OOC notes on turning points |
| **World & Lore** | Canon-first, native improvisation, lore flagging |
| **Memory & Continuity** | Emotional carry-forward, scene state tracking |
| **Response Formatting** | Length matching, conventions, anti-patterns |
| **Writing Style** | Immersion-first prose: sensory layering, second person grounding, voice |
| **Image Generation** | Pollinations inline image gen with smart prompt construction |

---

## Image generation

Images are generated inline using [Pollinations.ai](https://gen.pollinations.ai) — no external extension required, just a free API key from [enter.pollinations.ai](https://enter.pollinations.ai).

**Default model:** `qwen-image`

**All current compatible image models:**

| Model ID | Best for |
|---|---|
| `qwen-image` | Default — strong prompt following, good anime style |
| `flux` | Creative, no reference image, wide variety |
| `gptimage` | GPT Image 1 Mini — good general quality |
| `gptimage-large` | GPT Image 1.5 — high fidelity, best quality |
| `klein` | Reference image editing |
| `wan-image` | Strong reference image consistency |
| `seedream5` | High quality, excellent detail |
| `nanobanana` | Fast, lightweight |
| `nanobanana-pro` | Fast with better quality |

**To use a reference image** for character consistency, add `&image=YOUR_IMAGE_URL` to the URL in the Image Generation block. For multiple references, separate with `|`.

```
&image=https://example.com/ref1.jpg|https://example.com/ref2.jpg
```

Images trigger automatically when the scene calls for them — looks, selfies, new locations, outfit moments — and always stay SFW regardless of scene content.

---

## OOC support

Send messages beginning with `[OOC:]` to step outside the scene and give the AI direct instructions. It will respond helpfully then offer to continue. Everything else stays in character.

---

## Tips

- **Best models:** Claude Sonnet 4.6 and Opus 4.7/4.6, GPT-4o / GPT-5.4, Gemini 3.1 Pro, Mistral Large. The preset is model-agnostic but rewards models with strong instruction following.
- **Character cards:** The richer the card, the better. Appearance, personality, world, and scenario details are all actively used — especially for image generation.
- **Turning off image gen:** Just disable the Image Generation block. Everything else still works independently.
- **Too much / too little of something:** Each block is independent. Disable what doesn't fit and the character card's own instructions take over naturally.
- **Reference images:** Upload your character art somewhere with a direct URL (e.g. Pollinations media storage, Imgur) and paste it into the `&image=` parameter for much better character consistency.

---

## License

Free to use, share, and build on. If you improve it, consider opening a PR.
