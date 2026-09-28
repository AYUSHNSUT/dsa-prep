# Recent Google Interview Questions (2026-03-29 to 2026-09-28)

Extracted from first-hand Google interview posts on LeetCode Discuss. 123 coding questions from 64 posts
(levels: L4 72, L3 36, ? 9, L5 5, Intern 1; rounds: onsite 84, screen 38, OA 1).
Most were custom "story" problems, so each is mapped to the closest LeetCode problem where one exists. ✓ = already solved (2026-09-28 snapshot).

## Takeaways

- Almost no question was a verbatim LeetCode problem; most were a known pattern wrapped in a story, with 1–3 follow-ups.
- Graphs dominate: 42 of 123 questions were graph problems (BFS, flood fill, Dijkstra, union-find, topological sort), versus 23 DP.
- Design-style classes (AdService, logger, LFU, text editor, route matcher) came up 16 times; binary search on the answer 8 times, often combined with BFS/Dijkstra.
- Geometry with hash maps (rectangles/squares from points) came up 5 times, far more than its LeetCode frequency suggests.

## Patterns (questions using each, ≥2)

| Pattern | Questions |
|---|---:|
| DP | 23 |
| hash map | 17 |
| design (API / class) | 16 |
| heap | 14 |
| BFS | 12 |
| DFS / flood fill | 10 |
| prefix sum | 9 |
| binary search on answer | 8 |
| intervals / line sweep | 8 |
| graph (other) | 7 |
| shortest path (Dijkstra / minimax) | 6 |
| union-find | 6 |
| greedy | 6 |
| geometry | 5 |
| strings | 5 |
| topological sort | 5 |
| tree | 4 |
| binary search | 4 |
| trie | 4 |
| backtracking | 4 |
| sliding window | 3 |
| segment tree | 3 |
| divide and conquer | 2 |
| monotonic stack | 2 |
| linked list | 2 |

## Questions that recurred across independent posts

