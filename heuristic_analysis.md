# Heuristic Analysis

## Hardware

Test were run on a MacBook Pro Retina, 15-inch, Mid 2014.

## Problem 1

### Solving Air Cargo Problem 1 using breadth_first_search...

| Expansions |  Goal Tests |  New Nodes | Plan Length | Time |
| ---------- | ----------- | ---------- | ----------- | ---- |
|    43      |    56       |  180       | 6           | 0.03169 |

Plan length: 6  Time elapsed in seconds: 0.03169219399933354

```
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P2, JFK, SFO)
Unload(C2, P2, SFO)
Fly(P1, SFO, JFK)
Unload(C1, P1, JFK)
```

### Solving Air Cargo Problem 1 using depth_first_graph_search...

| Expansions |  Goal Tests |  New Nodes | Plan Length | Time |
| ---------- | ----------- | ---------- | ----------- | ---- |
|    21      |    22       |   84       |   20        | 0.01332 |

Plan length: 20  Time elapsed in seconds: 0.013321993999852566
Fly(P1, SFO, JFK)
Fly(P2, JFK, SFO)
Load(C2, P1, JFK)
Fly(P1, JFK, SFO)
Fly(P2, SFO, JFK)
Unload(C2, P1, SFO)
Fly(P1, SFO, JFK)
Fly(P2, JFK, SFO)
Load(C2, P2, SFO)
Fly(P1, JFK, SFO)
Load(C1, P2, SFO)
Fly(P2, SFO, JFK)
Fly(P1, SFO, JFK)
Unload(C2, P2, JFK)
Unload(C1, P2, JFK)
Fly(P2, JFK, SFO)
Load(C2, P1, JFK)
Fly(P1, JFK, SFO)
Fly(P2, SFO, JFK)
Unload(C2, P1, SFO)

### Solving Air Cargo Problem 1 using uniform_cost_search...

| Expansions |  Goal Tests |  New Nodes | Plan Length | Time |
| ---------- | ----------- | ---------- | ----------- | ---- |
|    55      |    57       |  224       |  6          | 0.03671 |

Plan length: 6  Time elapsed in seconds: 0.03670633299952897
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P1, SFO, JFK)
Fly(P2, JFK, SFO)
Unload(C1, P1, JFK)
Unload(C2, P2, SFO)

## Problem 2

### Solving Air Cargo Problem 2 using breadth_first_search...

| Expansions |  Goal Tests |  New Nodes | Plan Length | Time |
| ---------- | ----------- | ---------- | ----------- | ---- |
|   3343     |   4609      | 30509      |  9          | 13.63831 |

Plan length: 9  Time elapsed in seconds: 13.638315716999955
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Load(C3, P3, ATL)
Fly(P2, JFK, SFO)
Unload(C2, P2, SFO)
Fly(P1, SFO, JFK)
Unload(C1, P1, JFK)
Fly(P3, ATL, SFO)
Unload(C3, P3, SFO)


### Solving Air Cargo Problem 2 using depth_first_graph_search...

| Expansions |  Goal Tests |  New Nodes | Plan Length | Time |
| ---------- | ----------- | ---------- | ----------- | ---- |
|   624      |   625       |  5602      | 619         | 3.53949 |

