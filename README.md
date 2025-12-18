# AI-Powered Shopify Analytics App

## Overview
This project is a mini AI-powered analytics application for Shopify.
It allows users to ask natural language questions related to sales,
inventory, and customers.

## Architecture
- Rails API (API-only) works as backend gateway
- Python FastAPI service acts as AI agent
- ShopifyQL is used for analytics queries (mocked)

## Flow
User Question → Rails API → Python AI Agent → ShopifyQL → Answer

## Tech Stack
- Ruby on Rails (API)
- Python (FastAPI)
- ShopifyQL
- Mock Shopify API

## Sample Request
POST /api/v1/questions
```json
{
  "store_id": "demo-store.myshopify.com",
  "question": "How much inventory should I reorder for next week?"
}
