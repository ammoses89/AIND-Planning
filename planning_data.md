# AIND PLANNING DATA Metrics



### Non-heuristic planning

1. `air_cargo_p1` 

* bread-first-search

``` xpansions   Goal Tests   New Nodes
Expansions   Goal Tests   New Nodes
    43          56         180

Plan length: 6  Time elapsed in seconds: 0.0562283750041388
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P2, JFK, SFO)
Unload(C2, P2, SFO)
Fly(P1, SFO, JFK)
Unload(C1, P1, JFK)
```

* depth_first_graph_search

```
Expansions   Goal Tests   New Nodes
    21          22          84

Plan length: 20  Time elapsed in seconds: 0.02664980699773878
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
```

* uniform_cost_search

```
Expansions   Goal Tests   New Nodes
    55          57         224

Plan length: 6  Time elapsed in seconds: 0.06358329497743398
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P1, SFO, JFK)
Fly(P2, JFK, SFO)
Unload(C1, P1, JFK)
Unload(C2, P2, SFO)
```

2. `air_cargo_p2` 

* breadth_first_search

```
Expansions   Goal Tests   New Nodes
   3343        4609       30509

Plan length: 9  Time elapsed in seconds: 20.436932634969708
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Load(C3, P3, ATL)
Fly(P2, JFK, SFO)
Unload(C2, P2, SFO)
Fly(P1, SFO, JFK)
Unload(C1, P1, JFK)
Fly(P3, ATL, SFO)
Unload(C3, P3, SFO)
```

* depth_first_graph_search

```
Expansions   Goal Tests   New Nodes
   624         625         5602

Plan length: 619  Time elapsed in seconds: 5.135540232993662
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
```

* uniform_cost_search

```
Expansions   Goal Tests   New Nodes
   4852        4854       44030

Plan length: 9  Time elapsed in seconds: 17.03632665000623
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Load(C3, P3, ATL)
Fly(P1, SFO, JFK)
Fly(P2, JFK, SFO)
Fly(P3, ATL, SFO)
Unload(C3, P3, SFO)
Unload(C2, P2, SFO)
Unload(C1, P1, JFK)
```

3. `air_cargo_p3`

* `breadth_first_search`

```
Expansions   Goal Tests   New Nodes
   325         806         2792

Plan length: 6  Time elapsed in seconds: 2.228607640019618
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P2, JFK, SFO)
Unload(C2, P2, SFO)
Fly(P1, SFO, JFK)
Unload(C1, P1, JFK)
```

* `depth_first_search_graph`

```
Expansions   Goal Tests   New Nodes
   286         287         2365

Plan length: 274  Time elapsed in seconds: 2.036507358017843
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
```

* `uniform_cost_search`

```
Expansions   Goal Tests   New Nodes
   1087        1089        9592

Plan length: 6  Time elapsed in seconds: 5.645319307979662
Load(C1, P1, SFO)
Load(C2, P2, JFK)
Fly(P1, SFO, JFK)
Fly(P2, JFK, SFO)
Unload(C2, P2, SFO)
Unload(C1, P1, JFK)
```
