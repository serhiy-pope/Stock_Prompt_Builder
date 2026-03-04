# Stock Prompt Builder

[![Live Demo](https://img.shields.io/badge/demo-live-green)](https://serhiy-pope.github.io/Stock_Prompt_Builder/)
![License](https://img.shields.io/github/license/serhiy-pope/Stock_Prompt_Builder)
![Repo Size](https://img.shields.io/github/repo-size/serhiy-pope/Stock_Prompt_Builder)
![Last Commit](https://img.shields.io/github/last-commit/serhiy-pope/Stock_Prompt_Builder)
![Stars](https://img.shields.io/github/stars/serhiy-pope/Stock_Prompt_Builder?style=social)

![HTML](https://img.shields.io/badge/HTML-5-orange)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)
![CSS](https://img.shields.io/badge/CSS-3-blue)
![AI Prompt Engineering](https://img.shields.io/badge/AI-Prompt%20Engineering-purple)

A **local web tool for generating structured prompts for AI investment analysis agents.**

Stock Prompt Builder helps investors and analysts generate consistent, structured prompts for AI assistants such as:

ChatGPT

Claude

Gemini

any LLM capable of financial analysis

The tool allows users to configure the analysis context, portfolio constraints, and investment system rules, and then automatically generates a high-quality prompt that can be pasted into an AI chat.

The goal is to turn LLMs into structured investment assistants, rather than generic chatbots.

Key Idea

When using AI for investment research, the quality of the prompt determines the quality of the output.

Most prompts are:

inconsistent

missing context

not aligned with portfolio rules

lacking structured reasoning

This tool solves that problem by enforcing a structured prompt protocol.

Instead of asking:

"What do you think about NVDA?"

The generated prompt asks the AI to perform a proper investment analysis pipeline:

Gather current data

Calculate ROP valuation

Compare market vs analyst expectations

Evaluate risk constraints

Produce an Action Card decision

Features
Structured AI prompts

The tool generates prompts that instruct the AI to:

collect financial data

analyze valuation

evaluate portfolio constraints

run scenario analysis

output a structured decision card

Multiple analysis levels

Three levels of analysis depth:

Level	Purpose
Lite	quick idea validation
Standard	entry / hold decision
Pro	deep position review
Multi-AI support

Prompts are optimized for:

Claude (Project files)

ChatGPT (Projects + Browsing)

Gemini (Gem knowledge base)

Each model receives slightly different instructions for sourcing data.

Investment system integration

The prompt can reference external knowledge files stored in your AI project.

Example files:

02_investor_passport.md
03_investment_constitution.md
04_portfolio_snapshot.md
07_context_card.md
06_company_card.md
08_scenario_map.md

These files allow the AI to operate inside a personal investment framework.

Skill system

The builder automatically enables AI analysis modules such as:

Investor Passport

Constitution / QPTA

Portfolio Snapshot

Context Card

Company Card

Quality Gates (G0–G4)

ROP valuation

Price Power analysis

Scenario Map

Earnings Quality (EUREKA)

Life Cycle valuation

Final Report Card

Idea Triage

Different modules are activated depending on the analysis level.

Portfolio risk constraints

The generated prompt includes user risk parameters such as:

instrument type (Stock / ETF / Auto)

portfolio weight

max drawdown per position

investment horizon

investor role (Investor / Speculator / Saver)

These inputs allow the AI to adjust the analysis to the user’s risk model.

Multilingual prompts

The tool supports:

English

Ukrainian

Russian

Both the interface and generated prompt follow the selected language.

How it works

The app is a single static HTML file.

No backend is required.

Architecture:

HTML
CSS
JavaScript

Core components:

UI layer
Prompt builder logic
Translation system

Prompt generation flow:

User inputs
    ↓
Prompt builder
    ↓
Skill system
    ↓
System prompt block
    ↓
Final AI prompt
Example usage

User inputs:

Ticker: NVDA
Goal: Adding to position
Instrument: Stock
Max drawdown: 15%
Role: Investor
Horizon: 2 years

Generated prompt instructs the AI to:

1. Gather market and analyst expectations
2. Calculate ROP valuation
3. Compare market vs analyst views
4. Evaluate portfolio constraints
5. Produce an Action Card decision
Example output structure

AI output is expected to contain:

ACTION CARD
Market vs Analysts
ROP valuation
Decision logic
Key risks
Triggers
Why this tool exists

LLMs are powerful but lack structured thinking by default.

This builder enforces a repeatable analysis framework so that the AI behaves more like a portfolio analyst.

The result is:

more consistent outputs

less hallucination

clearer decision logic

better risk awareness

Installation

Clone the repository:

git clone https://github.com/YOUR_USERNAME/stock-prompt-builder.git

Open the app:

stock_prompt_builder.html

in any browser.

No build step required.

Project structure
stock-prompt-builder
│
├── stock_prompt_builder.html
├── README.md
└── LICENSE

The entire application is contained in a single HTML file.

Roadmap

Possible future improvements:

Prompt module architecture

Portfolio import

Scenario simulation

earnings calendar integration

macro regime detection

automatic AI prompt execution

License

MIT License