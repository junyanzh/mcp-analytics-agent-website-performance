# MCP Analytics Agent for Website Performance

An intelligent analytics assistant that processes natural language queries to retrieve and analyze website data through Google Analytics, Search Console, and PageSpeed APIs.

## Overview

This project implements a multi-layer agent system using Model-Controlled Proxy (MCP) architecture to create an interactive analytics assistant. The system allows users to ask questions about website analytics in natural language and receives formatted, insightful responses.

![Agent Workflow Process](Agent%20Workflow%20Process.png)

## Features

- **Natural Language Interface**: Ask analytics questions in plain English
- **Multi-API Integration**: Connects to Google Analytics 4, Search Console, and PageSpeed Insights
- **Two-Layer Agent Architecture**:
  - Orchestrator Agent: Analyzes intent and selects appropriate tools
  - Executor Agent: Executes API calls and collects results
- **Intelligent Response Generation**: Formats technical data into user-friendly insights
- **Interactive Jupyter Interface**: Explore analytics through conversational interaction

## System Architecture

![System Architecture](System%20Architecture.png)

The system consists of the following components:

1. **Core MCP System**: Handles tool definitions and API connections
2. **Agent System**: Processes queries and generates responses
3. **External APIs**: Retrieves data from Google services

## Query Processing Flow

![Query Processing Flow](Query%20Processing%20Flow.png)

When a user asks a question:
1. The **Orchestrator Agent** analyzes the query and selects the appropriate tools
2. Function calls are generated with the necessary parameters
3. The **Executor Agent** makes the API calls and retrieves data
4. The **Response Generator** creates a user-friendly summary

## Setup and Usage

### Prerequisites
- Python 3.8+
- Google Cloud Project with API access
- Service account with appropriate permissions

### Running the Application
```bash
# Launch the Jupyter notebook
jupyter notebook analytics_assistant.ipynb
