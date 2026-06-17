# n8n AI Data Visualization Pipeline

Upload 2 CSV files + describe what you want → AI generates HTML report, Google Slides PPT, or Tableau export automatically.

## What it does
- User uploads 2 CSV files and types a prompt
- AI (Google Gemma 4 31B via OpenRouter) analyzes the data
- Generates visualization in chosen format

## Output formats
- **HTML Report** — Chart.js charts in browser
- **PPT** — Real Google Slides presentation with charts
- **Tableau** — data.csv + datasource.tds files

## Setup instructions

### 1. Import workflow
- Open n8n → New Workflow → Import from file
- Select `workflow.json`

### 2. Add credentials
- **OpenRouter API key** → openrouter.ai (free)
- **Google OAuth2** → console.cloud.google.com

### 3. How to use
- Open the Form Trigger URL
- Upload 2 CSV files
- Type your prompt (examples below)

## Prompt examples
| Prompt | Output |
|---|---|
| show me a bar chart of sales | HTML report |
| FORMAT: PPT create a presentation | Google Slides |
| FORMAT: TABLEAU export data | Tableau files |
| show me both HTML and PPT | Both simultaneously |

## Tech stack
- n8n Cloud
- OpenRouter API (Google Gemma 4 31B free)
- Google Slides API
- QuickChart.io (free, no key needed)
