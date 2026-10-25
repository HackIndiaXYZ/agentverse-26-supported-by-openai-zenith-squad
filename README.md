# Autonomous IoT Infrastructure Guardian
**Team:** Zenith Squad
**Hackathon:** AgentVerse' 26 (Supported by OpenAI)

## Problem Statement
Critical infrastructure often suffers from silent sensor failures and delayed leak responses due to manual monitoring bottlenecks. To solve this, our multi-agent telemetry system autonomously monitors IoT sensor streams (like turbidity and TDS). The AI agents actively reason to distinguish between hardware faults and actual anomalies, automatically executing workflows like triggering localized shutoffs and dispatching maintenance alerts without human intervention.

## Architecture
- **Telemetry Agent:** Ingests live data from ESP32 nodes (Turbidity, TDS).
- **Diagnostic Agent:** Uses OpenAI LLMs to reason whether an anomaly is a sensor fault or a physical leak.
- **Action Agent:** Executes automated tool calls to shut off pumps or alert maintenance.

## Setup Instructions
1. Clone the repository.
2. Install dependencies: pip install -r requirements.txt
3. Copy .env.example to .env and add your OPENAI_API_KEY.
4. Run the agents: python main.py
