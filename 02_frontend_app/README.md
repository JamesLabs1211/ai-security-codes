# F5 AI Guardrail Lab – Frontend Installation Guide
This repository contains a Python Flask–based frontend application that connects to a Python-based AI Guardrail Gateway, which then integrates with F5 Calypso AI Guardrail and a backend LLM (e.g., Ollama).

The frontend does not connect to the LLM directly.
All AI traffic is enforced through the Guardrail layer.

## 1. Architecture Overview
```
Browser (UI)
   ↓
Flask Frontend App (/api/chat)
   ↓
Python Guardrail Gateway (/v1/chat/completions)
   ↓
F5 Calypso AI Guardrail (SaaS)
   ↓
LLM Runtime (Ollama /api/chat)
```
