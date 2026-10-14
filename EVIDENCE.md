# Evidence and acceptance limits

Evidence snapshot: 14 October 2026. These are scoped first-party records; private logs are summarized rather than offered as public reproductions.

| Claim | Source | Scope |
| --- | --- | --- |
| PCC reading, explicit WAITING save and page-reload persistence | [Seven continuous captures](DEMO.md), captured from 0.16.1 main on 14 Oct 2026 | Actual browser QA with synthetic records; save implementation unchanged; evidence pre-seeded |
| PCC Mac 0.16.1 formally installed; source/signature/bundle parity checked | Formal installed provenance and static validation records dated 14 Oct 2026; main `6488f743362dce6eae1893fd6170165db08b6486` | Local installation acceptance; not trusted public distribution, voice accuracy or Windows acceptance |
| MCP production identity and list/search/get success | Owner’s production session, 14 Oct 2026 13:36 JST, v1.0.0 / `9df7ccc1eebbc8bd64f2474d48cea0d87e262650` | Bounded production sample; logs remain private |
| One unread message stayed unread across list/get/list | Owner’s production session, 14 Oct 2026 14:04 JST | One naturally unread sample; not all messages or clients |
| FH source/package 16-case replay and F10 P95 | Machine summary dated 6 Oct 2026, pinned at record revision `80527c5c76c0062e7118c8f0a40c054d3d1b319f` | Physical screenshot fixtures, two 4K displays, DPI 144; 222.9952 / 260.1708 ms rounded to 223.0 / 260.2; final official FULL16/P95 not qualified |
| Cache example transitions and tests | [Sample source](https://github.com/yiyisann/evidence-cache-demo); locally run 14 Oct 2026 with Node 24.17.0 | Independent synthetic, in-memory example; 12 tests passed; not product or security evidence |

Japanese subject misses were observed in the owner’s MCP production session. HTML-only mail may not yield plain text. No production mail was accessed for this portfolio continuation.

The MCP and FH summaries have provenance but do not expose full public reproduction inputs. The visuals for those two projects are explanatory schematics. No adoption, usage, live gameplay or selection outcome is claimed.

## Development attribution

I use Claude Code and Codex as development collaborators and retain responsibility for requirements, product decisions, review and acceptance. For PCC and MCP, my account of Claude Code involvement spans early prototypes, UI and feature development, debugging and review. Private Git attribution records provide specific examples; they do not measure a share of code ownership or identify the tool used for every change.

| Project | Source of attribution | Recorded examples and scope |
| --- | --- | --- |
| PCC | My account of the development process, supported by private commits with Claude co-author attribution | Readability and contrast work in August 2026; native-shell design and launcher fixes in September. These are historical contributions, separate from the 0.16.1 walkthrough acceptance. |
| Personal AI Control Plane | My account of the development process, supported by private commits with Claude co-author attribution | Bounded content handling and regression tests on 11 September 2026; retrieval-only boundaries and runtime metadata handling on 19 September. These establish recorded contributions, not authorship of every later production change. |
| FH Overlay | My broader account of using both tools, supported by private commits with Claude co-author attribution | Overlay interaction, controls and window-order fixes on 29 August 2026. This does not assign the full recognition pipeline or the later fixture benchmark to one tool. |
| Independent evidence-cache demo | Its separate portfolio-preparation record on 14 October 2026 | Prepared with Codex assistance as a new teaching example. Its recorded origin is distinct from the collaboration on the three products. |

The underlying products and attribution records remain private. These summaries publish the scope of collaboration without exposing private code, logs or conversation records.
