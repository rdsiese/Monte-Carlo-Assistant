# Case brief: Kahrvinger (B)

*Short description of the situation, the problem and the model. Use together with `MC_Assistant.md`.*

## Situation

Kahrvinger AS, a Norwegian company, is evaluating an investment project with an 8-year life. All figures are in thousands of euros. With the base-case values below, the annual cash flow is 196 and the NPV at an 11% discount rate is about 208.

## Problem

Sales and the cost of electronic components are uncertain. Analyze how this uncertainty affects the NPV of the project: its possible range, its average and how likely it is to be negative.

## Forecast

**NPV(11)**: the net present value of the project at an 11% discount rate.

## Inputs and base values

| Input | Base value | Can be uncertain? |
|---|---:|---|
| Sales (revenues, per year) | 2,500 | Yes |
| Electronic components (cost, per year) | 500 | Yes |
| Investment (at the start, year 0) | 800 | No |
| Labor (per year) | 1,500 | No |
| Other materials (per year) | 250 | No |
| Tax rate | 36% | No |
| Discount rate | 11% | No |
| Project life | 8 years | No |

Names: the user may call Sales "revenues", and the electronic components "raw materials" or "costs". Treat these as the same inputs.

## Model

Each year *t* = 1,...,8 the figures are the same (**Sales and Electronic components are drawn once per trial and are the same in all 8 years**):

- Depreciation = Investment / 8 = 100 (linear)
- Gross profit = Sales - Labor - Electronic components - Other materials
- EBT (earnings before taxes) = Gross profit - Depreciation
- Taxes = Tax rate x EBT if EBT is positive; 0 otherwise
- Net profit = EBT - Taxes
- Cash flow = Net profit + Depreciation

NPV(11) = -Investment + sum of Cash flow / (1 + 0.11)^t   &nbsp;&nbsp; (over t = 1,...,8)

Check: with the base values, Gross profit = 250, EBT = 150, Taxes = 54, Net profit = 96, Cash flow = 196, and NPV(11) = 208.6.
