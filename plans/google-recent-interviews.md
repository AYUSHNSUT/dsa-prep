# Google Interview Questions — Last 12 Months

Extracted from first-hand Google interview posts on LeetCode Discuss, 2025-09-28 to 2026-03-28 and 2026-03-29 to 2026-09-28:
**270 coding questions from 144 posts** (124 in the last 6 months, 146 in the 6 months before),
plus 16 system design / LLD / domain rounds, and Googleyness questions listed in 20 posts.
Levels: L4 119, L3 85, ? 29, L5 15, NG 13, Intern 5, Apprentice 4.
Most questions were custom "story" problems, so each is mapped to the closest LeetCode problem where one exists. ✓ = already solved (2026-09-28 snapshot).

## Takeaways

- Almost no question was a verbatim LeetCode problem; most were a known pattern wrapped in a story, with 1–3 follow-ups.
- Graphs dominate: 82 of 270 questions were graph problems (BFS, flood fill, Dijkstra, union-find, topological sort), versus 41 DP.
- Small "design a class" problems (logger, ad service, LRU/LFU, parking lot, waitlist, inventory) came up 38 times.
- Binary search on the answer came up 16 times, usually combined with BFS/Dijkstra; geometry with hash maps 10 times.
- Google reuses questions: 30 themes appeared in two or more independent posts, some 5–9 times.
- System design is rare below L5: only a handful of prompts were reported (YouTube captions, Inshorts, Snapchat, an employee cab service), mostly at L5 or in specialised roles; one L4 coding round included a short design section.

## Patterns (questions using each, ≥3)

| Pattern | 12 months | Last 6 months |
|---|---:|---:|
| DP | 41 | 23 |
| design (API / class) | 38 | 17 |
| hash map | 35 | 17 |
| BFS | 25 | 12 |
| heap / ordered set | 25 | 14 |
| DFS / flood fill | 22 | 10 |
| intervals / line sweep | 18 | 8 |
| tree | 18 | 4 |
| greedy | 17 | 6 |
| graph (other) | 17 | 7 |
| strings | 17 | 5 |
| binary search on answer | 16 | 8 |
| prefix sum | 15 | 9 |
| binary search | 15 | 4 |
| math / counting | 14 | 2 |
| union-find | 12 | 6 |
| shortest path (Dijkstra / minimax) | 10 | 6 |
| geometry | 10 | 5 |
| arrays / sorting | 10 | 1 |
| queue / stream | 9 | 1 |
| backtracking | 8 | 4 |
| sliding window | 7 | 3 |
| topological sort | 7 | 5 |
| monotonic stack / stack | 7 | 2 |
| segment tree / Fenwick | 6 | 3 |
| trie | 6 | 4 |
| linked list | 6 | 2 |
| two pointers | 5 | 0 |
| divide and conquer | 3 | 2 |

## Questions that recurred across independent posts

