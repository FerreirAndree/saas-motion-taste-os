# Teardown: Zelios — iBanPay / iBanFirst-adjacent fintech SaaS demo

**Reference:** [YouTube — “SaaS Demo Video Example for Fintech Companies”](https://www.youtube.com/watch?v=wwIt5ZvROrs) (`wwIt5ZvROrs`)  
**Attributed production:** Zelios (per video description); client/product framed as **iBanPay** in on-screen UI and **iBanFirst** in surrounding marketing materials.  
**Stated runtime (platform metadata):** ~00:48  
**Local mp4 path (intended):** `references/source-videos/zelios-ibanpay.mp4` (local-only; **do not commit**)  

**Keyframes / contact sheet folder:** `references/teardowns/keyframes/zelios-ibanpay/`

---

## Source integrity & methodology (read first)

In this workspace, **direct acquisition of the full mp4 failed** (`yt-dlp`, `you-get`, captions/transcript APIs, and headless embed playback all returned `LOGIN_REQUIRED` / bot or player-configuration blocks typical of cloud-provider IPs).  

This teardown therefore rests on **high-signal public stills** (YouTube poster + auto-generated thumbnails **1–3**) plus **platform metadata** (title, description, category keywords). That is enough to analyze **composition, UI staging, hierarchy, and visual-system choices** with professional rigor, but it is **not** a frame-by-frame timing trace.

**Timestamp ranges below are *estimated* beats** for a ~48s launch/demo shape. They are useful as a **storyboard hypothesis** until you regenerate them from a local file with `ffprobe` + `ffmpeg`.

### Regenerate artifacts locally (when `zelios-ibanpay.mp4` exists)

```bash
ffprobe -hide_banner references/source-videos/zelios-ibanpay.mp4

ffmpeg -i references/source-videos/zelios-ibanpay.mp4 \
  -vf "fps=1/3,scale=480:-1,tile=5x6" \
  -frames:v 1 references/teardowns/keyframes/zelios-ibanpay/contact-sheet-full-video.jpg

ffmpeg -i references/source-videos/zelios-ibanpay.mp4 -ss 00:00:05 -vframes 1 references/teardowns/keyframes/zelios-ibanpay/kf-VERIFY-00m05s.jpg
# repeat -ss for each confirmed beat boundary
```

### ffprobe target fields (pending local mp4)

Once the file exists, record:

| Field | Command note |
| --- | --- |
| Duration | `ffprobe -show_entries format=duration -v quiet -of csv=p=0 …` |
| Resolution | `ffprobe -select_streams v:0 -show_entries stream=width,height …` |
| Frame rate | `ffprobe -select_streams v:0 -show_entries stream=r_frame_rate,avg_frame_rate …` |
| Audio | `ffprobe -show_streams` → confirm `codec_type=audio` |

**Audio presence (inferred):** *Likely* yes for a Zelios-packaged demo (VO/music), but **unconfirmed** without the muxed file.

---

## Artifact map (what is committed)

| File | Role |
| --- | --- |
| `contact-sheet.jpg` | **Four-up contact sheet** stitched from public stills (not a full-video time sample). |
| `youtube-maxresdefault.jpg` | High-res poster frame (primary “invoice lift” still). |
| `youtube-thumb-1.jpg` | Low-res auto still A — layered 3D stack + AI/chat proof. |
| `youtube-thumb-2.jpg` | Low-res auto still B — alternate crop of mail/invoice beat. |
| `youtube-thumb-3.jpg` | Low-res auto still C — mobile row + typographic “Pay”. |

---

## Beat teardown (estimated timeline; verify locally)

> **Legend:** Each beat lists the judgment categories requested in the brief. Where motion must be inferred from stills, it is labeled **(inferred)**.

### Beat 1 — “Intelligent stack” (AI + multi-surface depth)

**Time (estimated):** 0:00–0:12 *(verify)*  
**Beat name:** Hook — conversational finance agent inside a layered product world  

**Narrative purpose:** Establish *category* (AI-assisted financial ops) and *production value* (dimensional UI, glow-as-signal) before proving mundane software truth.  

**First read:** A single conversational bubble demanding confirmation — *payment intent is the stakes*.  
**Second read:** A robotic “agent” avatar and stack of glassy panels imply **orchestration** across multiple surfaces (not one flat screenshot).  

**Composition:** Isometric / off-axis **multi-plane** staging; strong **Z-depth**; purple **rim light** entering from the rear/left; hero bubble and agent head occupy **upper-right golden zone** while panels recede bottom-left.  

**Camera behavior:** **Static hold** or **very slow push** *(inferred)* — the depth sells scale, not a whip move. Shallow depth-of-field on thumbnails suggests **cinematic focus pull** is plausible between planes *(inferred)*.  

**Primary motion:** Chat text **types** or pops; AI head **activates**/glows; connector lines **pulse** along graph edges *(inferred)*.  

**Secondary motion:** Panel stack **parallax micro-drift**; soft **light sweep** across glass; tiny UI affordances (dots, pills) **breathe** *(inferred)*.  

**Transition in:** Hard cut or **light bloom into frame** from black/gradient *(inferred)* — typical for portfolio-grade hooks.  

**Transition out:** **Depth dive** toward the next, more literal desktop surface; *or* **match glow angle** into the next scene’s key light *(inferred)*.  

**Product truth:** The hook is *plausible finance behavior* (“confirm the payment…”) rather than abstract “AI sparkles.” It binds intelligence to **a decision moment**.  

**Typography behavior:** Conversational copy behaves like **product UI**, not a marketing caption — high trust if VO aligns. Subheaders/labels stay **small and functional** in the stack *(inferred)*.  

**UI/product treatment:** Hybrid **symbolic + literal**: readable message thread + semi-abstract surrounding modules. This matches *Cleaned UI* / *Abstracted UI* crossover in `references/product-ui-treatment.md`.  

**Premium signal:** **Expensive negative space** between modules; **one** purple accent system; reflections feel **consistent** with a single light direction.  

**Reusable principle:** *Lead with a **decision interrupt** (confirm/approve/verify), not a feature list — then show the interface that resolves the interrupt in Beat 2+.*  

**What not to copy:** The robot avatar metaphor, exact palette, and specific panel topology — take the **interrupt → proof** story shape only.  

---

### Beat 2 — “Desk truth” bridge *(inferred between hook and invoice proof)*

**Time (estimated):** 0:12–0:22 *(verify)*  
**Beat name:** Continuity bridge — moving from “AI layer” to “application layer”  

**Narrative purpose:** Hand attention from **conceptual intelligence** to **credible software** so the viewer believes the next UI beat.  

**First read:** A familiar **desktop productivity shell** begins to dominate frame.  
**Second read:** Chrome/toolbars imply **real work context** (send / sign / attach).  

**Composition:** **Single hero surface** begins to flatten perspective slightly; **left sidebar** returns as anchoring element in later stills.  

**Camera behavior:** **Lateral drift or yaw** that “lands” the viewer on the mailbox chrome; or **scale bridge** where a stacked layer expands into the full window *(inferred)*.  

**Primary motion:** Window **settles**; toolbar icons **resolve** from simplified blocks *(inferred)*.  

**Secondary motion:** Ambient **cursor idle** or **draft autosave** tick *(inferred)*.  

**Transition in:** **Spatial continuation** from Beat 1’s left-right lighting into the mail window’s left glow.  

**Transition out:** **Object lift** begins — PDF card **separates** from the canvas.  

**Product truth:** Signals **operational reality** (documents, recipients, actions).  

**Typography behavior:** Functional labels **lock to toolbar grid**; no oversized marketing type here *(inferred)*.  

**UI/product treatment:** Moves toward *Cleaned UI*: keep toolbar readable; remove inbox noise later.  

**Premium signal:** Restraint — **no duplicate headline** over the UI.  

**Reusable principle:** *Use a short bridge beat to change **fidelity level** (abstract → literal) without a meaningless transition.*  

**What not to copy:** Any specific iconography pack; invent your own coherent desktop language.  

---

### Beat 3 — “Lifted invoice” (concrete proof)

**Time (estimated):** 0:22–0:36 *(verify)*  
**Beat name:** Feature proof — document becomes the protagonist  

**Narrative purpose:** Prove **payment-adjacent workflow clarity**: a specific document, a specific counterparty email, a specific amount.  

**First read:** **Floating PDF invoice** in sharp focus with a **large purple total** ($15,500 in the poster still).  
**Second read:** Background mail UI is **deliberately de-resolved** (skeleton rows / blur) so parsing stays on the invoice.  

**Composition:** Classic **hero object** layout: centered-right card, **generous headroom**, mailbox sidebar anchoring left edge; **cursorHand** underscoring interaction.  

**Camera behavior:** Slight **camera push** or **dollying-in** while depth-of-field **thins** background clutter; or static camera with **card z-pop** only *(both plausible)*.  

**Primary motion:** Card **lifts on Z**; shadow **deepens**; cursor **settles** under the object implying drag/select semantics *(inferred)*.  

**Secondary motion:** Sidebar list **micro-scroll**; ambient shimmer on glass toolbar *(inferred)*.  

**Transition in:** **Expand** from list row **or** **match-cut** PDF glyph outline from prior icon.  

**Transition out:** Card **recedes** into send flow / payment rail / confirmation state *(inferred)*.  

**Product truth:** Strong — shows **recipient addressing** (`…@ibanfirst.com`), **transaction-scale number**, and **document type**. This is *Input → Output* proof (`references/product-ui-treatment.md`).  

**Typography behavior:** Hero numerics inside the PDF, not a external caption — **type integrated with the artifact**. Toolbar words (“New mail”, “Send”, “Sign”) behave as **microcopy**, spaced for scannability.  

**UI/product treatment:** *Cleaned UI* exemplar: **skeleton inbox** to reduce chart junk; crisp **macOS traffic lights** sell “real app.”  

**Premium signal:** **Optical hierarchy** via blur, not via brute-force dimming entire frame.  

**Reusable principle:** *When proving finance UX, **promote the document** to a physical object: mass, shadow, cursor, and a single highlighted numeric.*  

**What not to copy:** Exact totals, filenames, or email strings — they are client-specific narrative props.  

---

### Beat 4 — “Pay channel grid” (breadth / resolve)

**Time (estimated):** 0:36–0:48 *(verify)*  
**Beat name:** Platform breadth + typographic category stamp  

**Narrative purpose:** Communicate **multi-channel payout/payment** reach (mobile shells) while leaving the viewer with a **single word memory**: “Pay.”  

**First read:** Large **PAY** headline in clean sans; **three** framed phone states in a balanced row.  
**Second read:** Purple **brand field** supports the devices; screens show **app-store polish** not debug UI.  

**Composition:** **Symmetrical** triptych with **center-weighted** typography — more editorial than beats 1–3.  

**Camera behavior:** **Static** or **micro push** on the word; phones may **stagger in** on Y with small delays *(inferred)*.  

**Primary motion:** Phones **rise + settle**; PAY **tracks in** or **masks on** with crisp easing *(inferred)*.  

**Secondary motion:** Soft **gradient drift** in background; subtle **screen glare** pass *(inferred)*.  

**Transition in:** **Scale jump** from desktop world to mobile *(cut is OK here — channel shift justifies it)*.  

**Transition out:** Cut to **logo resolve / URL / CTA** *(inferred)* — not visible in stills.  

**Product truth:** **Symbolic** more than literal — reads as *coverage* and *touchpoints*. Pairing it after Beat 3 prevents “fake UI” feelings because credibility was already earned.  

**Typography behavior:** **Editorial display** word; likely **held** long enough to read despite device motion — good pacing instinct if true.  

**UI/product treatment:** *Symbolic UI* — acceptable as **evidence of platforms**, not feature truth.  

**Premium signal:** **Few moving layers**; typographic precision; devices share **one radius / one bezel language**.  

**Reusable principle:** *After a literal proof beat, you may go **symbolic** — but only if you already showed **one** undeniable “real” artifact.*  

**What not to copy:** The exact “PAY” lockup and triptych balance — take the **pattern** (literal proof → symbolic breadth).  

---

## Synthesis

### Narrative spine

**Interrupt (confirm payment) → Orchestration (AI + stack) → Desk reality (mail/productivity chrome) → Concrete document proof (invoice lift) → Multi-channel resolve (“Pay”).**  
It is a textbook **tension → agent/system → operational proof → scale memory** arc for sub-60s fintech SaaS.

### Signature choreography patterns

- **Lifted document hero** (Feature Proof / shallow DOF) — see `references/shot-archetypes.md` *Feature Proof Moment* + *Hero Object Reveal* hybrid.  
- **Attention ladder** from *Abstract stack → Literal window → Isolated artifact* (`references/choreography-patterns.md`).  
- **Cause-and-effect staging** implied: message/confirmation context → concrete payable object.

### Camera language

- Early: **isometric depth** to sell “system.”  
- Mid: **orthographic / shallow 3/4** desktop truth.  
- Late: **flat editorial** for brand typography.  
This trio keeps the film from becoming *only* fly-through or *only* screen record.

### Transition grammar

- Favor **motivated depth** (layer stack to window) over random wipes.  
- Where fidelity jumps (desk → phones), **hard cuts** are acceptable because **channel semantics** change (`references/choreography-patterns.md` *Continuity Rules* — justify eye jumps with meaning).

### Timing / rhythm profile *(inferred)*

- **Hook density higher** (multiple glowing edges, implied particle/connect line activity).  
- **Proof beat slower**, with **micro-pause** on the invoice amount.  
- **Resolve beat cleaner**, fewer simultaneous motions — aligns with *Calm Confidence* + *Product Momentum* hybrid in `references/timing-rhythm.md`.

### Visual system notes (`references/visual-system.md`)

- **Single accent hue** (purple) functions as *active finance emphasis* + *brand glow*.  
- **Glass + matte paper** material contrast (panels vs invoice).  
- **Light direction continuity** left→center across beats strengthens premium cohesion.

### Top 10 reusable principles

1. **Open on a decision**, not a logo — *confirm/approve* beats *hello world*.  
2. **Change fidelity on purpose**: symbolic stack → literal chrome.  
3. **Skeletonize** surrounding UI before you **heroize** a document.  
4. **Promote data** (amount, recipient) *inside* the artifact, not only as captions.  
5. **Depth-of-field is hierarchy**, especially in finance where tables kill focus.  
6. **Cursor as honest interaction** — oversized stylized cursor reads as demo clarity, not game UI, if motion is decisive.  
7. **One accent color** doing structural work (highlights, glow edges) rather than rainbow states.  
8. **Bridge beats** can be invisible if lighting and spatial zones *match* across cuts.  
9. **After literal proof**, symbolic app-grid shots land as *breadth*, not fakery.  
10. **Typography behaves in three registers**: chat microcopy, functional toolbar labels, editorial resolve word.

### Anti-patterns avoided (`references/anti-patterns.md`)

- **Generic particle “AI”** without a task — avoided: the bubble asks for **confirmation**.  
- **Equal-weight interface** — avoided via skeletonization + lifted hero card.  
- **Fake chart soup** — not evident in captured stills.  
- **Template slide transitions** — stills suggest **spatial** and **focal** continuity instead.

### What this teaches future SaaS launch videos

- Treat **payments/finance** as **objects with state** (invoices, approvals), not abstract arrows.  
- **Earn symbolic shots** with **one** brutally specific UI beat first.  
- **Pair atmospheric glow** with **literal chrome** — atmosphere without evidence reads as stock; evidence without atmosphere reads like a Loom.

---

## Self-critique (using `references/critique-rubric.md`)

**Context:** Scores below judge the **visible direction in committed stills** plus **high-confidence motion grammar** for this studio category. They are **not** a substitute for audio/VO/cut-timing review on the full master.

| Category | Score (1–5) | Notes |
| --- | ---: | --- |
| 1. Product Truth | **4** | Concrete invoice + recipient + amount; earlier stack beat is more symbolic but anchored to a payment prompt. |
| 2. Narrative Spine | **4** | Clear escalation from intelligence → literal workflow → proof → breadth, though exact VO/cut order unconfirmed here. |
| 3. Visual Hierarchy | **5** | Exceptional first/second reads in invoice beat; strong focal routing in AI stack. |
| 4. Motion Motivation | **4** | Inferred motion matches causality; risk is AI stack beat drifting decorative if animation overshoots. |
| 5. Timing & Rhythm | **3** | Cannot score precisely without master; structurally sound beat types. |
| 6. Typography & Copy | **4** | Typography mostly integrated; depends on VO/text density in final 10s. |
| 7. Product UI Treatment | **4** | Credible cleaned UI + purposeful abstraction; mobile row is symbolic by design. |
| 8. Finish & Polish | **4** | Lighting/modeling read premium; verify shadow consistency across longer shots. |
| 9. Camera & Staging | **4** | Multi-beat camera strategy is literate; avoid over-orbiting if present in unseen segments. |
| 10. Product Insight Quality | **4** | Details feel buyer-real (domain email, invoice semantics), not lorem dashboards. |

**Overall diagnosis:** This reference demonstrates **finance-grade hierarchy**—especially the **document-as-hero-object** beat—which is portable across many B2B launches. The main creative risk (unverified on full timeline) is the **AI persona** beat becoming glossy without tightening to **one workflow consequence**.

**Highest-impact findings (severity-ordered):**

1. **Proof density timing:** Ensure the **invoice amount** receives a **hold** that satisfies VO + scan time (`references/typography-layout.md`).  
2. **Stack beat discipline:** If connector lines multiply, they must **trace one causal path**, not wallpaper (`references/anti-patterns.md` *Constant Motion*).  
3. **Resolve specificity:** If “Pay” ends the film, pair with **one** product noun or logo frame so memory is *named*, not purely categorical.

**Recommended fixes if adapting (not copying) this template to another product:**

- Replace robot metaphor with **your** system metaphor (workflow graph, ledger timeline, policy gate) while **keeping the confirmation interrupt**.  
- Swap invoice for **your** proof artifact (contract, receipt, FX quote, policy packet).  
- Keep **one symbolic breadth shot**, but show **your** real connectors/integrations list at least once.

**Residual risk:** Without the full muxed file, this teardown cannot certify **audio mix**, **exact VO cadence**, or **micro-edit quirks** (rolled credits, end cards, platform bugs).

---

## Reusable pattern cards (`references/output-contracts.md` style)

```text
Reusable pattern: Document lift + shallow DOF inbox
Why it works: Forces a finance audience to see one deterministic number and party, not a wall of rows.
Where to use it: AR/AP, bill pay, treasury, invoicing, approvals.
Where not to use it: Deep multi-module ERP tours where relationships, not single docs, are the hero.
Adaptation note: Change doc type + numeric emphasis field (FX rate, fee, tax, margin).

Reusable pattern: AI stack → literal app bridge
Why it works: Sells vision then grounds it before skeptics dismiss the hook as vapor.
Where to use it: Copilots, ops agents, finance automation.
Where not to use it: Regulated categories that punish “autonomous” cues without human-in-the-loop proof.

Reusable pattern: Literal proof → symbolic multi-device resolve
Why it works: Breadth reads as availability without pretending each phone UI is a feature demo.
Where to use it: Payments, wallets, mobile-first platforms.
Where not to use it: Single-surface developer tools where mobile implies confusion.
```

---

## Git / storage hygiene

- **Do not commit** `references/source-videos/zelios-ibanpay.mp4` or other raw grabs.  
- **Committed artifacts** here are **small, high-signal JPEGs** supporting critique, not a substitute for the master.  

---

*End of teardown.*
