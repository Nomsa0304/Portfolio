# AI Job Market Explorer

**Stack:** R, Shiny, Plotly, ggplot2

## The Problem

Job market data is only useful if you can slice it the way your own question needs. Built as a self-service tool: pick a job title, experience level, company, or skill, and every chart recomputes against just that slice.

## What It Does

- **Salary & Job Experience Analytics** — salary trend by experience level, salary comparison by job title, job count by experience, min/avg/max salary range
- **Job Demand** — bar chart of job title frequency
- **Skills Analysis** — word cloud from the skills field
- **Job Explorer** — full filterable, searchable data table

All charts key off one reactive filtered dataset (`df_filtered()`), so every view stays consistent no matter which filters are combined.

## Skills Demonstrated

R Shiny · Reactive programming · Plotly · ggplot2 · Interactive dashboard design
