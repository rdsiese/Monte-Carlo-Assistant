# SkyWest Airlines prompts

To get started, attach the files `MC_Assistant.md` and `SkyWest_brief.md` to the chat.

Then, copy each prompt (**the text inside the gray boxes**) and paste it to the assistant.

```
Follow the instructions in the attached file MC_Assistant.md for this whole conversation. The other attached file, SkyWest_brief.md, describes the case.
```

## Uncertainty (Assumption)

```
Show up is Binomial with probability 0.9 and number of trials equal to Tickets sold.
```

## How many tickets to sell? (the decision variable)

```
Run the simulation for Tickets sold = 19, 20, 21, 22 and 23.
```

You will get a graph for each number of tickets and a table that compares them. 

## Probability of empty seats

```
Set Tickets sold to 21.
```

```
What is the probability that there are empty seats?
```

(You can ask the same for other numbers of tickets: set the new value and ask again.)

## Other things you can ask

- `Show the percentiles.`
- `Plot the cumulative distribution.`
- `Delete the mean from the graph.`
- `Run 5,000 scenarios (or other number).`
- `Run the simulation for other number of Tickets sold.`
- `Fix the random seed.` (to get the same results each time. This is a technical issue: disregard it unless you have a strong interest in it).
