**REFERENCE GUIDE · HONEYBEE SXS**

# Gemini vs. Gemini Spark

A new pairing in the SxS queue: standard Gemini against **Gemini Spark**, Google's agent mode. Same queue, same taxonomy, same grading — with **one thing changed that matters**. Spark issues no share links, so its trajectory is captured by saving the page instead.

---

## Contents

1. [What changes, and what does not](#1-what-changes-and-what-does-not)
2. [What Gemini Spark is](#2-what-gemini-spark-is)
3. [Setup: one account, and how to reach Spark](#3-setup-one-account-and-how-to-reach-spark)
4. [Running the Spark side](#4-running-the-spark-side)
5. [Capturing the Spark trajectory](#5-capturing-the-spark-trajectory)
6. [Before you submit](#6-before-you-submit)

> **READ THIS ALONGSIDE THE MAIN GUIDELINES**
>
> This page covers **only** what is different on a Gemini-versus-Spark task. Everything else — steering, turn capture, rubric grading, the eight dimensions, the preference — works exactly as described in **Honeybee SxS — Contributor Guidelines**, which remains the source of truth.

---

## 1. What changes, and what does not

| On a Spark task | Standard Gemini side | Gemini Spark side |
|---|---|---|
| **Account** | **One demo account, used for both sides.** The task lists a single set of credentials — sign in once and stay signed in. | *(same account — see left)* |
| **Where you run it** | `gemini.google.com`, as normal | Same site, **same account** → sidebar → **Switch to Spark** |
| **Model version** | Named in the task requirements | Named in the task requirements |
| **Per-turn share links** | Yes — every turn | **None. Spark has no Share feature.** |
| **Final trajectory link** | Yes — `share.gemini.google/…` | **None.** You upload a saved page instead |
| **Browser** | Any | **Chrome** — required for the capture to be usable |
| **Everything else** | Unchanged. Turn entries, attachments, key turn, rubric grades, the eight dimension ratings, the preference and the submission checklist are all exactly as in the main guidelines. | *(same — see left)* |

> **WEB ONLY, AND CHROME SPECIFICALLY**
>
> **These tasks are run on the web.** There is no mobile surface in scope, and the Gemini app on Mac is not what the task is asking you to evaluate.
>
> **Use Google Chrome.** The Spark capture depends on Chrome's ***Webpage, Single File*** save format, which is what gets parsed downstream into a readable trajectory. A file saved from another browser may not parse, and there is no way to recover it after the fact.

---

## 2. What Gemini Spark is

**Gemini Spark is Google's personal AI agent, built into the Gemini app.** Where a standard Gemini chat answers what you ask in the moment, Spark is designed to **take on a whole workflow**: it plans a sequence of steps, uses connected apps and tools to carry them out, and can keep working on a task over time rather than turn by turn.

To do that it draws on more than the conversation. Spark can use **Connected Apps** (Gmail, Drive, Calendar, Docs, Sheets, Slides, Keep, Tasks, Contacts, Photos, YouTube and Search services), **skills** — reusable instruction sets it applies to a kind of job, **schedules** that trigger a task automatically, your past chats, and a browser it can drive itself. Google's own examples are things like decluttering an inbox, producing a running news digest, or researching a topic with cited sources.

> **THE THREE BUILDING BLOCKS, IN GOOGLE'S TERMS**
>
> - **A task is the goal** — the whole objective you hand over. ***"Plan and manage my trip to London."***
> - **A schedule is the when** — an automatic trigger, by time or by event. ***"Every day at 8am, update me on AI news."***
> - **A skill is the how** — reusable instructions plus context that teach Spark to do a particular kind of job.

Two consequences matter for evaluation. First, **Spark shows its work**: a task thread carries a visible trace of the steps it planned, the tools it called and the files it touched. Second, **Spark acts** — it will ask you to confirm before sending mail, changing data or submitting a form, and it may pause and ask you to take over its browser. Both of those are part of what you are grading, and both need to survive into your capture.

> **DO NOT PUT ANYTHING SENSITIVE INTO A SPARK THREAD**
>
> Google's guidance is explicit: never type sign-in details, payment details or anything you consider sensitive into a task thread. That applies here too — you are working in a synthetic demo account, and **nothing personal of yours should ever enter one of these runs.** If Spark asks for a credential, it is asking the persona, not you; steer around it rather than inventing one.

---

## 3. Setup: one account, and how to reach Spark

> **ONE DEMO ACCOUNT COVERS BOTH SIDES OF THIS TASK**
>
> **The task lists a single set of demo credentials, and you use it for both models.** If you have worked a Gemini-versus-Gemini batch where each side had its own login, **this batch is not that** — there is no second account to find and nothing to sign out of between the two runs.
>
> That works because the two sides are not two accounts, they are **two modes of the same app.** Standard Gemini is the normal chat; Spark is reached from the sidebar of that same signed-in session.

### Step 1 — Sign in once, with the demo account

Sign in to `gemini.google.com` with the demo credentials on your task and **take the account screenshot as usual.** One screenshot covers the task, because one account runs both sides.

As always, **the demo credentials are for Gemini only** — they are not a login for any other product, and you never substitute a Google account of your own.

### Step 2 — Switch between the two modes

Run the standard Gemini side in a normal chat. For the Spark side, **on the sidebar, click "Switch to Spark"** — same browser, same session, no signing out. That is the whole of it: Spark is a mode inside the Gemini app, not a separate product to install or a separate site to visit.

**Check which mode you are in before you send Turn 1 of each run.** With one account behind both sides, the mode is the only thing separating them, and nothing in the tooling will notice if you run the same one twice.

Spark requires a Google AI Pro or Ultra subscription and a personal Google account. **The demo account is already set up for both**, so if Spark is not available to you, that is a task problem to raise in the War Room — not something to fix by signing in with an account of your own.

> **[ASPIRATIONAL] REHYDRATE BETWEEN THE TWO RUNS — IT IS THE ONLY THING SEPARATING THEM**
>
> The standing rule already requires a reset before ***every*** run, including between the two models on a base task. **It matters more here.** On a batch with two accounts, each side started in its own untouched environment; on this one, both sides share an account, so whatever the first model sent, created or changed is still sitting there when the second one starts. **Reset at `synthetic-account-hydration.outlier.ai/reset` before the second run**, or the comparison is invalid no matter how carefully you grade it. On a **Traffic** task there is no universe and nothing to reset.

### Step 3 — Confirm the model and screenshot it

The exact Gemini version for each side is **set per task and shown in your task requirements.** It is managed by variables, so it can change between batches without this document changing — **read it off the task, never off this page.** Screenshot the selector before Turn 1 as you would anywhere else.

---

## 4. Running the Spark side

Steer it as you would any other run: paste the opening prompt verbatim as Turn 1, build toward the target deliverables over 20+ turns, and reveal withheld information the way a real user would. The turn entries, per-turn attachments and the single key turn are all unchanged.

Three things are specific to Spark:

- **Let it finish its plan.** Spark works in steps and can take noticeably longer than a chat reply. Sending the next turn while it is mid-task truncates work you would otherwise be grading.
- **Handle take-over requests in character.** Spark may pause and ask you to take control of its browser to complete an action. Doing so is legitimate and part of the product — note the turn, because the overhead belongs in **Interaction efficiency** and **Recovery Overhead**.
- **Watch what it actually did, not what it says it did.** Spark reports its own steps confidently. Open the account and verify the draft, the event or the file really landed, exactly as you would on any other model — this is **Action Honesty** under Trust & grounding.

### Example: Spark's tool trace, expanded

*(Screenshot in the original PDF, transcribed below. Lines marked ✉ / ⧉ are tool calls — Gmail and Google Workspace Search; lines marked ◷ and the lines under them are Spark's planning steps.)*

```text
Retrieving and summarizing recent email threads  ⌄

  ◷  I've determined this is a straightforward summarization, focusing on recent email activity.
  ✉  Gmail
  ◷  I've initiated a search for the most recent emails in the inbox to understand the overall context.
     I've just reviewed the email threads for relevant URLs to understand their context better.
  ✉  Gmail
  ◷  I've confirmed a required field's absence and re-examined a key verification rule.
  ⧉  Google Workspace Search
  ◷  I've obtained the original URLs from the email threads for further inspection.
     I realized the relevant URLs reside in a different tool's output, and clarified the correct procedure.
     I now understand why the summarization failed and will adjust the retrieval strategy.
     I've confirmed what the user likely wants and am now analyzing email threads from the inbox.
  ✉  Gmail
  ✉  Gmail
  ◷  I've identified the primary categories and threads within the email data, focusing on August 2026 notifications.
     I've examined the email data for specific events, including security alerts and project updates from June and July 2026.
     I found the correct URL for the Fable House retrospective and confirmed its usage per communication guidelines.
     I've just located a specific relevant URL within the retrieved contextual information.
     I've located a specific data point, its associated key, and its exact address.
     I've analyzed more emails and am creating a structured summary with linked factual claims, per the guidelines.
     Show less
```

**Spark's tool trace, expanded.** Each entry is a step it planned or a tool it called. **This trace is part of the evidence** — it is where you can see whether a claimed action was really a Gmail call or just a sentence. It is collapsed by default, and it must be expanded before you save the page.

---

## 5. Capturing the Spark trajectory

> **THERE IS NO LINK TO COLLECT — DO NOT GO LOOKING FOR ONE**
>
> **Spark produces no per-turn links and no conversation share link**, and printing to PDF comes out unreadable. This is a known limitation of the product, not a missing setting.
>
> **Never paste a browser address-bar URL into a link field, and never paste a link from the standard Gemini side of the task.** A session URL is private to you and a link from the wrong side files one model's evidence against the other.

Instead, you save the conversation itself and upload it. **Do this in Chrome, at the end of the run, with the whole conversation loaded on screen.**

### Capture 1 — Expand everything first

Scroll the conversation from top to bottom so every turn has loaded, and **expand the collapsed tool traces** — the ***"N tool steps"*** toggles. What is collapsed on screen is what you risk losing from the saved file, and the trace is the part that shows which tools Spark actually called.

### Capture 2 — Right-click the page and choose "Save As…"

*(Screenshot in the original PDF: a Spark thread titled "Email Correspondence Summary", marked **BETA** and **Complete**, with Chrome's right-click menu open over the conversation. The menu reads: Back · Forward · Reload · **Save As…** (highlighted) · Print… · Cast… · Search this tab with Google Lens · Open in Reading Mode · Create QR Code for this Page · Translate to English · View Page Source · Inspect.)*

**Right-click anywhere on the conversation.** Use ***Save As…*** — **not *Print…***, which produces the unusable PDF.

### Capture 3 — Save it as a single file, named for the task

In the save dialog, set **Format** to **Webpage, Single File**, and name the file:

```text
[CB ID]_[TASK ID]_SPARK
```

*(Screenshot in the original PDF: the save dialog filled in as follows.)*

| Field | Value |
|---|---|
| Save As | `[CB ID]_[TASK ID]_SPARK` |
| Tags | *(empty)* |
| Where | Downloads |
| Format | **Webpage, Single File** |

**Both fields matter.** ***Webpage, Single File*** bundles the whole conversation into one file. Any other format saves a stub plus a folder of assets, which does not survive the upload.

**Substitute your real CB ID and the real task ID** — do not upload a file still called `[CB ID]_[TASK ID]_SPARK`. The name is how your capture is matched back to the task.

### Capture 4 — Upload it to the task

Attach the saved file to the Spark side of the task. **This file is the Spark trajectory** — it is the only record of the run, and it takes the place of the share link and the chat PDF that the other side supplies.

> **WHY WE CAPTURE THIS WAY**
>
> Spark has no export feature yet. Rather than block the work on one being built, the saved page is parsed on our side into the same kind of readable trajectory the other models produce — **including the tool trace**, which is why expanding it matters. The capture method may change once the product supports sharing; until then, this is the method, and a run without it cannot be reviewed at all.

---

## 6. Before you submit

> **SPARK-SPECIFIC CHECKS**
>
> - [ ] Both sides run on **the one demo account** listed on the task, with an account screenshot.
> - [ ] The two runs made in **different modes** — one standard Gemini chat, one Spark — and not the same mode twice.
> - [ ] Spark reached via **sidebar → Switch to Spark**.
> - [ ] **[Aspirational]** Environment reset between the two runs.
> - [ ] The run captured in **Chrome**.
> - [ ] Whole conversation scrolled and loaded, and **every tool trace expanded**, before saving.
> - [ ] Saved as **Webpage, Single File**.
> - [ ] Named `[CB ID]_[TASK ID]_SPARK` with the real IDs filled in.
> - [ ] File uploaded to the Spark side of the task.
> - [ ] **No browser URL pasted into a link field** to fill a gap, and no link borrowed from the Gemini side.
> - [ ] Every written reference to a model says **"Model A"** or **"Model B"** — not "Spark" and not a version number.

Then run the rest of the main checklist as normal: turn entries complete and in order, one key turn, rubric graded and annotated, eight dimensions rated with 200+ character justifications, safety answered, preference recorded, and **no chat deleted.**

> **DELETING THE SPARK CHAT IS STILL A TASK KILLER**
>
> It is worth saying plainly here, because the usual reasoning does not obviously apply: there is no share link to break. **Delete the thread anyway and the run becomes unverifiable** — your saved file can no longer be checked against anything. The rule is unchanged. Do not delete any chat, on either side, before or after submitting.