| Theme | Posts | Closest LeetCode |
|---|---:|---|
| Max-area rectangle / square from points, including rotated | 5 | [939. Minimum Area Rectangle](https://leetcode.com/problems/minimum-area-rectangle/), [963. Minimum Area Rectangle II](https://leetcode.com/problems/minimum-area-rectangle-ii/), [2013. Detect Squares](https://leetcode.com/problems/detect-squares/) |
| Topological sort for dependency ordering / validation | 5 | [207. Course Schedule](https://leetcode.com/problems/course-schedule/) ✓, [210. Course Schedule II](https://leetcode.com/problems/course-schedule-ii/) ✓ |
| Min/max threshold path: binary search on answer + BFS/Dijkstra | 5 | [1631. Path With Minimum Effort](https://leetcode.com/problems/path-with-minimum-effort/) ✓, [1102. Path With Maximum Minimum Value](https://leetcode.com/problems/path-with-maximum-minimum-value/) 🔒, [2812. Find the Safest Path in a Grid](https://leetcode.com/problems/find-the-safest-path-in-a-grid/), [1293. Shortest Path in a Grid with Obstacles Elimination](https://leetcode.com/problems/shortest-path-in-a-grid-with-obstacles-elimination/) |
| Kadane / prefix-sum subarray variants | 4 | [53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/) ✓, [3026. Maximum Good Subarray Sum](https://leetcode.com/problems/maximum-good-subarray-sum/) |
| Stream dedupe / logger / rate limiter variants | 4 | [359. Logger Rate Limiter](https://leetcode.com/problems/logger-rate-limiter/) 🔒 |
| Lakes inside an island (flood fill) | 3 | [200. Number of Islands](https://leetcode.com/problems/number-of-islands/) ✓, [1254. Number of Closed Islands](https://leetcode.com/problems/number-of-closed-islands/) |
| AdService: heap, no consecutive repeats, cooldown follow-up | 3 | [621. Task Scheduler](https://leetcode.com/problems/task-scheduler/), [767. Reorganize String](https://leetcode.com/problems/reorganize-string/) ✓, [358. Rearrange String k Distance Apart](https://leetcode.com/problems/rearrange-string-k-distance-apart/) 🔒 |
| Movie similarity graph -> top-k recommendations | 3 | [721. Accounts Merge](https://leetcode.com/problems/accounts-merge/) ✓ |
| Tree DP: min cost to cut all leaves off the root | 2 | — (custom) |
| Root a tree as a binary tree with alternating level colours | 2 | — (custom) |
| LIS with difference 1, then difference <= d | 2 | [1218. Longest Arithmetic Subsequence of Given Difference](https://leetcode.com/problems/longest-arithmetic-subsequence-of-given-difference/), [2407. Longest Increasing Subsequence II](https://leetcode.com/problems/longest-increasing-subsequence-ii/) |
| Earliest time everyone is connected (union-find over time) | 2 | [1101. The Earliest Moment When Everyone Become Friends](https://leetcode.com/problems/the-earliest-moment-when-everyone-become-friends/) 🔒 |
| Schedule tasks on CPUs; min CPUs for best finish time | 2 | [1834. Single-Threaded CPU](https://leetcode.com/problems/single-threaded-cpu/), [2187. Minimum Time to Complete Trips](https://leetcode.com/problems/minimum-time-to-complete-trips/) |
| Longest path in grid with "jump back up to previous height" rule | 2 | [329. Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix/) |
| Flights/airports with times: earliest arrival | 2 | [787. Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops/) ✓ |
| Minimum Time to Finish the Race (tyre DP) | 2 | [2188. Minimum Time to Finish the Race](https://leetcode.com/problems/minimum-time-to-finish-the-race/) |

## Practice list: mapped problems not yet solved (44)

- [ ] [359. Logger Rate Limiter](https://leetcode.com/problems/logger-rate-limiter/) 🔒 — seen in 4 question(s)
- [ ] [963. Minimum Area Rectangle II](https://leetcode.com/problems/minimum-area-rectangle-ii/) — seen in 4 question(s)
- [ ] [621. Task Scheduler](https://leetcode.com/problems/task-scheduler/) — seen in 3 question(s)
- [ ] [939. Minimum Area Rectangle](https://leetcode.com/problems/minimum-area-rectangle/) — seen in 3 question(s)
- [ ] [1254. Number of Closed Islands](https://leetcode.com/problems/number-of-closed-islands/) — seen in 3 question(s)
- [ ] [329. Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix/) — seen in 2 question(s)
- [ ] [460. LFU Cache](https://leetcode.com/problems/lfu-cache/) — seen in 2 question(s)
- [ ] [994. Rotting Oranges](https://leetcode.com/problems/rotting-oranges/) — seen in 2 question(s)
- [ ] [1101. The Earliest Moment When Everyone Become Friends](https://leetcode.com/problems/the-earliest-moment-when-everyone-become-friends/) 🔒 — seen in 2 question(s)
- [ ] [1102. Path With Maximum Minimum Value](https://leetcode.com/problems/path-with-maximum-minimum-value/) 🔒 — seen in 2 question(s)
- [ ] [1218. Longest Arithmetic Subsequence of Given Difference](https://leetcode.com/problems/longest-arithmetic-subsequence-of-given-difference/) — seen in 2 question(s)
- [ ] [1293. Shortest Path in a Grid with Obstacles Elimination](https://leetcode.com/problems/shortest-path-in-a-grid-with-obstacles-elimination/) — seen in 2 question(s)
- [ ] [1834. Single-Threaded CPU](https://leetcode.com/problems/single-threaded-cpu/) — seen in 2 question(s)
- [ ] [2187. Minimum Time to Complete Trips](https://leetcode.com/problems/minimum-time-to-complete-trips/) — seen in 2 question(s)
- [ ] [2188. Minimum Time to Finish the Race](https://leetcode.com/problems/minimum-time-to-finish-the-race/) — seen in 2 question(s)
- [ ] [2407. Longest Increasing Subsequence II](https://leetcode.com/problems/longest-increasing-subsequence-ii/) — seen in 2 question(s)
- [ ] [3026. Maximum Good Subarray Sum](https://leetcode.com/problems/maximum-good-subarray-sum/) — seen in 2 question(s)
- [ ] [99. Recover Binary Search Tree](https://leetcode.com/problems/recover-binary-search-tree/) — seen in 1 question(s)
- [ ] [114. Flatten Binary Tree to Linked List](https://leetcode.com/problems/flatten-binary-tree-to-linked-list/) — seen in 1 question(s)
- [ ] [249. Group Shifted Strings](https://leetcode.com/problems/group-shifted-strings/) 🔒 — seen in 1 question(s)
- [ ] [253. Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii/) 🔒 — seen in 1 question(s)
- [ ] [337. House Robber III](https://leetcode.com/problems/house-robber-iii/) — seen in 1 question(s)
- [ ] [358. Rearrange String k Distance Apart](https://leetcode.com/problems/rearrange-string-k-distance-apart/) 🔒 — seen in 1 question(s)
- [ ] [381. Insert Delete GetRandom O(1) - Duplicates allowed](https://leetcode.com/problems/insert-delete-getrandom-o1-duplicates-allowed/) — seen in 1 question(s)
- [ ] [442. Find All Duplicates in an Array](https://leetcode.com/problems/find-all-duplicates-in-an-array/) — seen in 1 question(s)
- [ ] [494. Target Sum](https://leetcode.com/problems/target-sum/) — seen in 1 question(s)
- [ ] [687. Longest Univalue Path](https://leetcode.com/problems/longest-univalue-path/) — seen in 1 question(s)
- [ ] [759. Employee Free Time](https://leetcode.com/problems/employee-free-time/) 🔒 — seen in 1 question(s)
- [ ] [784. Letter Case Permutation](https://leetcode.com/problems/letter-case-permutation/) — seen in 1 question(s)
- [ ] [809. Expressive Words](https://leetcode.com/problems/expressive-words/) — seen in 1 question(s)
- [ ] [846. Hand of Straights](https://leetcode.com/problems/hand-of-straights/) — seen in 1 question(s)
- [ ] [850. Rectangle Area II](https://leetcode.com/problems/rectangle-area-ii/) — seen in 1 question(s)
- [ ] [925. Long Pressed Name](https://leetcode.com/problems/long-pressed-name/) — seen in 1 question(s)
- [ ] [1167. Minimum Cost to Connect Sticks](https://leetcode.com/problems/minimum-cost-to-connect-sticks/) 🔒 — seen in 1 question(s)
- [ ] [1296. Divide Array in Sets of K Consecutive Numbers](https://leetcode.com/problems/divide-array-in-sets-of-k-consecutive-numbers/) — seen in 1 question(s)
- [ ] [1462. Course Schedule IV](https://leetcode.com/problems/course-schedule-iv/) — seen in 1 question(s)
- [ ] [1801. Number of Orders in the Backlog](https://leetcode.com/problems/number-of-orders-in-the-backlog/) — seen in 1 question(s)
- [ ] [1882. Process Tasks Using Servers](https://leetcode.com/problems/process-tasks-using-servers/) — seen in 1 question(s)
- [ ] [2013. Detect Squares](https://leetcode.com/problems/detect-squares/) — seen in 1 question(s)
- [ ] [2296. Design a Text Editor](https://leetcode.com/problems/design-a-text-editor/) — seen in 1 question(s)
- [ ] [2359. Find Closest Node to Given Two Nodes](https://leetcode.com/problems/find-closest-node-to-given-two-nodes/) — seen in 1 question(s)
- [ ] [2812. Find the Safest Path in a Grid](https://leetcode.com/problems/find-the-safest-path-in-a-grid/) — seen in 1 question(s)
- [ ] [3453. Separate Squares I](https://leetcode.com/problems/separate-squares-i/) — seen in 1 question(s)
- [ ] [3481. Apply Substitutions](https://leetcode.com/problems/apply-substitutions/) 🔒 — seen in 1 question(s)

## Mapped problems already solved (26) — revise these

- [207. Course Schedule](https://leetcode.com/problems/course-schedule/) — seen in 3
- [208. Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree/) — seen in 3
- [210. Course Schedule II](https://leetcode.com/problems/course-schedule-ii/) — seen in 3
- [53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/) — seen in 2
- [200. Number of Islands](https://leetcode.com/problems/number-of-islands/) — seen in 2
- [416. Partition Equal Subset Sum](https://leetcode.com/problems/partition-equal-subset-sum/) — seen in 2
- [743. Network Delay Time](https://leetcode.com/problems/network-delay-time/) — seen in 2
- [787. Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops/) — seen in 2
- [1235. Maximum Profit in Job Scheduling](https://leetcode.com/problems/maximum-profit-in-job-scheduling/) — seen in 2
- [1631. Path With Minimum Effort](https://leetcode.com/problems/path-with-minimum-effort/) — seen in 2
- [21. Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists/) — seen in 1
- [41. First Missing Positive](https://leetcode.com/problems/first-missing-positive/) — seen in 1
- [56. Merge Intervals](https://leetcode.com/problems/merge-intervals/) — seen in 1
- [62. Unique Paths](https://leetcode.com/problems/unique-paths/) — seen in 1
- [64. Minimum Path Sum](https://leetcode.com/problems/minimum-path-sum/) — seen in 1
- [78. Subsets](https://leetcode.com/problems/subsets/) — seen in 1
- [91. Decode Ways](https://leetcode.com/problems/decode-ways/) — seen in 1
- [139. Word Break](https://leetcode.com/problems/word-break/) — seen in 1
- [146. LRU Cache](https://leetcode.com/problems/lru-cache/) — seen in 1
- [206. Reverse Linked List](https://leetcode.com/problems/reverse-linked-list/) — seen in 1
- [238. Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self/) — seen in 1
- [301. Remove Invalid Parentheses](https://leetcode.com/problems/remove-invalid-parentheses/) — seen in 1
- [380. Insert Delete GetRandom O(1)](https://leetcode.com/problems/insert-delete-getrandom-o1/) — seen in 1
- [721. Accounts Merge](https://leetcode.com/problems/accounts-merge/) — seen in 1
- [767. Reorganize String](https://leetcode.com/problems/reorganize-string/) — seen in 1
- [1944. Number of Visible People in a Queue](https://leetcode.com/problems/number-of-visible-people-in-a-queue/) — seen in 1
