# Kahrvinger (B): your prompts

To get started, attach the files `MC_Assistant.md` and `KahrvingerB_case_brief.md` to the chat.

Then, copy each prompt (**the text inside the gray boxes**) and paste it to the assistant.

```
Follow the instructions in the attached file MC_Assistant.md for this whole conversation. The other attached file, KahrvingerB_case_brief.md, describes the case.
```


## Part (b): uniform distributions

```
Sales is Uniform(2300, 2700). Electronic components is Uniform(450, 550).
```

```
Run the simulation.
```

## Part (c): custom distributions from quantiles

The case does not give a lower limit (0%) or an upper limit (100%) for either input. The first is a value below which the input cannot realistically fall; the latter is an upper limit, beyond which the input cannot realistically go. You have to choose them with common sense. 

```
Use a Continuous Custom distribution for Sales.
```

```
Q0.01 = 2350, Q0.25 = 2450, Q0.5 = 2500, Q0.75 = 2550, Q0.99 = 2650. Lower limit: ... Upper limit: ...
```

```
Use a Continuous Custom distribution for Electronic components.
```

```
Q0.01 = 410, Q0.25 = 460, Q0.5 = 500, Q0.75 = 510, Q0.99 = 540. Lower limit: ... Upper limit: ...
```

```
Run the simulation.
```

## Probability questions

After running the simulation (in any of the parts) you can ask:

```
What is the probability that the NPV is negative?
```

```
What is the probability that the NPV is between 0 and 500?
```

## Other things you can ask

- `Show the percentiles.`
- `Plot the cumulative distribution.`
- `Delete the mean from the graph.`
- `Run 5,000 scenarios (or other number).`
- `Fix the random seed.` (to get the same results each time. This is a technical issue: disregard it unless you have a strong interest in it). 