| Theme | Posts | Closest LeetCode |
|---|---:|---|
| Signal/threshold paths: binary search on answer + BFS/Dijkstra (safest path, min max edge) | 9 | [1631. Path With Minimum Effort](https://leetcode.com/problems/path-with-minimum-effort/) ✓, [1102. Path With Maximum Minimum Value](https://leetcode.com/problems/path-with-maximum-minimum-value/) 🔒, [2812. Find the Safest Path in a Grid](https://leetcode.com/problems/find-the-safest-path-in-a-grid/), [1970. Last Day Where You Can Still Cross](https://leetcode.com/problems/last-day-where-you-can-still-cross/) |
| Stream dedupe / logger / rate limiter variants | 8 | [359. Logger Rate Limiter](https://leetcode.com/problems/logger-rate-limiter/) 🔒 |
| Rectangles or squares from points / drawings (incl. rotated, empty rectangles) | 7 | [939. Minimum Area Rectangle](https://leetcode.com/problems/minimum-area-rectangle/), [963. Minimum Area Rectangle II](https://leetcode.com/problems/minimum-area-rectangle-ii/), [2013. Detect Squares](https://leetcode.com/problems/detect-squares/) |
| Topological sort for dependency ordering / validation | 6 | [207. Course Schedule](https://leetcode.com/problems/course-schedule/) ✓, [210. Course Schedule II](https://leetcode.com/problems/course-schedule-ii/) ✓ |
| Routers with a range: can a broadcast reach the destination (BFS) | 5 | — (custom) |
| Movie similarity graph -> top-k recommendations | 4 | [721. Accounts Merge](https://leetcode.com/problems/accounts-merge/) ✓, [215. Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array/) ✓ |
| Schedule tasks on CPUs; min CPUs for best finish time | 4 | [1834. Single-Threaded CPU](https://leetcode.com/problems/single-threaded-cpu/), [2187. Minimum Time to Complete Trips](https://leetcode.com/problems/minimum-time-to-complete-trips/) |
| Kadane / prefix-sum subarray variants | 4 | [53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/) ✓, [3026. Maximum Good Subarray Sum](https://leetcode.com/problems/maximum-good-subarray-sum/) |
| Lakes inside an island (flood fill) | 3 | [200. Number of Islands](https://leetcode.com/problems/number-of-islands/) ✓, [1254. Number of Closed Islands](https://leetcode.com/problems/number-of-closed-islands/) |
| AdService: heap, no consecutive repeats, cooldown follow-up | 3 | [621. Task Scheduler](https://leetcode.com/problems/task-scheduler/), [767. Reorganize String](https://leetcode.com/problems/reorganize-string/) ✓, [358. Rearrange String k Distance Apart](https://leetcode.com/problems/rearrange-string-k-distance-apart/) 🔒 |
| Fastest-reachable favourite city (Dijkstra) + via-vertex follow-up | 3 | [743. Network Delay Time](https://leetcode.com/problems/network-delay-time/) ✓ |
| Chat events: most active user, then top K | 3 | — (custom) |
| LRU / LFU cache variants (expiry, custom eviction) | 3 | [146. LRU Cache](https://leetcode.com/problems/lru-cache/) ✓, [460. LFU Cache](https://leetcode.com/problems/lfu-cache/) |
| File-system tree: sizes, structure, recursion | 3 | [588. Design In-Memory File System](https://leetcode.com/problems/design-in-memory-file-system/) 🔒 |
| Who is present in each time segment (merge schedules) | 2 | [759. Employee Free Time](https://leetcode.com/problems/employee-free-time/) 🔒 |
| Find the missing rook with a countRooks(rectangle) API | 2 | — (custom) |
| Find all 1s in a sparse bit array using query(L, R) | 2 | — (custom) |
| Linked list with chained hashes: build, reverse, validate | 2 | [206. Reverse Linked List](https://leetcode.com/problems/reverse-linked-list/) ✓ |
| Unlock patterns on a dot grid (backtracking + symmetry) | 2 | [351. Android Unlock Patterns](https://leetcode.com/problems/android-unlock-patterns/) 🔒 |
| Split data into fewest packets <= C, minimise the largest | 2 | — (custom) |
| APK / OS version range queries | 2 | — (custom) |
| Run-length encoding with get(i) | 2 | — (custom) |
| Event/RPC logs: detect timeouts early, bounded memory | 2 | — (custom) |
| Min-price order book with removals (heap / ordered set) | 2 | [1801. Number of Orders in the Backlog](https://leetcode.com/problems/number-of-orders-in-the-backlog/), [2034. Stock Price Fluctuation](https://leetcode.com/problems/stock-price-fluctuation/) |
| Tree DP: min cost to cut all leaves off the root | 2 | — (custom) |
| Root a tree as a binary tree with alternating level colours | 2 | — (custom) |
| LIS with difference 1, then difference <= d | 2 | [1218. Longest Arithmetic Subsequence of Given Difference](https://leetcode.com/problems/longest-arithmetic-subsequence-of-given-difference/), [2407. Longest Increasing Subsequence II](https://leetcode.com/problems/longest-increasing-subsequence-ii/) |
| Earliest time everyone is connected (union-find over time) | 2 | [1101. The Earliest Moment When Everyone Become Friends](https://leetcode.com/problems/the-earliest-moment-when-everyone-become-friends/) 🔒 |
| Longest grid path with "jump back up to previous height" rule | 2 | [329. Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix/) |
| Minimum Time to Finish the Race (tyre DP) | 2 | [2188. Minimum Time to Finish the Race](https://leetcode.com/problems/minimum-time-to-finish-the-race/) |

## Practice list: mapped problems not yet solved (72)

Number = reported questions that map to it, or posts in its recurring theme, whichever is higher.

- [ ] [1102. Path With Maximum Minimum Value](https://leetcode.com/problems/path-with-maximum-minimum-value/) 🔒 — 9
- [ ] [1970. Last Day Where You Can Still Cross](https://leetcode.com/problems/last-day-where-you-can-still-cross/) — 9
- [ ] [2812. Find the Safest Path in a Grid](https://leetcode.com/problems/find-the-safest-path-in-a-grid/) — 9
- [ ] [359. Logger Rate Limiter](https://leetcode.com/problems/logger-rate-limiter/) 🔒 — 8
- [ ] [939. Minimum Area Rectangle](https://leetcode.com/problems/minimum-area-rectangle/) — 7
- [ ] [963. Minimum Area Rectangle II](https://leetcode.com/problems/minimum-area-rectangle-ii/) — 7
- [ ] [2013. Detect Squares](https://leetcode.com/problems/detect-squares/) — 7
- [ ] [1834. Single-Threaded CPU](https://leetcode.com/problems/single-threaded-cpu/) — 4
- [ ] [2187. Minimum Time to Complete Trips](https://leetcode.com/problems/minimum-time-to-complete-trips/) — 4
- [ ] [3026. Maximum Good Subarray Sum](https://leetcode.com/problems/maximum-good-subarray-sum/) — 4
- [ ] [358. Rearrange String k Distance Apart](https://leetcode.com/problems/rearrange-string-k-distance-apart/) 🔒 — 3
- [ ] [460. LFU Cache](https://leetcode.com/problems/lfu-cache/) — 3
- [ ] [588. Design In-Memory File System](https://leetcode.com/problems/design-in-memory-file-system/) 🔒 — 3
- [ ] [621. Task Scheduler](https://leetcode.com/problems/task-scheduler/) — 3
- [ ] [759. Employee Free Time](https://leetcode.com/problems/employee-free-time/) 🔒 — 3
- [ ] [1254. Number of Closed Islands](https://leetcode.com/problems/number-of-closed-islands/) — 3
- [ ] [278. First Bad Version](https://leetcode.com/problems/first-bad-version/) — 2
- [ ] [329. Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix/) — 2
- [ ] [351. Android Unlock Patterns](https://leetcode.com/problems/android-unlock-patterns/) 🔒 — 2
- [ ] [994. Rotting Oranges](https://leetcode.com/problems/rotting-oranges/) — 2
- [ ] [1101. The Earliest Moment When Everyone Become Friends](https://leetcode.com/problems/the-earliest-moment-when-everyone-become-friends/) 🔒 — 2
- [ ] [1218. Longest Arithmetic Subsequence of Given Difference](https://leetcode.com/problems/longest-arithmetic-subsequence-of-given-difference/) — 2
- [ ] [1293. Shortest Path in a Grid with Obstacles Elimination](https://leetcode.com/problems/shortest-path-in-a-grid-with-obstacles-elimination/) — 2
- [ ] [1801. Number of Orders in the Backlog](https://leetcode.com/problems/number-of-orders-in-the-backlog/) — 2
- [ ] [2034. Stock Price Fluctuation](https://leetcode.com/problems/stock-price-fluctuation/) — 2
- [ ] [2188. Minimum Time to Finish the Race](https://leetcode.com/problems/minimum-time-to-finish-the-race/) — 2
- [ ] [2407. Longest Increasing Subsequence II](https://leetcode.com/problems/longest-increasing-subsequence-ii/) — 2
- [ ] [99. Recover Binary Search Tree](https://leetcode.com/problems/recover-binary-search-tree/) — 1
- [ ] [114. Flatten Binary Tree to Linked List](https://leetcode.com/problems/flatten-binary-tree-to-linked-list/) — 1
- [ ] [202. Happy Number](https://leetcode.com/problems/happy-number/) — 1
- [ ] [221. Maximal Square](https://leetcode.com/problems/maximal-square/) — 1
- [ ] [249. Group Shifted Strings](https://leetcode.com/problems/group-shifted-strings/) 🔒 — 1
- [ ] [253. Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii/) 🔒 — 1
- [ ] [261. Graph Valid Tree](https://leetcode.com/problems/graph-valid-tree/) 🔒 — 1
- [ ] [304. Range Sum Query 2D - Immutable](https://leetcode.com/problems/range-sum-query-2d-immutable/) — 1
- [ ] [337. House Robber III](https://leetcode.com/problems/house-robber-iii/) — 1
- [ ] [354. Russian Doll Envelopes](https://leetcode.com/problems/russian-doll-envelopes/) — 1
- [ ] [381. Insert Delete GetRandom O(1) - Duplicates allowed](https://leetcode.com/problems/insert-delete-getrandom-o1-duplicates-allowed/) — 1
- [ ] [387. First Unique Character in a String](https://leetcode.com/problems/first-unique-character-in-a-string/) — 1
- [ ] [410. Split Array Largest Sum](https://leetcode.com/problems/split-array-largest-sum/) — 1
- [ ] [442. Find All Duplicates in an Array](https://leetcode.com/problems/find-all-duplicates-in-an-array/) — 1
- [ ] [486. Predict the Winner](https://leetcode.com/problems/predict-the-winner/) — 1
- [ ] [494. Target Sum](https://leetcode.com/problems/target-sum/) — 1
- [ ] [687. Longest Univalue Path](https://leetcode.com/problems/longest-univalue-path/) — 1
- [ ] [715. Range Module](https://leetcode.com/problems/range-module/) — 1
- [ ] [784. Letter Case Permutation](https://leetcode.com/problems/letter-case-permutation/) — 1
- [ ] [809. Expressive Words](https://leetcode.com/problems/expressive-words/) — 1
- [ ] [811. Subdomain Visit Count](https://leetcode.com/problems/subdomain-visit-count/) — 1
- [ ] [846. Hand of Straights](https://leetcode.com/problems/hand-of-straights/) — 1
- [ ] [850. Rectangle Area II](https://leetcode.com/problems/rectangle-area-ii/) — 1
- [ ] [877. Stone Game](https://leetcode.com/problems/stone-game/) — 1
- [ ] [905. Sort Array By Parity](https://leetcode.com/problems/sort-array-by-parity/) — 1
- [ ] [925. Long Pressed Name](https://leetcode.com/problems/long-pressed-name/) — 1
- [ ] [1047. Remove All Adjacent Duplicates In String](https://leetcode.com/problems/remove-all-adjacent-duplicates-in-string/) — 1
- [ ] [1167. Minimum Cost to Connect Sticks](https://leetcode.com/problems/minimum-cost-to-connect-sticks/) 🔒 — 1
- [ ] [1296. Divide Array in Sets of K Consecutive Numbers](https://leetcode.com/problems/divide-array-in-sets-of-k-consecutive-numbers/) — 1
- [ ] [1339. Maximum Product of Splitted Binary Tree](https://leetcode.com/problems/maximum-product-of-splitted-binary-tree/) — 1
- [ ] [1361. Validate Binary Tree Nodes](https://leetcode.com/problems/validate-binary-tree-nodes/) — 1
- [ ] [1443. Minimum Time to Collect All Apples in a Tree](https://leetcode.com/problems/minimum-time-to-collect-all-apples-in-a-tree/) — 1
- [ ] [1462. Course Schedule IV](https://leetcode.com/problems/course-schedule-iv/) — 1
- [ ] [1514. Path with Maximum Probability](https://leetcode.com/problems/path-with-maximum-probability/) — 1
- [ ] [1671. Minimum Number of Removals to Make Mountain Array](https://leetcode.com/problems/minimum-number-of-removals-to-make-mountain-array/) — 1
- [ ] [1882. Process Tasks Using Servers](https://leetcode.com/problems/process-tasks-using-servers/) — 1
- [ ] [2296. Design a Text Editor](https://leetcode.com/problems/design-a-text-editor/) — 1
- [ ] [2316. Count Unreachable Pairs of Nodes in an Undirected Graph](https://leetcode.com/problems/count-unreachable-pairs-of-nodes-in-an-undirected-graph/) — 1
- [ ] [2359. Find Closest Node to Given Two Nodes](https://leetcode.com/problems/find-closest-node-to-given-two-nodes/) — 1
- [ ] [2364. Count Number of Bad Pairs](https://leetcode.com/problems/count-number-of-bad-pairs/) — 1
- [ ] [3284. Sum of Consecutive Subarrays](https://leetcode.com/problems/sum-of-consecutive-subarrays/) 🔒 — 1
- [ ] [3453. Separate Squares I](https://leetcode.com/problems/separate-squares-i/) — 1
- [ ] [3481. Apply Substitutions](https://leetcode.com/problems/apply-substitutions/) 🔒 — 1
- [ ] [3532. Path Existence Queries in a Graph I](https://leetcode.com/problems/path-existence-queries-in-a-graph-i/) — 1
- [ ] [3738. Longest Non-Decreasing Subarray After Replacing at Most One Element](https://leetcode.com/problems/longest-non-decreasing-subarray-after-replacing-at-most-one-element/) — 1

## Mapped problems already solved (37) — revise these

- [1631. Path With Minimum Effort](https://leetcode.com/problems/path-with-minimum-effort/) — 9
- [207. Course Schedule](https://leetcode.com/problems/course-schedule/) — 6
- [210. Course Schedule II](https://leetcode.com/problems/course-schedule-ii/) — 6
- [53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/) — 4
- [56. Merge Intervals](https://leetcode.com/problems/merge-intervals/) — 4
- [215. Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array/) — 4
- [721. Accounts Merge](https://leetcode.com/problems/accounts-merge/) — 4
- [743. Network Delay Time](https://leetcode.com/problems/network-delay-time/) — 4
- [146. LRU Cache](https://leetcode.com/problems/lru-cache/) — 3
- [200. Number of Islands](https://leetcode.com/problems/number-of-islands/) — 3
- [208. Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree/) — 3
- [347. Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements/) — 3
- [416. Partition Equal Subset Sum](https://leetcode.com/problems/partition-equal-subset-sum/) — 3
- [767. Reorganize String](https://leetcode.com/problems/reorganize-string/) — 3
- [787. Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops/) — 3
- [91. Decode Ways](https://leetcode.com/problems/decode-ways/) — 2
- [206. Reverse Linked List](https://leetcode.com/problems/reverse-linked-list/) — 2
- [1235. Maximum Profit in Job Scheduling](https://leetcode.com/problems/maximum-profit-in-job-scheduling/) — 2
- [1944. Number of Visible People in a Queue](https://leetcode.com/problems/number-of-visible-people-in-a-queue/) — 2
- [21. Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists/) — 1
- [41. First Missing Positive](https://leetcode.com/problems/first-missing-positive/) — 1
- [57. Insert Interval](https://leetcode.com/problems/insert-interval/) — 1
- [60. Permutation Sequence](https://leetcode.com/problems/permutation-sequence/) — 1
- [62. Unique Paths](https://leetcode.com/problems/unique-paths/) — 1
- [64. Minimum Path Sum](https://leetcode.com/problems/minimum-path-sum/) — 1
- [78. Subsets](https://leetcode.com/problems/subsets/) — 1
- [133. Clone Graph](https://leetcode.com/problems/clone-graph/) — 1
- [139. Word Break](https://leetcode.com/problems/word-break/) — 1
- [238. Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self/) — 1
- [239. Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum/) — 1
- [295. Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream/) — 1
- [297. Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree/) — 1
- [301. Remove Invalid Parentheses](https://leetcode.com/problems/remove-invalid-parentheses/) — 1
- [332. Reconstruct Itinerary](https://leetcode.com/problems/reconstruct-itinerary/) — 1
- [380. Insert Delete GetRandom O(1)](https://leetcode.com/problems/insert-delete-getrandom-o1/) — 1
- [485. Max Consecutive Ones](https://leetcode.com/problems/max-consecutive-ones/) — 1
- [1004. Max Consecutive Ones III](https://leetcode.com/problems/max-consecutive-ones-iii/) — 1

## System design, LLD and domain rounds

- **system design** (L5, last 6 mo): Design YouTube closed captioning: architecture, reducing data load, local storage
- **system design** (L5, last 6 mo): Rate limiter: fixed vs sliding window, token/leaky bucket trade-offs
- **system design** (L5, 6–12 mo): Design Inshorts (news summaries); dedupe summaries of the same story from different sources
- **system design** (?, 6–12 mo): Design Snapchat
- **system design** (L4, 6–12 mo): System design section inside a coding round (topic not given)
- **system design** (?, 6–12 mo): Google's employee cab service: allocation, routing, scheduling at scale
- **LLD** (L4, last 6 mo): Multi-user heart-rate monitor: classes, relationships, data structures
- **LLD** (?, 6–12 mo): Application Engineer loop: LLD round and a system-integration round (topics not given)
- **LLD** (L4, 6–12 mo): Application Engineer: design a mall parking system (requirements, APIs)
- **domain** (L4/L5, last 6 mo): ML system design: a Google Reviews-like system (NLP pipeline, BERT vs LLM trade-offs)
- **domain** (L4, last 6 mo): SRE loops may use NALSD: capacity and latency estimates worked out by hand
- **domain** (L3, 6–12 mo): WSE: SQL joins/aggregation/ranking; propose a Google Maps feature recommending businesses
- **domain** (L4, 6–12 mo): AI/ML round: classify which array a query value belongs to (clustering)
- **domain** (L4, 6–12 mo): Application Engineer: integrate Workday with a payroll system for hires/updates
- **domain** (L4, 6–12 mo): Android domain round (framework fundamentals)
- **domain** (L3, 6–12 mo): WSE web: what happens when you type a URL; SSR vs CSR; optimise a site across frontend/backend/DB

## Googleyness themes

Grouped from the questions candidates listed. Prepare one STAR story per theme; the top five cover most rounds.

| Theme | Posts | Example prompts |
|---|---:|---|
| Conflict and disagreement | 12 | Conflict management; People disagreeing with the majority on a non-work matter; Disagreement with a colleague or manager |
| Deadlines, priorities and juggling projects | 9 | Handling missed deadlines; Juggling multiple tasks and priorities; A time you faced a deadline |
| Your projects, motivation and goals | 8 | A career goal for the near future; A challenging technical problem you solved; Tell me about yourself |
| Leadership, management, culture | 6 | Manager setting reasonable, then unreasonable demands; If you were CTO, what would you change; Your ideal manager |
| Failure, mistakes and self-improvement | 5 | A time you changed your work style; A mistake you made; An instance of self-improvement |
| Helping, mentoring, underperformers | 5 | Helping an underperforming team member improve; A time you helped someone; Helping someone outside your team |
| Ownership beyond your scope | 4 | Taking ownership outside your responsibility; Taking ownership; Ownership and decision-making |
| Someone taking credit for your work | 3 | Someone repeatedly taking credit for your work; Someone taking credit for your work; Someone took credit for your work |
| Ambiguity and unclear requirements | 3 | Handling unclear goals; Unclear requirements; Ambiguous scenarios |
| Using AI in your work | 2 | How you use AI in your daily work; How you use AI in your workflow; Do you give AI full ownership of a project |
| Giving and receiving feedback | 2 | Giving critical feedback to someone; Receiving critical feedback |
| Hypotheticals (outings, unhappy customers, ideal workplace) | 2 | What you would want at work that does not exist today; Customers are unhappy with your product: what do you do; Your ideal software engineer |
