# Chemical Fusion (C) prompts

To get started, attach the files `MC_Assistant.md` and `ChemicalFusionC_brief.md` to the chat.

Then, copy each prompt (**the text inside the gray boxes**) and paste it to the assistant.

```
Follow the instructions in the attached file MC_Assistant.md for this whole conversation. The other attached file, ChemicalFusionC_brief.md, describes the case.
```

## Uncertainties (Assumptions)

```
Use a Discrete distribution for IQI demand.
```

```
0 with probability 0.15, 1000 with probability 0.15, 2000 with probability 0.20, 3000 with probability 0.30, 4000 with probability 0.20.
```

```
Artisans demand is Uniform(0, 2000).
```

(If you prefer to work in whole liters, you can ask for `Artisans demand is Discrete Uniform(0, 2000).` Because there are so many possible values, the results are almost identical.)

## How much to produce? (the decision variable)

```
Run the simulation for Production = 3000, 3500, 4000, 4500 and 5000.
```

You will get a graph for each production level and a table that compares them.

## Risk of a loss

```
Set Production to 3500.
```

```
What is the probability that the profit is negative?
```

(You can ask the same for other production levels: set the new value and ask again.)

## Other things you can ask (refine search, check stability of simulation results)

```
Run the simulation for Production = 3300, 3400, 3500, 3600 and 3700.
```

```
For Production = 3500, run the simulation with 10, 100, 1000, 5000, 10000, 15000, 25000 and 50000 scenarios.
```

```
For Production = 3500, run the simulation 8 times with 10000 scenarios each.
```

- `Show the percentiles.`
- `Plot the cumulative distribution.`
- `Delete the mean from the graph.`
- `Run 5,000 scenarios (or other number).`
- `Fix the random seed.` (to get the same results each time. This is a technical issue: disregard it unless you have a strong interest in it).