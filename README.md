# DSA Notebook

Interactive, step-by-step algorithm visualizations for classic data structures and algorithms (DSA) problems — the kind that show up in coding interviews and LeetCode practice. Every visualizer lets you scrub through an algorithm one operation at a time — watching state, pointers, tables, queues, and edges change at each step — so the internal logic stops being abstract.

**Live site:** [mahav.io](https://mahav.io)

> **This is a living document.** New visualizers get added as I work through problems, and existing ones get refined as I find better ways to explain them. The list below will grow over time.

## What's inside

Each visualizer is a self-contained static page with play/pause/prev/next controls and keyboard navigation.

### Graph algorithms
- **Dijkstra's Shortest Path** — greedy extract-min with a live min-heap and distance table ([`/graphs`](https://mahav.io/graphs))
- **Topological Sort** — Kahn's BFS on a course-prerequisite DAG with live in-degree counters ([`/topo-sort`](https://mahav.io/topo-sort), solves LeetCode #207 Course Schedule)

### Dynamic programming ([`/dp`](https://mahav.io/dp))
Five classic DP problems sharing one interactive table renderer:
- **Fibonacci** (LC #509) — canonical 1-D DP
- **Climbing Stairs** (LC #70) — same recurrence, different framing
- **House Robber** (LC #198) — 1-D DP with an adjacency constraint
- **Longest Common Subsequence** (LC #1143) — 2-D DP indexed by prefix lengths
- **Edit Distance** (LC #72) — Levenshtein distance via insert/delete/replace

### Strings
- **Longest Palindromic Substring** (LC #5) — expand-around-center with live pointer and window tracking ([`/strings`](https://mahav.io/strings))

### Technical interview prep
- **LeetCode Tracker** — curated problem checklist with per-problem notes for technical interview prep, persisted in `localStorage` ([`/leetcode`](https://mahav.io/leetcode))

## Unique characteristics

- **Step-level granularity** — every cell update, queue pop, edge relaxation, pointer move is its own step. No skipped operations.
- **Side-by-side state** — the visual (graph, table, string) is always shown next to the data structures driving it (priority queue, in-degree list, DP table, order array).
- **Hand-authored walkthroughs** — each step is curated for clarity rather than mechanically generated, with a plain-English explanation attached to every operation.
- **Keyboard controls** — arrow keys step through, spacebar toggles play/pause.
- **Grows over time** — a personal DSA learning log. Visualizers get added as I solve new problems; no roadmap, just whatever I'm working through next.
