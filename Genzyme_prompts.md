# Genzyme prompts

To get started, attach the files `MC_Assistant.md`, `Genzyme_brief.md` and `Genzyme Template.xlsx` to the chat. 

Then, copy each prompt (**the text inside the gray boxes**) and paste it to the assistant.

```
Follow the instructions in the attached file MC_Assistant.md for this whole conversation. The other attached files describe the case: Genzyme_brief.md is the case brief and Genzyme model.xlsx is the Excel file.
```

## Uncertainties (Assumptions)

These are the hypotheses for the eight uncertainties (Assumptions). You can send them all in one message:

```
FDA approval is Yes-No with probability of Yes 65%.
Launch delay is Discrete: 0 with probability 70%, 1 with probability 20%, 2 with probability 10%.
Life of drug is Triangular(10, 13, 20).
Peak market share is Triangular(20%, 50%, 59%).
Compliance is Triangular(75%, 92%, 94%).
Price per patient is Triangular(600, 1100, 1300).
Gross profit (%) is Normal with mean 70% and standard deviation 5%.
Marketing multiplier is Triangular(0.87, 0.93, 1.2).
```

```
Run the simulation.
```

## Questions

```
What is the probability that Genzyme NPV is negative?
```

```
Show the distribution of JV value (NPV of the JV).
```

```
What is the probability that JV value is negative?
```

## Which inputs matter most? (tornado chart: how much NPV changes when an input goes from its lowest to highest value, with all other inputs at their base values)

```
Show the tornado chart.
```

## Other things you can ask

- `Show the percentiles.`
- `Plot the cumulative distribution.`
- `Delete the mean from the graph.`
- `Run 5,000 scenarios (or other number).`
- `Set Genzyme price for JV to 20000 and run the simulation again.` (the amount Genzyme pays, in $000)
- `Set Genzyme share of JV to 0.8 and run the simulation again.`
- `Fix the random seed.` (to get the same results each time. This is a technical issue: disregard it unless you have a strong interest in it).