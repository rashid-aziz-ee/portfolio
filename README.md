# Grid & Pipeline Research Triager (GPR-Agent)

> **Autonomous AI Agent for Log Telemetry Ingestion, Anomaly Diagnostics, and Daily Brief Generation.**

## Overview
GPR-Agent is a specialized personal AI agent designed to ingest raw industrial telemetry logs and search performance metrics (`.csv`, `.log`), analyze position drops and data variance, and automatically generate structured, human-readable Markdown diagnostic briefs.

---

## 🏗 System Architecture & Data Flow
[Raw Log Files / CSV Data]
│
▼
┌─────────────────────────────────────────┐
│ GPR-Agent (Claude Engine + MCP Connectors)│
├─────────────────────────────────────────┤
│ 1. Read Logs (mcp_filesystem_read)     │
│ 2. Shape Verification & Null Check      │
│ 3. Python Interpreter Exception Analysis│
└─────────────────────────────────────────┘
│
▼
[Structured Markdown Briefs (outputs/daily_brief.md)]
---

## ⚡ Quick Start Setup Guide

A stranger should be able to set up and run GPR-Agent in under 3 minutes:

1. **Clone the Repository:**
```bash
git clone [https://github.com/rashid-aziz-ee/portfolio.git](https://github.com/rashid-aziz-ee/portfolio.git)
cd portfolio
```
