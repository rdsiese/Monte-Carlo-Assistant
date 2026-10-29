# MC Assistant

Monte Carlo simulation with an AI assistant. Developed by Rafael Santiago (IESE Business School) to help you analyze the following cases: Kahrvinger B, Chemical Fusion C, SkyWest Airlines, Genzyme-Geltex and Netscape. 

## How it works

For each case you need: 

| File | What to do | What it is |
|---|---|---|
| `MC_Assistant.md` | Attach to the chat (same for all cases) | General instructions that make the assistant carry out the simulations. |
| `[name]_case_brief.md` | Attach to the chat (one for each case) | Description of the case and the model. |
| | | |

Genzyme and Netscape also need their Excel file (`Genzyme Template.xlsx`, `Netscape.xlsx`) to be attached to the chat. 

NOTE: The files `[name]_case_brief.md` contain the streamlined facts from each case that are needed to run the simulation, so you don’t need to attach the whole case. This allows you to follow IESE guidelines regarding case copyright (and it’s faster). 


## Quick start

1. Open a new chat in an AI assistant that accepts file attachments and can run code (Claude, ChatGPT, Gemini).
2. Attach `MC_Assistant.md`, the corresponding case brief `[name]_case_brief.md` and, if the case has one, the Excel file.
3. From the corresponding prompts file (`[name]_user_prompts.md`), copy and paste the starting message from **Before you start**.
4. Paste the remaining prompts one at a time, in order.

Use a new chat for each case.

## Cases

| # | Case | Forecast | Folder |
|---|---|---|---|
| 1 | Kahrvinger B | NPV | `1_KahrvingerB/` |
| 2 | Chemical Fusion C | Profit (decision variable: production) | `2_Chemical_FusionC/` |
| 3 | SkyWest Airlines | Profit (decision variable: tickets sold) | `3_SkyWest_Airlines/` |
| 4 | Genzyme-GelTex | Genzyme NPV | `4_Genzyme/` |
| 5 | Netscape | Total NPV, Price/share | `5_Netscape/` |

## What the assistant can do

- Define Assumptions with standard distributions (Normal, Triangular, Uniform, Lognormal, Exponential, Binomial, Poisson, Discrete Uniform, Yes-No), continuous custom and discrete distributions.
- Run 10,000 scenarios by default (up to 1,000,000) and show the Forecast chart and the Crystal Ball statistics table.
- Answer probability questions with range charts.
- Compare values of a decision variable using the same random draws.
- Draw tornado charts, and re-run with only the most relevant Assumptions.
- Use an Excel model as the source of the formulas, without editing it.

## Notes

- Results vary slightly from run to run because the simulation uses random numbers.
- In class we use Crystal Ball, a trademark of Oracle. This project is not affiliated with Oracle.

