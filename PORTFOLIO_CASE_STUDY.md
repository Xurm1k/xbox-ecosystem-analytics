# Portfolio case study: Xbox Ecosystem Strategy Analysis

## The project

I built an end-to-end analysis to explore how major game launches, Game Pass availability, console sales, and subscriber growth could fit together in a business narrative. The project combines Python data preparation, a dimensional model, Power BI measures, and an executive-facing presentation.

The analysis is framed as a strategy exercise. Its central question is whether launch-window subscription access can support ecosystem growth while hardware sales remain constrained.

## What the project does

- Creates daily console-sales and subscription time series for 2020–2025 with a reproducible Python generator.
- Organizes the analysis around game, date, console-sales, and subscription data.
- Compares Day One Game Pass releases with first-party non-Day-One releases and a third-party control group.
- Uses Power BI and DAX to summarize launch windows, hardware trends, and subscriber trajectories.
- Presents findings and strategic options in a dashboard and executive deck.

## A decision I had to make

The repository's data generator models the time series using chosen baselines, seasonal multipliers, release-window boosts, and random variation. That made it possible to build and demonstrate an end-to-end analytics workflow without claiming access to complete commercial sales or subscriber records.

It also sets a clear boundary on interpretation: the reported lifts and plateaus are outputs of the modeled assumptions. They are useful for showing how a business question can be translated into a data model and dashboard, but they do not establish what Game Pass caused in the real market.

## What I personally contributed

- Framed the business question around the relationship between launch timing, console demand, and subscription growth.
- Structured the project as a repeatable pipeline from generated data through a star-schema model to Power BI reporting.
- Defined comparison groups and analytical windows for the dashboard.
- Developed the strategy narrative and recommendations as hypotheses for further investigation.
- Kept the distinction between modeled outputs and real-world evidence explicit.

I used AI-assisted coding where helpful. My contribution was the analytical framing, data assumptions, modeling choices, review of the outputs, and the way the findings are communicated.

## Limits

The time series are synthetic and encode the patterns the analysis later examines. They cannot validate market-level causal claims, estimate real sales lift, or prove that a particular subscription policy would improve revenue. The strategic recommendations are options to test against reliable external data, not conclusions supported by the generated dataset.

## What I would do next

1. Replace modeled values with documented, appropriately licensed real-world data where available.
2. Add sensitivity analysis for seasonal patterns, launch effects, baselines, and subscriber churn.
3. Separate descriptive trends from causal estimates and document any identification strategy.
4. Add data lineage, source notes, and validation checks to the reporting workflow.
5. Present recommendations with scenario ranges and assumptions rather than point estimates.

## How I would present it in an interview

Start with the business question and explain the end-to-end workflow: Python-generated data, dimensional modeling, DAX, and an executive dashboard. Then be direct that the dataset is synthetic. Use that to explain the difference between demonstrating an analytical method and substantiating a market claim, and describe what real data and validation would be needed for the next stage.

## Resume wording

These bullets describe the analytical work without presenting simulated results as observed market outcomes:

- Built a reproducible Python-to-Power BI analytics workflow to explore modeled relationships among game-release windows, console sales, and subscription growth.
- Designed comparison groups, a dimensional data model, and DAX measures for an executive-facing dashboard.
- Documented synthetic-data assumptions and translated scenario outputs into testable strategy questions.