Plan length: 619  Time elapsed in seconds: 3.539487648999966
Fly(P3, ATL, SFO)
Fly(P1, SFO, ATL)
Fly(P3, SFO, JFK)
Fly(P1, ATL, JFK)
Fly(P2, JFK, ATL)
Fly(P3, JFK, ATL)
Fly(P2, ATL, SFO)
Fly(P3, ATL, SFO)
Load(C2, P1, JFK)
Fly(P2, SFO, ATL)
Fly(P1, JFK, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, SFO)
Fly(P3, SFO, ATL)
Fly(P1, SFO, JFK)
Load(C3, P3, ATL)
Fly(P3, ATL, SFO)
Fly(P2, JFK, ATL)
Fly(P3, SFO, JFK)
Fly(P2, ATL, SFO)
Fly(P1, JFK, ATL)
Fly(P2, SFO, JFK)
Fly(P1, ATL, SFO)
Unload(C3, P3, JFK)
Fly(P1, SFO, JFK)
Fly(P3, JFK, ATL)
Fly(P2, JFK, ATL)
Fly(P3, ATL, SFO)
Fly(P2, ATL, SFO)
Fly(P1, JFK, ATL)
Fly(P3, SFO, ATL)
Fly(P1, ATL, SFO)
Unload(C2, P1, SFO)
Fly(P3, ATL, SFO)
Fly(P2, SFO, ATL)
Fly(P1, SFO, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, JFK)
Fly(P3, SFO, ATL)
Fly(P2, JFK, ATL)
Fly(P3, ATL, JFK)
Fly(P2, ATL, SFO)
Fly(P1, JFK, ATL)
Load(C3, P3, JFK)
Fly(P1, ATL, SFO)
Fly(P2, SFO, ATL)
Fly(P3, JFK, ATL)
Fly(P2, ATL, JFK)
Fly(P3, ATL, SFO)
Fly(P1, SFO, ATL)
Fly(P2, JFK, ATL)
Fly(P1, ATL, JFK)
Fly(P2, ATL, SFO)
Fly(P3, SFO, ATL)
Unload(C3, P3, ATL)
Fly(P3, ATL, SFO)
Fly(P2, SFO, ATL)
Fly(P3, SFO, JFK)
Fly(P2, ATL, JFK)
Fly(P1, JFK, ATL)
Fly(P3, JFK, ATL)
Fly(P2, JFK, ATL)
Load(C3, P2, ATL)
Fly(P3, ATL, SFO)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Fly(P3, SFO, ATL)
Fly(P2, SFO, JFK)
Fly(P3, ATL, JFK)
Fly(P1, SFO, JFK)
Fly(P2, JFK, SFO)
Unload(C3, P2, SFO)
Fly(P2, SFO, ATL)
Fly(P3, JFK, ATL)
Fly(P2, ATL, JFK)
Fly(P3, ATL, SFO)
Load(C2, P3, SFO)
Fly(P3, SFO, ATL)
Fly(P2, JFK, ATL)
Fly(P3, ATL, JFK)
Fly(P2, ATL, SFO)
Fly(P1, JFK, ATL)
Fly(P2, SFO, JFK)
Fly(P1, ATL, SFO)
Unload(C2, P3, JFK)
Fly(P1, SFO, JFK)
Fly(P3, JFK, ATL)
Fly(P2, JFK, ATL)
Fly(P3, ATL, SFO)
Fly(P2, ATL, SFO)
Fly(P1, JFK, ATL)
Fly(P3, SFO, ATL)
Fly(P1, ATL, SFO)
Load(C3, P2, SFO)
Fly(P3, ATL, SFO)
Fly(P2, SFO, ATL)
Fly(P1, SFO, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, JFK)
Fly(P3, SFO, ATL)
Load(C2, P2, JFK)
Fly(P3, ATL, JFK)
Fly(P2, JFK, ATL)
Fly(P1, JFK, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Unload(C3, P2, SFO)
Fly(P2, SFO, ATL)
Fly(P1, SFO, ATL)
Fly(P2, ATL, JFK)
Fly(P3, JFK, ATL)
Fly(P1, ATL, SFO)
Fly(P3, ATL, SFO)
Fly(P1, SFO, JFK)
Fly(P2, JFK, ATL)
Fly(P3, SFO, ATL)
Fly(P2, ATL, SFO)
Load(C1, P2, SFO)
Fly(P3, ATL, SFO)
Fly(P2, SFO, ATL)
Fly(P3, SFO, JFK)
Fly(P2, ATL, JFK)
Fly(P1, JFK, ATL)
Fly(P3, JFK, ATL)
Fly(P1, ATL, SFO)
Fly(P3, ATL, SFO)
Unload(C2, P2, JFK)
Fly(P1, SFO, ATL)
Fly(P2, JFK, ATL)
Fly(P1, ATL, JFK)
Fly(P3, SFO, ATL)
Fly(P2, ATL, SFO)
Fly(P3, ATL, JFK)
Fly(P1, JFK, ATL)
Load(C3, P2, SFO)
Fly(P1, ATL, SFO)
Fly(P2, SFO, ATL)
Fly(P1, SFO, JFK)
Fly(P2, ATL, JFK)
Fly(P3, JFK, ATL)
Fly(P1, JFK, ATL)
Fly(P3, ATL, SFO)
Fly(P1, ATL, SFO)
Unload(C3, P2, JFK)
Fly(P3, SFO, ATL)
Fly(P2, JFK, ATL)
Fly(P3, ATL, JFK)
Fly(P2, ATL, SFO)
Fly(P1, SFO, ATL)
Fly(P2, SFO, JFK)
Unload(C1, P2, JFK)
Fly(P1, ATL, SFO)
Fly(P2, JFK, ATL)
Fly(P1, SFO, JFK)
Fly(P2, ATL, SFO)
Fly(P3, JFK, ATL)
Fly(P2, SFO, JFK)
Fly(P3, ATL, SFO)
Load(C3, P2, JFK)
Fly(P2, JFK, ATL)
Fly(P3, SFO, ATL)
Fly(P2, ATL, SFO)
Fly(P3, ATL, JFK)
Fly(P1, JFK, ATL)
Fly(P2, SFO, ATL)
Fly(P1, ATL, SFO)
Unload(C3, P2, ATL)
Fly(P2, ATL, SFO)
Fly(P1, SFO, ATL)
Fly(P2, SFO, JFK)
Fly(P1, ATL, JFK)
Fly(P3, JFK, ATL)
Fly(P2, JFK, SFO)
Fly(P3, ATL, SFO)
Load(C2, P1, JFK)
Fly(P2, SFO, ATL)
Fly(P3, SFO, ATL)
Fly(P1, JFK, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Fly(P3, ATL, JFK)
Fly(P2, SFO, ATL)
Unload(C2, P1, SFO)
Fly(P2, ATL, JFK)
Fly(P1, SFO, ATL)
Fly(P3, JFK, ATL)
Fly(P1, ATL, JFK)
Fly(P3, ATL, SFO)
Fly(P2, JFK, ATL)
Fly(P1, JFK, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Load(C2, P3, SFO)
Fly(P3, SFO, ATL)
Fly(P2, SFO, ATL)
Fly(P1, SFO, ATL)
Fly(P3, ATL, JFK)
Fly(P1, ATL, JFK)
Fly(P2, ATL, SFO)
Load(C1, P3, JFK)
Fly(P2, SFO, JFK)
Fly(P3, JFK, ATL)
Fly(P2, JFK, ATL)
Fly(P3, ATL, SFO)
Fly(P1, JFK, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Fly(P3, SFO, ATL)
Unload(C2, P3, ATL)
Fly(P3, ATL, SFO)
Fly(P2, SFO, ATL)
Fly(P1, SFO, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, JFK)
Fly(P3, SFO, JFK)
Fly(P2, JFK, ATL)
Unload(C1, P3, JFK)
Fly(P2, ATL, SFO)
Fly(P3, JFK, ATL)
Fly(P2, SFO, JFK)
Fly(P3, ATL, SFO)
Fly(P1, JFK, ATL)
Fly(P3, SFO, JFK)
Fly(P1, ATL, SFO)
Load(C1, P2, JFK)
Fly(P1, SFO, JFK)
Fly(P2, JFK, ATL)
Fly(P3, JFK, ATL)
Fly(P2, ATL, SFO)
Fly(P3, ATL, SFO)
Fly(P1, JFK, ATL)
Fly(P2, SFO, ATL)
Fly(P1, ATL, SFO)
Unload(C1, P2, ATL)
Fly(P2, ATL, SFO)
Fly(P1, SFO, ATL)
Fly(P3, SFO, ATL)
Fly(P1, ATL, JFK)
Fly(P3, ATL, JFK)
Fly(P2, SFO, JFK)
Fly(P1, JFK, ATL)
Fly(P2, JFK, ATL)
Load(C3, P2, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Fly(P2, SFO, JFK)
Fly(P1, SFO, JFK)
Fly(P3, JFK, ATL)
Fly(P2, JFK, ATL)
Fly(P3, ATL, SFO)
Fly(P2, ATL, SFO)
Unload(C3, P2, SFO)
Fly(P3, SFO, ATL)
Fly(P2, SFO, ATL)
Fly(P3, ATL, JFK)
Fly(P2, ATL, JFK)
Fly(P1, JFK, ATL)
Fly(P3, JFK, ATL)
Fly(P1, ATL, SFO)
Fly(P3, ATL, SFO)
Fly(P2, JFK, ATL)
Fly(P1, SFO, ATL)
Load(C3, P3, SFO)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Fly(P3, SFO, ATL)
Fly(P2, SFO, ATL)
Fly(P3, ATL, JFK)
Fly(P2, ATL, JFK)
Fly(P1, SFO, ATL)
Fly(P3, JFK, ATL)
Fly(P1, ATL, JFK)
Load(C2, P3, ATL)
Fly(P3, ATL, SFO)
Fly(P2, JFK, ATL)
Fly(P3, SFO, JFK)
Fly(P2, ATL, SFO)
Fly(P1, JFK, ATL)
Fly(P2, SFO, JFK)
Fly(P1, ATL, SFO)
Unload(C3, P3, JFK)
Fly(P1, SFO, JFK)
Fly(P3, JFK, ATL)
Fly(P2, JFK, ATL)
Fly(P3, ATL, SFO)
Fly(P2, ATL, SFO)
Fly(P1, JFK, ATL)
Fly(P3, SFO, ATL)
Fly(P1, ATL, SFO)
Unload(C2, P3, ATL)
Fly(P3, ATL, SFO)
Fly(P2, SFO, ATL)
Fly(P1, SFO, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, JFK)
Load(C3, P1, JFK)
Fly(P3, SFO, ATL)
Fly(P2, JFK, ATL)
Fly(P3, ATL, JFK)
Fly(P2, ATL, SFO)
Fly(P1, JFK, ATL)
Load(C2, P1, ATL)
Fly(P1, ATL, SFO)
Fly(P2, SFO, ATL)
Fly(P1, SFO, JFK)
Fly(P2, ATL, JFK)
Fly(P3, JFK, ATL)
Fly(P1, JFK, ATL)
Fly(P3, ATL, SFO)
Fly(P1, ATL, SFO)
Unload(C3, P1, SFO)
Fly(P3, SFO, ATL)
Fly(P1, SFO, JFK)
Fly(P3, ATL, JFK)
Fly(P2, JFK, ATL)
Fly(P1, JFK, ATL)
Fly(P2, ATL, SFO)
Fly(P3, JFK, ATL)
Load(C3, P2, SFO)
Fly(P3, ATL, SFO)
Fly(P1, ATL, SFO)
Fly(P2, SFO, ATL)
Fly(P3, SFO, ATL)
Fly(P2, ATL, JFK)
Fly(P3, ATL, JFK)
Fly(P1, SFO, ATL)
Unload(C3, P2, JFK)
Fly(P3, JFK, ATL)
Fly(P2, JFK, ATL)
Fly(P1, ATL, SFO)
Fly(P3, ATL, SFO)
Fly(P2, ATL, SFO)
Fly(P1, SFO, ATL)
Load(C1, P1, ATL)
Fly(P1, ATL, SFO)
Fly(P2, SFO, ATL)
Fly(P3, SFO, ATL)
Fly(P2, ATL, JFK)
Fly(P1, SFO, JFK)
Fly(P3, ATL, SFO)
Load(C3, P2, JFK)
Fly(P3, SFO, JFK)
Fly(P2, JFK, ATL)
Fly(P3, JFK, ATL)
Fly(P2, ATL, SFO)
Fly(P1, JFK, SFO)
Fly(P3, ATL, SFO)
Fly(P2, SFO, ATL)
Fly(P1, SFO, ATL)
Unload(C3, P2, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Fly(P3, SFO, ATL)
Fly(P2, SFO, ATL)
Fly(P3, ATL, JFK)
Fly(P2, ATL, JFK)
Fly(P1, SFO, ATL)
Fly(P3, JFK, ATL)
Fly(P1, ATL, JFK)
Fly(P3, ATL, SFO)
Unload(C2, P1, JFK)
Fly(P2, JFK, ATL)
Fly(P3, SFO, ATL)
Fly(P1, JFK, ATL)
Fly(P2, ATL, SFO)
Fly(P3, ATL, SFO)
Fly(P1, ATL, SFO)
Fly(P3, SFO, JFK)
Fly(P2, SFO, ATL)
Load(C3, P2, ATL)
Fly(P2, ATL, SFO)
Fly(P1, SFO, ATL)
Fly(P2, SFO, JFK)
Fly(P3, JFK, ATL)
Fly(P1, ATL, SFO)
Fly(P3, ATL, SFO)
Unload(C3, P2, JFK)
Fly(P1, SFO, ATL)
Fly(P2, JFK, ATL)
Fly(P1, ATL, JFK)
Fly(P2, ATL, SFO)
Load(C3, P1, JFK)
Fly(P3, SFO, ATL)
Fly(P2, SFO, ATL)
Fly(P3, ATL, JFK)
Fly(P2, ATL, JFK)
Fly(P1, JFK, ATL)
Fly(P3, JFK, ATL)
Fly(P1, ATL, SFO)
Fly(P3, ATL, SFO)
Fly(P2, JFK, ATL)
Fly(P1, SFO, ATL)
Unload(C1, P1, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Fly(P3, SFO, ATL)
Fly(P2, SFO, ATL)
Fly(P3, ATL, JFK)
Fly(P2, ATL, JFK)
Unload(C3, P1, SFO)
Fly(P1, SFO, ATL)
Fly(P3, JFK, ATL)
Fly(P2, JFK, ATL)
Load(C1, P3, ATL)
Fly(P3, ATL, SFO)
Fly(P1, ATL, SFO)
Fly(P2, ATL, SFO)
Fly(P3, SFO, ATL)
Fly(P2, SFO, JFK)
Fly(P3, ATL, JFK)
Fly(P1, SFO, ATL)
Fly(P2, JFK, SFO)
Fly(P1, ATL, JFK)
Fly(P2, SFO, ATL)
Unload(C1, P3, JFK)
Fly(P2, ATL, JFK)
Fly(P3, JFK, ATL)
Fly(P1, JFK, ATL)
Fly(P2, JFK, ATL)
Fly(P3, ATL, SFO)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Fly(P3, SFO, ATL)
Load(C3, P1, SFO)
Fly(P3, ATL, JFK)
Fly(P2, SFO, ATL)
Fly(P1, SFO, ATL)
Fly(P3, JFK, ATL)
Fly(P2, ATL, JFK)
Fly(P3, ATL, SFO)
Fly(P1, ATL, SFO)
Load(C2, P2, JFK)
Fly(P3, SFO, ATL)
Fly(P1, SFO, JFK)
Fly(P3, ATL, JFK)
Fly(P2, JFK, ATL)
Fly(P1, JFK, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Unload(C3, P1, SFO)
Fly(P2, SFO, ATL)
Fly(P1, SFO, ATL)
Fly(P3, JFK, ATL)
Fly(P2, ATL, SFO)
Fly(P3, ATL, SFO)
Fly(P1, ATL, JFK)
Fly(P2, SFO, ATL)
Unload(C2, P2, ATL)
Fly(P2, ATL, SFO)
Fly(P3, SFO, ATL)
Fly(P2, SFO, JFK)
Fly(P3, ATL, JFK)
Fly(P1, JFK, ATL)
Fly(P3, JFK, SFO)
Fly(P1, ATL, SFO)
Load(C3, P3, SFO)
Fly(P3, SFO, ATL)
Fly(P1, SFO, ATL)
Fly(P3, ATL, JFK)
Fly(P1, ATL, JFK)
Fly(P2, JFK, ATL)
Fly(P3, JFK, ATL)
Load(C2, P3, ATL)
Fly(P3, ATL, SFO)
Fly(P2, ATL, SFO)
Fly(P3, SFO, JFK)
Fly(P2, SFO, JFK)
Fly(P1, JFK, ATL)
Fly(P2, JFK, ATL)
Fly(P1, ATL, SFO)
Load(C1, P3, JFK)
Fly(P2, ATL, SFO)
Fly(P1, SFO, ATL)
Fly(P3, JFK, ATL)
Fly(P1, ATL, JFK)
Fly(P3, ATL, SFO)
Fly(P2, SFO, ATL)
Fly(P1, JFK, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, SFO)
Fly(P3, SFO, ATL)
Unload(C2, P3, ATL)
Fly(P3, ATL, SFO)
Fly(P1, SFO, ATL)
Fly(P2, JFK, ATL)
Fly(P1, ATL, JFK)
Fly(P2, ATL, SFO)
Fly(P3, SFO, JFK)
Fly(P1, JFK, ATL)
Unload(C3, P3, JFK)
Fly(P1, ATL, SFO)
Fly(P2, SFO, ATL)
Fly(P1, SFO, JFK)
Fly(P2, ATL, JFK)
Fly(P3, JFK, ATL)
Fly(P1, JFK, ATL)
Fly(P3, ATL, SFO)
Fly(P1, ATL, SFO)
Unload(C1, P3, SFO)
Fly(P3, SFO, ATL)
Fly(P1, SFO, ATL)
Fly(P3, ATL, JFK)
Fly(P1, ATL, JFK)
Fly(P2, JFK, ATL)
Fly(P3, JFK, ATL)
Fly(P2, ATL, SFO)
Fly(P3, ATL, SFO)
Load(C3, P1, JFK)
Fly(P2, SFO, ATL)
Fly(P1, JFK, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, SFO)
Fly(P3, SFO, ATL)
Fly(P1, SFO, JFK)
Load(C2, P3, ATL)
Fly(P3, ATL, SFO)
Fly(P2, JFK, ATL)
Fly(P3, SFO, JFK)
Fly(P2, ATL, SFO)
Fly(P1, JFK, ATL)
Fly(P3, JFK, ATL)
Fly(P1, ATL, SFO)
Fly(P3, ATL, SFO)
Unload(C3, P1, SFO)
Fly(P2, SFO, ATL)
Unload(C2, P3, SFO)
Load(C3, P1, SFO)
Fly(P2, ATL, JFK)
Fly(P3, SFO, ATL)
Fly(P2, JFK, SFO)
Fly(P3, ATL, JFK)
Fly(P1, SFO, ATL)
Fly(P3, JFK, SFO)
Fly(P1, ATL, JFK)
Load(C2, P2, SFO)
Fly(P3, SFO, ATL)
Fly(P2, SFO, ATL)
Fly(P3, ATL, JFK)
Fly(P2, ATL, JFK)
Fly(P1, JFK, ATL)
Fly(P3, JFK, ATL)
Unload(C3, P1, ATL)
Fly(P1, ATL, JFK)
Fly(P3, ATL, SFO)
Fly(P2, JFK, ATL)
Fly(P1, JFK, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Fly(P3, SFO, ATL)
Fly(P2, SFO, ATL)
Fly(P3, ATL, JFK)
Fly(P2, ATL, JFK)
Load(C1, P1, SFO)
Fly(P1, SFO, ATL)
Fly(P3, JFK, ATL)
Fly(P1, ATL, JFK)
Fly(P2, JFK, ATL)
Fly(P3, ATL, SFO)
Fly(P2, ATL, SFO)
Fly(P3, SFO, JFK)
Unload(C2, P2, SFO)
Fly(P2, SFO, ATL)
Fly(P3, JFK, ATL)
Fly(P1, JFK, ATL)
Fly(P3, ATL, SFO)
Fly(P2, ATL, SFO)
Unload(C1, P1, ATL)
Fly(P1, ATL, SFO)
Fly(P3, SFO, ATL)
Fly(P2, SFO, ATL)
Fly(P3, ATL, JFK)
Fly(P2, ATL, JFK)
Fly(P1, SFO, ATL)
Fly(P3, JFK, ATL)
Fly(P1, ATL, JFK)
Fly(P3, ATL, SFO)
Fly(P2, JFK, ATL)
Load(C3, P2, ATL)
Fly(P2, ATL, SFO)
Fly(P3, SFO, ATL)
Fly(P2, SFO, JFK)
Fly(P3, ATL, JFK)
Fly(P1, JFK, ATL)
Fly(P2, JFK, ATL)
Fly(P3, JFK, ATL)
Load(C1, P3, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Fly(P3, ATL, JFK)
Fly(P2, SFO, ATL)
Fly(P1, SFO, JFK)
Fly(P2, ATL, JFK)
Fly(P1, JFK, ATL)
Fly(P3, JFK, SFO)
Fly(P1, ATL, SFO)
Unload(C3, P2, JFK)
Fly(P3, SFO, ATL)
Fly(P1, SFO, ATL)
Fly(P2, JFK, ATL)
Fly(P3, ATL, JFK)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Unload(C1, P3, JFK)
Fly(P2, SFO, ATL)
Fly(P1, SFO, JFK)
Fly(P2, ATL, JFK)
Fly(P3, JFK, ATL)
Fly(P1, JFK, ATL)
Fly(P3, ATL, SFO)
Fly(P1, ATL, SFO)
Load(C3, P2, JFK)
Fly(P3, SFO, ATL)
Fly(P2, JFK, ATL)
Fly(P1, SFO, ATL)
Fly(P2, ATL, SFO)
Fly(P3, ATL, SFO)
Fly(P1, ATL, JFK)
Fly(P3, SFO, JFK)
Unload(C3, P2, SFO)


### Solving Air Cargo Problem 2 using uniform_cost_search...

| Expansions |  Goal Tests |  New Nodes | Plan Length | Time |
| ---------- | ----------- | ---------- | ----------- | ---- |
|   4780     |   4782      |  43381     |  9          | 12.28935 |

Plan length: 9  Time elapsed in seconds: 12.289354056999969
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Load(C3, P3, ATL)
Fly(P1, SFO, JFK)
Fly(P2, JFK, SFO)
Fly(P3, ATL, SFO)
Unload(C1, P1, JFK)
Unload(C2, P2, SFO)
Unload(C3, P3, SFO)

## Problem 3

### Solving Air Cargo Problem 3 using breadth_first_search...

| Expansions |  Goal Tests |  New Nodes | Plan Length | Time |
| ---------- | ----------- | ---------- | ----------- | ---- |
|  13489     |  17029      |  119420    |  12         | 90.58743 |

Plan length: 12  Time elapsed in seconds: 90.58743127700006
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P2, JFK, SFO)
Unload(C2, P2, SFO)
Fly(P1, SFO, ATL)
Load(C3, P1, ATL)
Fly(P1, ATL, ORD)
Load(C4, P1, ORD)
Fly(P1, ORD, JFK)
Unload(C1, P1, JFK)
Unload(C3, P1, JFK)
Unload(C4, P1, JFK)


### Solving Air Cargo Problem 3 using depth_first_graph_search...

| Expansions |  Goal Tests |  New Nodes | Plan Length | Time |
| ---------- | ----------- | ---------- | ----------- | ---- |
|   422      |   423       |  3476      |  406        | 1.74092 |

Plan length: 406  Time elapsed in seconds: 1.740921733999926
Fly(P1, SFO, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ORD, ATL)
Fly(P1, ATL, JFK)
Fly(P2, ATL, SFO)
Load(C2, P1, JFK)
Fly(P2, SFO, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, SFO)
Unload(C2, P1, SFO)
Fly(P1, SFO, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ORD, ATL)
Fly(P1, ATL, JFK)
Fly(P2, ATL, SFO)
Load(C2, P2, SFO)
Fly(P2, SFO, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Load(C3, P1, ATL)
Fly(P1, ATL, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, SFO)
Fly(P2, ORD, ATL)
Fly(P1, SFO, JFK)
Fly(P2, ATL, SFO)
Unload(C3, P1, JFK)
Fly(P2, SFO, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, SFO)
Unload(C2, P2, JFK)
Fly(P1, SFO, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ORD, ATL)
Fly(P1, ATL, JFK)
Fly(P2, ATL, SFO)
Load(C3, P1, JFK)
Fly(P2, SFO, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, SFO)
Fly(P2, ATL, JFK)
Unload(C3, P1, SFO)
Fly(P1, SFO, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ORD, ATL)
Fly(P1, ATL, JFK)
Fly(P2, ATL, SFO)
Load(C3, P2, SFO)
Fly(P2, SFO, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, SFO)
Load(C1, P1, SFO)
Fly(P2, ATL, ORD)
Fly(P1, SFO, ORD)
Fly(P2, ORD, SFO)
Fly(P1, ORD, ATL)
Fly(P2, SFO, JFK)
Fly(P1, ATL, JFK)
Unload(C3, P2, JFK)
Fly(P2, JFK, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, SFO)
Unload(C1, P1, ATL)
Fly(P1, ATL, ORD)
Fly(P2, SFO, ORD)
Fly(P1, ORD, SFO)
Fly(P2, ORD, ATL)
Fly(P1, SFO, JFK)
Fly(P2, ATL, JFK)
Load(C3, P2, JFK)
Fly(P2, JFK, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Unload(C3, P2, ATL)
Fly(P2, ATL, ORD)
Fly(P1, ATL, ORD)
Fly(P2, ORD, SFO)
Fly(P1, ORD, SFO)
Fly(P2, SFO, JFK)
Fly(P1, SFO, JFK)
Load(C2, P2, JFK)
Fly(P2, JFK, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Unload(C2, P2, SFO)
Fly(P2, SFO, ORD)
Fly(P1, SFO, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Load(C3, P1, ATL)
Fly(P1, ATL, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, SFO)
Fly(P2, ORD, ATL)
Fly(P1, SFO, JFK)
Fly(P2, ATL, SFO)
Unload(C3, P1, JFK)
Fly(P2, SFO, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, SFO)
Load(C3, P2, JFK)
Fly(P1, SFO, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ORD, SFO)
Fly(P1, ATL, JFK)
Fly(P2, SFO, ATL)
Load(C1, P2, ATL)
Fly(P2, ATL, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, SFO)
Fly(P1, ORD, ATL)
Fly(P2, SFO, JFK)
Fly(P1, ATL, SFO)
Unload(C3, P2, JFK)
Fly(P1, SFO, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ORD, SFO)
Fly(P1, ATL, JFK)
Load(C3, P1, JFK)
Fly(P2, SFO, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, SFO)
Unload(C3, P1, SFO)
Fly(P1, SFO, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ORD, ATL)
Fly(P1, ATL, JFK)
Fly(P2, ATL, SFO)
Unload(C1, P2, SFO)
Fly(P2, SFO, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, SFO)
Load(C3, P1, SFO)
Fly(P1, SFO, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, JFK)
Fly(P2, ORD, ATL)
Unload(C3, P1, JFK)
Fly(P2, ATL, JFK)
Fly(P1, JFK, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Load(C4, P2, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ATL, ORD)
Fly(P2, ATL, SFO)
Fly(P1, ORD, SFO)
Fly(P2, SFO, JFK)
Fly(P1, SFO, JFK)
Unload(C4, P2, JFK)
Fly(P2, JFK, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Load(C2, P2, SFO)
Fly(P2, SFO, ORD)
Fly(P1, SFO, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, JFK)
Unload(C2, P2, JFK)
Fly(P2, JFK, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Load(C1, P2, SFO)
Fly(P2, SFO, ORD)
Fly(P1, SFO, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, JFK)
Unload(C1, P2, JFK)
Fly(P2, JFK, ORD)
Load(C4, P1, JFK)
Fly(P2, ORD, ATL)
Fly(P1, JFK, ORD)
Fly(P2, ATL, SFO)
Fly(P1, ORD, ATL)
Fly(P2, SFO, JFK)
Fly(P1, ATL, SFO)
Unload(C4, P1, SFO)
Fly(P1, SFO, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ORD, ATL)
Fly(P1, ATL, JFK)
Fly(P2, ATL, SFO)
Load(C4, P2, SFO)
Fly(P2, SFO, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, SFO)
Load(C3, P2, JFK)
Fly(P1, SFO, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ORD, ATL)
Fly(P1, ATL, JFK)
Fly(P2, ATL, SFO)
Unload(C4, P2, SFO)
Fly(P2, SFO, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Load(C2, P2, JFK)
Fly(P1, ATL, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, SFO)
Fly(P2, ORD, ATL)
Fly(P1, SFO, JFK)
Fly(P2, ATL, SFO)
Unload(C3, P2, SFO)
Fly(P2, SFO, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, SFO)
Unload(C2, P2, JFK)
Fly(P1, SFO, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ORD, ATL)
Fly(P1, ATL, JFK)
Load(C2, P1, JFK)
Fly(P2, ATL, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, SFO)
Fly(P1, ORD, ATL)
Fly(P2, SFO, JFK)
Fly(P1, ATL, SFO)
Unload(C2, P1, SFO)
Fly(P1, SFO, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ORD, ATL)
Fly(P1, ATL, JFK)
Load(C1, P1, JFK)
Fly(P2, ATL, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, SFO)
Fly(P1, ORD, ATL)
Fly(P2, SFO, JFK)
Fly(P1, ATL, SFO)
Unload(C1, P1, SFO)
Fly(P1, SFO, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ORD, ATL)
Fly(P1, ATL, JFK)
Fly(P2, ATL, SFO)
Load(C4, P2, SFO)
Fly(P2, SFO, ATL)
Fly(P1, JFK, ORD)
Fly(P2, ATL, JFK)
Fly(P1, ORD, ATL)
Fly(P2, JFK, ORD)
Fly(P1, ATL, SFO)
Load(C3, P1, SFO)
Fly(P2, ORD, ATL)
Fly(P1, SFO, ORD)
Fly(P2, ATL, SFO)
Fly(P1, ORD, ATL)
Fly(P2, SFO, JFK)
Unload(C4, P2, JFK)
Fly(P1, ATL, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, SFO)
Fly(P2, ORD, ATL)
Fly(P1, SFO, JFK)
Fly(P2, ATL, SFO)
Load(C4, P1, JFK)
Fly(P2, SFO, ORD)
Fly(P1, JFK, ATL)
Fly(P2, ORD, ATL)
Fly(P1, ATL, ORD)
Unload(C3, P1, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ATL, ORD)
Fly(P1, ATL, SFO)
Fly(P2, ORD, SFO)
Fly(P1, SFO, JFK)
Fly(P2, SFO, JFK)
Unload(C4, P1, JFK)
Fly(P2, JFK, ORD)
Fly(P1, JFK, ATL)
Fly(P2, ORD, ATL)
Fly(P1, ATL, ORD)
Fly(P2, ATL, SFO)
Fly(P1, ORD, SFO)
Load(C2, P2, SFO)
Fly(P2, SFO, ORD)
Fly(P1, SFO, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, JFK)
Unload(C2, P2, JFK)
Fly(P2, JFK, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Load(C1, P2, SFO)
Fly(P2, SFO, ORD)
Fly(P1, SFO, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, JFK)
Unload(C1, P2, JFK)
Fly(P2, JFK, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Load(C3, P1, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ATL, ORD)
Fly(P1, ATL, SFO)
Fly(P2, ORD, SFO)
Fly(P1, SFO, JFK)
Load(C4, P1, JFK)
Fly(P2, SFO, JFK)
Fly(P1, JFK, ORD)
Fly(P2, JFK, ORD)
Fly(P1, ORD, ATL)
Fly(P2, ORD, ATL)
Fly(P1, ATL, SFO)
Unload(C4, P1, SFO)
Fly(P2, ATL, ORD)
Fly(P1, SFO, ORD)
Fly(P2, ORD, SFO)
Fly(P1, ORD, ATL)
Fly(P2, SFO, JFK)
Fly(P1, ATL, JFK)
Load(C2, P2, JFK)
Fly(P2, JFK, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Unload(C2, P2, SFO)
Fly(P2, SFO, ORD)
Fly(P1, SFO, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, JFK)
Unload(C3, P1, JFK)
Fly(P2, JFK, ORD)
Fly(P1, JFK, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, SFO)
Fly(P1, ATL, SFO)
Load(C4, P2, SFO)
Fly(P2, SFO, ORD)
Fly(P1, SFO, ORD)
Fly(P2, ORD, ATL)
Fly(P1, ORD, ATL)
Fly(P2, ATL, JFK)
Fly(P1, ATL, JFK)
Unload(C4, P2, JFK)


### Solving Air Cargo Problem 3 using uniform_cost_search...

| Expansions |  Goal Tests |  New Nodes | Plan Length | Time |
| ---------- | ----------- | ---------- | ----------- | ---- |
|  18236     |  18238      | 159726     | 12          | 52.84357 |

Plan length: 12  Time elapsed in seconds: 52.843569731
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P1, SFO, ATL)
Load(C3, P1, ATL)
Fly(P1, ATL, ORD)
Load(C4, P1, ORD)
Fly(P2, JFK, SFO)
Fly(P1, ORD, JFK)
Unload(C1, P1, JFK)
Unload(C2, P2, SFO)
Unload(C3, P1, JFK)
Unload(C4, P1, JFK)

