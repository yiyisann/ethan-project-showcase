# Ethan · Tools for a clear next step

My background is hospitality partnerships and TravelTech operations in Japan. I turn everyday friction into tools I can use and inspect, own product direction and acceptance, and work with Claude Code and Codex on implementation and review.

**Start with Personal Command Center:** keep a source, its uncertainty and an explicit next step together. **Updated 27 October 2026:** PCC 0.17.0 has completed formal installed-app acceptance on Mac and Windows, preserving existing data and settings.

[Portfolio](https://ethan-wei-portfolio.ethanwei77.chatgpt.site) · [LinkedIn](https://www.linkedin.com/in/ethan-w-43a111238/)

[Historical 0.16.1 browser walkthrough](DEMO.md) · [Evidence and limits](EVIDENCE.md) · [Runnable cache example](https://github.com/yiyisann/evidence-cache-demo)

The viewable walkthrough below is the **historical 0.16.1 browser flow**: read a synthetic monitor comparison, explicitly save a waiting action, and return after a page reload. A new 0.17.0 native recording is not provided; [EVIDENCE](EVIDENCE.md) separates current acceptance from this historical capture and its limits.

![PCC reading a synthetic monitor comparison](assets/pcc-02-read.png)

*Actual PCC 0.16.1 frontend, isolated browser QA, synthetic data. Article evidence and waiting conditions were pre-seeded; saving here uses browser localStorage. Native SQLite writes and AI-provider calls are outside this demonstration.*

## Personal Command Center · flagship

**Problem:** Information, reading and decisions are easy to separate into different tools, losing the source and the next action.

**My contribution:** I shaped the reading-and-decision workflow, cache continuity and explicit save boundary. I worked with Claude Code and Codex across prototyping, UI and feature development, debugging and review, and own the acceptance decisions. Private development history includes Claude-attributed readability and native-shell changes.

**Implementation:** React/TypeScript, Tauri/Rust and SQLite in the desktop product. The current 0.17.0 release adds a Decisions Workbench with structured context and question-level images. The viewable walkthrough uses the existing browser QA gateway from the historical 0.16.1 main revision.

**Result:** The 0.17.0 release record confirms Mac and Windows formal installed-app acceptance at the same product revision, including preservation of existing data and settings. Separate synthetic native acceptance records cover explicit save and restart persistence. The historical browser walkthrough shows reading → saved decision context → an explicit waiting action → return to the same article → persistence after reload. Reading alone creates no saved event.

**Key limit:** Decisions paid Live API behavior remains unverified. [Evidence and acceptance limits](EVIDENCE.md) detail capture, platform and distribution coverage.

## Personal AI Control Plane · supporting project

**Problem:** AI context can become ambiguous about permission, which source is current, and whether a read changes the underlying account.

**My contribution:** I defined account and authority boundaries and worked with Claude Code and Codex on prototypes, implementation, debugging and review. Recorded Claude contributions include retrieval-only boundaries and bounded content handling. I kept deployed code identity separate from source identity.

**Implementation:** TypeScript, a stateless MCP service on Cloudflare Workers, owner OAuth, SHA-pinned source reads and a bounded read-only IMAP adapter.

**Result:** The dated production record for **1.1.0, 21 October 2026 (Japan time)** confirms scoped PCC source access, bounded mail reads and continuation to older results. A source outside the approved repository set was rejected. The deployment is tied to its implementation revision; the later documentation HEAD is a separate identity.

**Key limit:** HTML-to-text fallback has local validation but no live HTML-only sample. One bounded Japanese-subject query succeeded; general Unicode matching remains unproven. The 1.1 run had no naturally unread sample, so the earlier one-message unread check remains historical. Natural 24-hour OAuth refresh and fresh ChatGPT/Windows/Linux client acceptance were not revalidated. Private production evidence is not publicly reproducible.

![Original schematic of scoped MCP access](assets/mcp-boundaries.svg)

*Architecture schematic, not a client capture or a security proof. No mail content is included.*

## FH Overlay · supporting project

**Problem:** Captured race context and recommendations need to stay readable in one focused Windows surface.

**My contribution:** I shaped the focused overlay, recovery behavior and acceptance of the full F10-to-result path, working with Claude Code and Codex on implementation and debugging. Recorded Claude contributions include overlay interaction and window-order fixes.

**Implementation:** Python/Tk, local visual recognition and a recommendation policy.

**Result:** Source and packaged builds completed the recorded physical screenshot-fixture replay, exercising the F10-to-result path.

**Key limit:** This is fixture replay, not natural live gameplay or a final installed-runtime benchmark. Raw per-case inputs and outputs are not published.

![Original recognition pipeline schematic](assets/game-recognition-pipeline.svg)

*Pipeline schematic, not a game capture or recognition result.*

## A small example you can run

[Evidence-cache demo](https://github.com/yiyisann/evidence-cache-demo) illustrates one rule: a failed refresh preserves the last useful fact and its observation time, while visibly marking it stale. Node.js 22+, no dependencies or network; run `node demo.mjs` and `node --test cache.test.mjs`.

It is an independent teaching example, not extracted product code. It does not prove PCC behavior, MCP authorization safety or recognition performance.

## Hospitality experience and the proposed competition direction

My hotel-partnerships experience makes visit preparation a useful next problem: assemble public hotel facts into a short brief with source links, flag conflicts and gaps, and turn them into questions to confirm during the visit. This is the direction I **plan to explore during Built with Claude Japan 2026**, not a completed product. PCC and the supporting projects are prior work, not work claimed to have been built during the competition. The proposed brief would use public sources only; no employer or customer confidential materials are included here. No selection outcome, adoption or time saving is claimed.

**Development and responsibility:** Claude Code and Codex contributed at different stages of these products. I defined the requirements, reviewed the results and decided what was ready to use. [Development attribution and acceptance limits](EVIDENCE.md) distinguish my account of that collaboration from recorded examples. Full product repositories and operational records remain private. See [visual sources and reuse scope](ASSETS.md).
