# AI Powered Shopify Analytics App

## Overview
This project is a conceptual design of an AI-powered analytics system for Shopify stores. The goal is to allow store owners to ask business questions in natural language and receive simple, human-readable insights based on store data such as orders, products, and inventory.

This assignment focuses on system design and reasoning rather than a fully working production system.

## Architecture
The system is divided into three main parts:

- Rails API acts as a gateway that receives user questions.
- Python AI service acts as the brain that understands the question and generates insights.
- Shopify is the data source for orders, inventory, and customers.

## Agent Workflow
1. The user sends a natural language question.
2. The AI identifies the intent (sales, inventory, or customers).
3. The system decides what Shopify data is required.
4. A ShopifyQL query is generated.
5. The data is fetched (mocked for this assignment).
6. The result is converted into simple business-friendly language.

## Example Flow
**Question:**  
“How much inventory should I reorder for next week?”

- **Intent:** Inventory forecasting  
- **Data used:** Last 30 days sales  
- **Logic:** Calculate average daily sales and multiply by 7 days  
- **Output:**  
“Based on recent sales trends, you should reorder approximately 70 units to avoid stockouts next week.”

## Tech Stack
- Ruby on Rails (API-only)
- Python (FastAPI/Flask)
- LLM (Mocked)
- ShopifyQL (Conceptual)

## Assumptions & Limitations
- Shopify API integration is mocked.
- OAuth authentication is not fully implemented.
- AI reasoning is simulated.
- The focus is on design clarity rather than production readiness.


