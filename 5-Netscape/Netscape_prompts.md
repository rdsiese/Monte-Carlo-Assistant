# Netscape prompts

To get started, attach the files `MC_Assistant.md`, `Netscape_brief.md` and `Netscape.xlsx` to the chat. 

Then, copy each prompt (**the text inside the gray boxes**) and paste it to the assistant.

```
Follow the instructions in the attached file MC_Assistant.md for this whole conversation. The other attached files describe the case: Netscape_brief.md is the case brief and Netscape.xlsx is the Excel model.
```

## Uncertainties (Assumptions)

These are the hypotheses for the nine uncertainties (Assumptions) considered in the case. You can send them all in one message:

```
Revenue growth rate is Normal with mean 65% and standard deviation 5%.
TV growth rate is Discrete Uniform: the values 1%, 2%, 3%, ..., 10%, each with the same probability.
Cost of sales is Normal with mean 10.44% and standard deviation 1.6%.
R&D expenses are Triangular with minimum 32%, most likely 36.76% and maximum 42%.
Capital expenditures are Uniform between 44% and 46%.
Other operating expenses are Uniform between 79% and 81%.
Depreciation is Uniform between 4.5% and 6.5%.
Risk-free rate is Triangular with minimum 6%, most likely 6.71% and maximum 7.5%.
Market-risk premium is Uniform between 5% and 10%.
```


## Simulate

```
Run the simulation.
```

You get the distribution and statistics of **Total NPV** (in $000) and of **Price/share**.

## The other Forecasts

```
Show the distribution of the other Forecasts: Ratio TV/Total NPV and Max loss.
```

## Was the IPO price justified?


```
What is the probability that Price/share is above 28?
```

## Which inputs matter most? (tornado chart: tornado chart: how much Total NPV changes when an input goes from its lowest to highest value, with all other inputs at their base values)

```
Show the tornado chart.
```

## Do the minor inputs matter?

```
Re-run the simulation using only the first four variables listed in the tornado chart (Revenue growth rate, TV growth rate, R&D and Market-risk premium).
```

Compare the results with the ones you obtained when you first ran the simulation (with the nine uncertain inputs).

## Other things you can ask

- `Show the percentiles.`
- `Plot the cumulative distribution.`
- `Delete the mean from the graph.`
- `Run 5,000 scenarios (or other number).`
- `Fix the random seed.` (to get the same results each time. This is a technical issue: disregard it unless you have a strong interest in it).
