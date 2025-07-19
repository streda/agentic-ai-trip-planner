# Agent AI Trip Planner

An AI-powered trip planning assistant that designs customized travel itineraries for the fictional city of AgentsVille.

This project uses advanced prompting techniques, chain-of-thought reasoning, and tool-assisted planning to build and refine personalized travel schedules. It demonstrates how large language models (LLMs) can interact with tools and reason step-by-step using the ReAct pattern (THOUGHT → ACTION → OBSERVATION).

---

## Features

- Expert Itinerary Generation based on travel preferences
- Tool-using ReAct Agent for iterative plan refinement
- Weather-aware activity scheduling
- Budget evaluation and recalculation
- Day-by-day itinerary planning
- Built on [Pydantic](https://docs.pydantic.dev), [OpenAI](https://openai.com/), and Jupyter Notebook

---

---

## Sample Output

✅ Sample itinerary evaluation:

✅ The agent detects this and swaps the activity with a weather-compatible one using the `get_activities_by_date_tool`.

---

## How It Works

This project involves two core AI components:

1. **Expert Planner**  
   Uses user preferences (like interests, budget, dates) to create an initial itinerary using a Pydantic model.

2. **Itinerary Revision Agent**  
   Applies the ReAct pattern (reasoning + tool use) to revise the plan, call APIs, re-evaluate it, and produce a final itinerary.

---

## Disclaimer

> This project is based on coursework from [Udacity Generative AI Nanodegree](https://www.udacity.com/course/generative-ai--nd936), and successfully implemented by me as part of the coursework requirement.


---

## Requirements

- Python 3.10+
- OpenAI API client
- Pydantic
- Jupyter Notebook

---

## How to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/streda/agent-ai-trip-planner.git
   cd agent-ai-trip-planner