# MarketMaster: Dual-Agent Financial Research Assistant

A dual-agent AI system designed to reduce hallucinations in financial analysis by separating data collection from analysis.
## Problem Statement
Traditional single-agent LLM systems often suffer from hallucinations , generating plausible but incorrect information. In financial research, this can lead to:

- Fabricated stock prices
- Invented company developments
- Unreliable market analysis

## Solution: Dual-Agent Architecture
- MarketMaster employs two specialized AI agents:

### Researcher Agent (Internet-enabled)
- Gathers raw data from Google Search and NewsAPI
- Collects latest news, stock prices, and market information
- No analysis or interpretation

### Analyst Agent (No internet access)
- Receives ONLY data from Researcher
- Cannot fabricate information (no external access)
- Produces structured analysis reports

By isolating the analysis phase from data collection, the system significantly reduces hallucination risk.

## Results:
Based on a query run
### Facts and Numbers
- Dual-Agent:  36.8 
- Single-Agent: 13.8
- Improvement: +166.7%

### Reliability Score:
- Dual-Agent:   32.0/100
- Single-Agent: 8.0/100
- Improvement: +300%

### However, there arises a fluctuation in the number of uncertain_words for the dual and the single agent model based on the fact that the data is inherently uncertain.
