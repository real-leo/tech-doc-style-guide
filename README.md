# English technical documentation style guide (personal/team synthesis)

> **Disclaimer:** This document is an **unofficial personal/team synthesis** based on the Microsoft Writing Style Guide, the Google developer documentation style guide, the Apple Style Guide, and Write the Docs community practices. It is **not** an official Microsoft, Google, Apple, or Write the Docs publication. Rules are drawn from publicly available sources; if anything here conflicts with an official guide’s latest version, follow the official guide.

---

## 1. What this guide is / sources and scope

### 1.1 Purpose

For engineers who write English product help, developer docs, API references, and how-to procedures. This handbook consolidates four major sources into one place so you do not have to switch among them constantly. Explanations are in clear English; examples stay in the original English form used by those guides.

### 1.2 Primary sources

| Source | Focus | Entry point |
|--------|-------|-------------|
| Microsoft Writing Style Guide | Product copy, voice, capitalization, procedures, bias-free language | [Welcome](https://learn.microsoft.com/en-us/style-guide/welcome/) |
| Google developer documentation style guide | Developer/API docs, word list, code, accessibility | [About this guide](https://developers.google.com/style) |
| Apple Style Guide | Apple product and UI copy, terminology, technical typography | [Apple Style Guide](https://support.apple.com/guide/applestyleguide/welcome/web) |
| Write the Docs | Documentation principles, skimmable structure, Docs as Code | [Software documentation guide](https://www.writethedocs.org/guide/) |

### 1.3 Scope

- **In scope:** Feature descriptions, tutorials, step-by-step procedures, concept pages, API/CLI references, error messages, and UI microcopy (in English).
- **Out of scope:** Legal contracts, purely academic papers, and marketing slogans (marketing can borrow Microsoft brand voice, but this handbook prioritizes technical documentation).
- **Default conflict policy** (see also section 13):
  - General product copy → Microsoft
  - Developer/API → Google
  - Apple ecosystem product copy → Apple
  - Docs engineering principles → Write the Docs

---

## 2. Core principles (four-way consensus)

These principles are emphasized across multiple guides (sources noted in parentheses).

| Principle | Shared by | Key points |
|-----------|-----------|------------|
| **Short and clear** | MS, Google, Apple, WtD | Fewer words, more meaning; keep sentences short; cut unnecessary modifiers (MS Top 10; Google tone; Apple present tense / clarity) |
| **Skimmable** | MS, Google, WtD | Lead with what matters; put the point in headings and first sentences; chunk with lists and headings (MS scannable; WtD Skimmable) |
| **Active voice + second person *you*** | MS, Google | Make clear who acts; address the reader as *you*; avoid *we* for what the reader must do (Google Highlights) |
| **Consistent** | Google, WtD, Apple, MS | Terms, capitalization, and formatting stay uniform; project-specific rules override general ones (Google reference hierarchy; WtD Consistent) |
| **Task- and intent-focused** | MS, Google, WtD | Clarify what the reader needs to finish before you write (MS intent; Google focus on the task) |
| **Inclusive and accessible** | MS, Google, Apple, WtD | Bias-free wording; do not rely on color or direction alone; provide alt text (inclusive / accessibility guidance across sources) |
| **Globalization-friendly** | MS, Google, Apple | Short sentences, few idioms, consistent terms—easier to translate and for non-native readers (MS localization; Google global audience) |
| **Accurate and timeless** | WtD, Google | Wrong docs are worse than none; avoid *currently / soon / new* and similar aging words (WtD Current; Google timeless) |
| **Rules can be broken** | Google (citing Orwell) | Break a rule for clarity when needed—but stay consistent after you do |

**Write the Docs additions (docs engineering):** Documentation should be precursory (written early) and participatory (everyone contributes); content should be ARID (Acceptable Repetition In Documentation), exemplary (include examples), and nearby (source files live close to the code).

---

## 3. Voice and person

### 3.1 Target voice

| Prefer | Avoid |
|--------|-------|
| Conversational, friendly, and respectful—like a knowledgeable colleague (Google: conversational, friendly, respectful) | Cute slang, internet memes, exaggerated hype (*Dude! This API is totally awesome!*) |
| Natural spoken feel, but cleaner than real speech (MS: write like you speak; Google: do not write like a chat transcript) | Stiff bureaucratic phrasing (*may enable the acquisition of…*) |
| Direct and helpful | Over-politeness (repeating *please* in every step) |

**Google tone scale examples:**

| Too informal | Just about right | Too formal |
|--------------|------------------|------------|
| Dude! This API is totally awesome! | This API lets you collect data about what your users like. | The API documented by this page may enable the acquisition of information pertaining to user preferences. |

### 3.2 Person

- **Use second person *you*** (Google, MS): address the reader who is doing the work.
- **Avoid *we* for actions the reader must take**; Google explicitly discourages *let's do something*.
- For a singular person of unknown gender: use *they/their*, or rewrite in the plural / with *you* (MS bias-free; Google inclusive).

### 3.3 Contractions

- **Microsoft product copy:** Encourage *it's, you'll, you're, we're, let's*—they sound friendly.
- **Google developer docs:** Natural tone is enough; do not force contractions, but avoid sounding overly formal.
- **Default recommendation:** Use contractions in product help and tutorials; API reference can be slightly more formal—keep the whole document consistent.

**Prefer:** To help you do more, the assistant needs to know what **you're** interested in.  
**Avoid:** …what **you are** interested in… (not wrong, but MS treats it as stiffer)

### 3.4 Tone words to minimize (Google)

Avoid: *simply / it's easy / quickly* (in procedures), overused exclamation points, trendy slang, *please note*, *at this time*.

**Prefer:** To view the document, click **View**.  
**Avoid:** To view the document, please click **View**.

---

## 4. Sentences and paragraphs

### 4.1 Shared rules

1. **Prefer short sentences** (MS, Google, Apple, WtD): Google suggests aiming under about 26 words per sentence; MS notes that compound sentences are harder to translate.
2. **Front-load important information** (MS Top 10, WtD): Put the conclusion or action in the first sentence.
3. **Use active voice** (Google, MS): Make the subject clear.
4. **Lead with verbs** (MS): Prefer verb-led statements and steps; cut extra *you can* and *there is/are*.
5. **Put conditions before instructions** (Google): *If X, do Y*—not *Do Y if X* (readers often miss the condition).

### 4.2 Prefer / avoid

| Prefer | Avoid | Source |
|--------|-------|--------|
| Ready to buy? Contact us. | If you're ready to purchase Office 365 for your organization, contact your Microsoft account representative. | MS |
| Store files online, access them from all your devices, and share them with coworkers. | You can access Office apps across your devices, and you get online file storage and sharing. | MS |
| Save time by creating a document template that includes the styles you use most often. | Templates provide a starting point… Consider creating a template if… (point buried at the end) | MS |
| If the build fails, check the logs. | Check the logs if the build fails. | Google (condition first) |
| The Output Directories area appears. | The Output Directories area displays. (*display* misused as intransitive) | Google word list |

### 4.3 Paragraphs

- One main idea per paragraph; make the first sentence skimmable (WtD, Google).
- Break walls of text with headings and lists (Google accessibility).
- Do not bury long asides inside numbered steps (MS Learn quick start).

---

## 5. Word choice and spelling

### 5.1 General conventions

- **American English** (Google explicitly; MS/Apple practice is also US): *color, behavior, canceled* (Google follows the first Merriam-Webster spelling).
- **Dictionaries:** Google → Merriam-Webster; nontechnical style may follow the Chicago Manual of Style; for technical points, Google’s own hierarchy also points back to the Microsoft Style Guide.
- Spell out uncommon abbreviations on first use (Google, WtD, Apple).

### 5.2 Preferred words (MS and Google largely agree)

| Prefer | Avoid | Notes |
|--------|-------|-------|
| sign in / sign out | log in / log out (as verbs) | MS prefers *sign in*; Google generally uses *sign in*, and matches UI only if the product literally says *log in* |
| sign-in (n./adj.) | login (as a verb); signin | Google word list |
| select (a checkbox) | check (ambiguous) | Google |
| clear (a checkbox) | uncheck / deselect | Google |
| click (desktop) | click on; hit | Google; use *tap* for touch |
| enter / type (text) | vague *specify* as the action verb | Google UI |
| stop / exit / cancel / end | abort / kill / terminate (unless domain jargon) | Google; except Linux signal names |
| allowlist / denylist (nouns) | whitelist / blacklist | Google, MS (also primary/subordinate, etc.) |
| stop responding | hang | MS, Google |
| for example / that is | e.g. / i.e. | Google, Apple |
| and | & (in body text/headings) | Google |
| lets you | allows you to / enables you to | Google |
| because | since / as (for cause) | Google (*since/as* can mean time) |
| to | in order to (in most cases) | Google |
| app (for end users) | application (unless enterprise/complex context) | Google |
| email (noun) | e-mail; do not use as a verb → *send email* | Google |
| on-premises | on prem / on-premise | Google |
| setup (n.) / set up (v.) | mixing the two | Common across guides |
| dialog | dialogue (for UI); popup | Google |
| later / earlier (versions) | higher / lower / above / below (for versions) | Google (Android exception: higher/lower) |

### 5.3 Differences and defaults

| Topic | Microsoft | Google | Default recommendation |
|-------|-----------|--------|------------------------|
| Contractions / *let's* | OK in product copy | Avoid *let's* in developer docs | Product copy → MS; developer docs → Google |
| Self-reference as *documentation* | Learn often says *article*, etc. | Prefer *this document*; avoid *this article/page/doc* | Follow Google for developer docs |
| *data* | — | Treat as singular: *the data is* | Follow Google |
| UI bold | Context-dependent | Bold UI labels | Follow Google for developer docs |
| Apple product names | — | — | For Apple ecosystem content, follow Apple strictly: do not abbreviate product names; keep leading lowercase on names like iPhone |

### 5.4 Objective wording (Google: precise, objective)

Remove subjective “easy/hard” judgments:

**Prefer:** Open the configuration file and add your custom key.  
**Avoid:** Simply open the configuration file to quickly add your custom key.

---

## 6. Capitalization, punctuation, lists

### 6.1 Capitalization

- **Headings and subheadings: sentence-style (sentence case)**—capitalize only the first word and proper nouns (MS Top 10; Google Highlights; also WtD site practice).
- **Do not default to Title Case** (MS: When in doubt, don't capitalize).

**Prefer:** Create a project template  
**Avoid:** Create A Project Template / Limited-Time Offer → **Limited-time offer**

- UI labels: generally match the UI; if the UI is all caps, rewrite in sentence case in body text (Google UI).
- Apple: table and figure titles use sentence-style; figure titles usually omit a final period.

### 6.2 Punctuation

| Rule | Prefer | Avoid | Source |
|------|--------|-------|--------|
| Oxford / serial comma | Android, iOS, and Windows | Android, iOS and Windows | MS, Google |
| Spaces after a period | One space | Two spaces | MS |
| Em dash | pipelines—logical groups—… (no spaces) | pipelines — logical groups — … | MS |
| End punctuation in titles | Usually no period or colon on headings/subheadings | Move a tile. | MS |
| Lists of three or more | Commas + and/or | Relying on *and/or* with slashes (Google is cautious about and/or) | Google |

### 6.3 Lists

- **Ordered steps → numbered lists**; **unordered points → bullets** (Google).
- Paired data can use description lists (Google).
- Keep list items parallel (MS, Google, WtD).
- Full sentences: capitalize and end with a period; phrases: stay consistent within the list (align with Google list rules).

---

## 7. Titles and structure

### 7.1 Skimmable structure (WtD Skimmable + MS/Google)

- Write like a newspaper, not a novel: headings name a concrete task or concept.
- Do not skip heading levels (`h1` → `h2` → `h3`) (Google accessibility).
- Make link text meaningful: **do not** use *click here* / *read this* (Google, WtD).
- Put recognizable concepts early in paragraphs and list items (WtD).

**Prefer headings:** Create an API key / Authenticate with OAuth 2.0  
**Avoid headings:** Overview / Miscellaneous / More info

### 7.2 Front-loading

Put decision-critical information first: what you can do, prerequisites, and next steps.

**Prefer:** Save time by creating a document template that includes the styles, formats, and page layouts that you use most often.  
**Avoid:** Defining “template” abstractly first, and only at the end suggesting that creating one might help.

### 7.3 Document types (WtD / practice)

- Separate tutorials and examples from strict reference so both stay skimmable (WtD Exemplary).
- Keep reference pages complete and addressable (stable headings/anchors per concept).
- Treat outdated content as a defect: fix wrong docs first (WtD Current).

---

## 8. Procedures and UI instructions

### 8.1 Writing steps (Microsoft primary, Google supplemental)

1. Use a **numbered list** for multi-step procedures; a single step can use a bullet for layout consistency (MS).
2. One action per step; short actions in the same UI place can be combined (MS).
3. Write steps as complete sentences: capitalize and end with a period; most steps start with an **imperative verb** (MS).
4. **Locate, then act** (MS, Google): *On the Design tab, select Header Row.*
5. Use a short intro when needed to set context; do not merely repeat the heading (MS).
6. Split long procedures into sections; avoid overly long single procedures (MS: consider splitting around 12+ steps).
7. Put conditions and results before the action (Google).
8. Prefer task goals over brittle control names so UI renames hurt less (Google: focus on the task).

**Example (MS):**

To create a group of tiles:

1. On the Start screen, select the tiles that you want to group together.
2. Drag the tiles to an open space. When a gray bar appears behind them, release them to create the new group.

### 8.2 UI wording (Google primary)

| Scenario | Prefer | Avoid |
|----------|--------|-------|
| Button | Click **OK**. | Click the "OK" button. / Click on OK. |
| Menu path | Select **File > Open**. or In the **File** menu, select **Open**. | Vague *go there and hit Open* |
| Checkbox | Select the **Automatically check for updates** checkbox. / Clear the **Bookmarks** checkbox. | Check / Uncheck … |
| Text input | In the **Owner** box (or Google Cloud: **field**), enter your name. | Name the account. (treating UI as an English verb) |
| Icon button | Use the tooltip/accessible name: Click **Notifications**. | Click the bell icon. / hamburger menu |
| Keyboard | Press Control+C (or Command+C on macOS). | Press Ctrl+C (⌘+C). (spell out modifier key names) |
| Touch | tap; Android: touch & hold | click (in touch-only contexts) |

**Input-device neutrality:** Use *click* on desktop and *tap* on touch; for cross-device content, name the task: “Refresh the page.”

### 8.3 Angle-bracket paths and accessibility

When you write `Menu > Command`, screen readers may say “greater than.” Google recommends an accessible label such as *and then* for `>`. Microsoft also advises confirming with accessibility experts before heavy use of `>`.

---

## 9. Code and API docs

Prefer the **Google** developer style guide, with **Microsoft Learn** technical-writing habits as a secondary reference.

### 9.1 Code and typography

- Use monospace (code font) for code, commands, filenames, and API identifiers (Google).
- Bold UI labels; do not use code font for UI unless the label is literally code (Google).
- Sentence punctuation that belongs to the sentence uses body font; punctuation that belongs to the code stays in the code (Apple has similar guidance).

### 9.2 Placeholders (Google placeholders)

- Form: `UPPER_SNAKE_CASE`, such as `PROJECT_ID`, `INSTANCE_NAME`.
- Do not use `xxx`, `foo`/`bar` (unless domain-unavoidable); do not use `MY_` / `YOUR_` prefixes.
- Explain after first use:
  - One placeholder: *Replace `BUILD_ID` with …*
  - Several: *Replace the following:* then a parallel list.

**Prefer:**

```text
gcloud compute instances create INSTANCE_NAME \
    --metadata enable-guest-attributes=TRUE
```

Replace `INSTANCE_NAME` with the name that you want your new VM instance to have.

### 9.3 Command line (Google)

- Copy-ready samples should contain runnable content and placeholders only; avoid unexplained `[]` `{}` `|` `...` inside one-click copy blocks (they get pasted literally and fail).
- Document optional and mutually exclusive parameters in separate examples or sections.
- Break long commands with a line-continuation character (Linux `\` / Windows `^`) and indent continuation lines.
- When showing output, use a fixed lead-in: *The output is similar to the following:* / *The output is the following:*
- Do not verbify `ssh` / `RDP`: *Connect by using SSH*, not *ssh into the instance*.

### 9.4 API / reference page structure (practical consensus)

Common sections (not every page needs all of them, but keep like pages alike):

1. Overview (what it does, when to use it)
2. Prerequisites
3. Request/endpoint or command syntax
4. Parameter table (name, type, required?, description)
5. Example request and response
6. Errors and status codes
7. Related links

MS Learn: put detail in code comments inside steps so the surrounding prose stays uncluttered.

### 9.5 Apple technical typography notes (when writing for Apple platforms)

- File extensions lowercase with a leading dot: `.jpg`; type names uppercase: JPEG, MP3.
- Prefer present tense; do not switch to future tense in steps without reason.
- Do not abbreviate Apple product or service names.

---

## 10. Accessibility and bias-free writing

### 10.1 Bias-free language (MS + Google + Apple)

| Prefer | Avoid |
|--------|-------|
| chair, moderator; workforce, staff; person-hours | chairman; manpower; man-hours |
| they / you / plural rewrite | generic he/she, he/she, s/he |
| primary / replica (or precise terms like parent / worker) | master / slave |
| perimeter network | demilitarized zone (DMZ) (MS) |
| allowlist / blocklist and other precise terms | whitelist / blacklist |
| person who is blind; users with limited dexterity | defining people by disability; pitying phrasing (*suffering from*) |
| Diverse fictional names and roles | Single-culture or gendered stereotypes |

**MS:** When writing about real people, use the pronouns they prefer; keep fictional examples diverse.  
**Google:** When replacing legacy industry terms, you may note the old name in parentheses on first use, then switch; if an old keyword must appear in code, keep it only in code font and explain it.

### 10.2 Accessible writing (Google accessibility and others)

- Provide meaningful **alt** text for images; empty alt for decorative images; do not put copy-paste code or terminal output only in images.
- Make links understandable out of context; call out unusual behavior (downloads, new tabs).
- **Do not convey meaning by color, position, or shape alone.**
- **Avoid directional language** for UI or doc location: prefer *preceding / following*, or name the control; add a screenshot when needed.

**Prefer:** Click **Menu**. / In the preceding diagram, …  
**Avoid:** In the left-side panel, click the button with three lines. / In the diagram above, …

- Use correct heading hierarchy; give tables headers and avoid merged cells; introduce tables in prose first.
- Provide captions/transcripts for video; avoid flashing content.

---

## 11. Globalization and localization notes

Combined from MS Learn localization, Google global audience, and Apple international style:

1. **Short sentences and simple structure**; minimize parentheticals and long clause chains (MS).
2. **Keep “little words”:** *a, the, that, is* matter for machine translation (MS).
3. **Keep terminology and capitalization consistent** across the doc (MS, Google).
4. **Avoid idioms, puns, pop culture, and sports metaphors** (Google).
5. **Dates and numbers:** use unambiguous date formats (Google); watch decimal and thousands separators by locale (Apple international).
6. **Example places and people:** avoid politically contested regions; keep geographic hierarchy consistent (do not mix countries and states in the same listing logic) (MS).
7. **Screenshots and UI:** leave room for localization growth; do not burn long English-only strings into images (practical consensus).
8. **Tense and timeliness:** minimize *currently, soon, new, as of this writing* (Google timeless) so translated copies age more slowly.

---

## 12. Quick reference: prefer vs avoid

| Prefer (Do) | Avoid (Don't) |
|-------------|----------------|
| Create a project. | Create a new project. (unless contrasting with another just-created one) |
| Sign in to your account. | Log in to your account. / Sign into your account. |
| Click **Save**. | Click on the **Save** button, please! |
| Select the **I agree** checkbox. | Check the **I agree** checkbox. |
| Enter your project ID. | Specify your desired project ID. |
| If the token expires, refresh it. | Refresh it if the token expires. |
| The API lets you export logs. | The API allows you to / enables you to export logs. |
| Use version 2.2 or later. | Use version 2.2 or higher / 2.2+. |
| For example, set `REGION` to `us-east1`. | Set `REGION` to `us-east1`, e.g. |
| Add the IP address to the allowlist (sometimes called a whitelist). | Blacklist the IP. |
| Press Control+S (Command+S on macOS). | Hit Ctrl+S. |
| See [Configure OAuth](…). | Click here for more information. |
| Replace `PROJECT_ID` with your project ID. | Replace `xxx` / `foo` with … |
| This document describes how to… | This article/page/doc describes… (developer-doc context; follow Google) |
| The service stops responding. | The service hangs. |
| Older adults; people with disabilities | the elderly; the disabled (context-dependent; respect community preferences) |

---

## 13. Where the four guides differ

| Topic | Microsoft | Google | Apple | Write the Docs | **How to choose on conflict** |
|-------|-----------|--------|-------|----------------|------------------------------|
| Primary audience | Broad product users + technical content | Software developers and technical practitioners | Apple product/UI/training readers | Docs community and engineering teams | Choose by document type |
| Voice | Warm, relaxed, more contractions | Friendly but not flippant; less *let's* / *please* | Clear, consistent, strict product terminology | Neutral-friendly; light on tool evangelism | **Product copy → MS**; **developer → Google**; **Apple products → Apple** |
| Heading capitalization | Sentence case | Sentence case | Mostly sentence-style (figure/table titles, etc.); product names per brand | Sentence case (their site) | Unify on sentence case |
| Oxford comma | Yes | Yes | See A–Z (generally careful) | Per your house style guide | **Use the Oxford comma** |
| UI action verbs | select / go to, etc. | Detailed word list: click/tap/select/clear… | Follow Apple UI wording and product names | — | Developer docs → Google word list |
| Word-list focus | Bias-free, global communication | Long word list + inclusive language | Product terminology A–Z | Emphasizes building your own guide and staying consistent | API/cloud docs → Google |
| Code/CLI | Learn practice-oriented | Very detailed placeholders, optional params, copy-ready samples | Technical notation and placeholder chapters | Docs as Code; sources near code | **API/CLI → Google**; process → WtD |
| Accessibility | Guidance and terminology | Dedicated chapter (directional language, alt, tables…) | Writing inclusively | Resource roundups | **Developer docs → Google**; everyone follows bias-free rules |
| Flexibility | Brand-voice framework | Explicit “Break the rules” | Consistency with Apple materials first | Principle-led; encourages house guides | Clarity first, then whole-doc consistency |

**One-line default policy:**

- Writing **Windows / Microsoft 365 / general SaaS product help** → start with Microsoft.
- Writing **APIs, SDKs, cloud consoles, open-source developer guides** → start with Google (Google also notes that Microsoft Style Guide can help on technical points).
- Writing **iPhone / macOS / App Store and other Apple user copy** → start with Apple.
- Designing **doc systems, IA, process, Docs as Code** → start with Write the Docs principles, then apply the language rules from the three vendor guides above.

---

## 14. Reference links

### Microsoft

- https://learn.microsoft.com/en-us/style-guide/welcome/
- https://learn.microsoft.com/en-us/style-guide/top-10-tips-style-voice
- https://learn.microsoft.com/en-us/contribute/content/style-quick-start
- https://learn.microsoft.com/en-us/style-guide/bias-free-communication
- https://learn.microsoft.com/en-us/style-guide/procedures-instructions/writing-step-by-step-instructions

### Google

- https://developers.google.com/style
- https://developers.google.com/style/highlights
- https://developers.google.com/style/tone
- https://developers.google.com/style/word-list
- https://developers.google.com/style/accessibility
- https://developers.google.com/style/inclusive-documentation
- https://developers.google.com/style/ui-elements
- https://developers.google.com/style/code-syntax
- https://developers.google.com/style/placeholders

### Apple

- https://support.apple.com/guide/applestyleguide/welcome/web
- https://help.apple.com/pdf/applestyleguide/en_US/apple-style-guide.pdf

### Write the Docs

- https://www.writethedocs.org/guide/
- https://www.writethedocs.org/guide/writing/docs-principles/
- https://www.writethedocs.org/guide/writing/style-guides/
- https://www.writethedocs.org/style-guide/

---

*Compilation note: Entries map to publicly documented rules and examples from the sources above. This synthesis is for personal or internal team use to unify English technical documentation style.*
