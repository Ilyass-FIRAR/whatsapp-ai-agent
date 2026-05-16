# WhatsApp AI Agent – AI-Powered Order Confirmation System

## Overview

This project is an AI-powered WhatsApp order confirmation system designed for e-commerce businesses using Cash on Delivery (COD).

The system automates the order confirmation process by sending WhatsApp messages to customers, analyzing their responses using AI, and updating the order status automatically.

This project was developed as an academic PFA (Projet de Fin d’Année).

---

## Problem Statement

Many e-commerce businesses in Morocco manually confirm customer orders through phone calls or WhatsApp messages.

This process creates several problems:

- Time-consuming manual confirmation
- High cancellation rates
- Delayed order processing
- Human errors in customer communication
- Difficulty managing large numbers of orders

---

## Proposed Solution

The system automatically:

1. Detects a new order
2. Sends a WhatsApp confirmation message
3. Receives the customer response
4. Uses AI to classify the response
5. Updates the order status automatically

Possible AI decisions:

- confirmed
- cancelled
- needs_more_info

---

## Technical Stack

### Automation & Orchestration
- n8n

### Messaging
- Meta WhatsApp Cloud API

### AI Processing
- Gemini AI / AI Agent

### Database & Storage
- Google Sheets

### E-commerce Source
- Shopify (or simulated orders)

### APIs & Webhooks
- REST APIs
- Webhooks

---

## System Architecture

```text
Shopify Orders
       ↓
Google Sheets
       ↓
n8n Workflow Trigger
       ↓
WhatsApp Template Message
       ↓
Customer Reply
       ↓
AI Agent Analysis
       ↓
Order Status Update
```

---

## Workflow Explanation

### 1. New Order Detection
A new order is inserted into Google Sheets.

### 2. Workflow Trigger
n8n detects the new order automatically.

### 3. WhatsApp Message Sending
The system sends a WhatsApp template message to the customer.

### 4. Customer Response
The customer confirms, cancels, or asks for more information.

### 5. AI Classification
The AI agent analyzes the message intent.

### 6. Automatic Update
The order status is updated inside Google Sheets.

---

## Project Features

- Automated order confirmation
- AI-powered customer response analysis
- WhatsApp integration
- Real-time workflow automation
- Google Sheets synchronization
- No manual intervention required

---

## Example AI Responses

| Customer Message | AI Decision |
|---|---|
| "Yes, I confirm my order" | confirmed |
| "I want to cancel" | cancelled |
| "Can I change the address?" | needs_more_info |

---

## Repository Structure

```text
├── docs/
├── workflow/
├── screenshots/
├── diagrams/
├── README.md
└── .gitignore
```

---

## Screenshots

Screenshots and workflow demonstrations are available in the `/screenshots` folder.

---

## UML & Documentation

The project documentation includes:

- Use Case Diagram
- Sequence Diagram
- Technical Architecture
- Workflow Documentation
- PFA Report

---

## Future Improvements

- Arabic voice AI agent
- CRM integration
- Dashboard analytics
- Multi-language support
- Automatic delivery tracking

---

## Author

**Ilyass FIRAR**  
EMSI – Computer Engineering Student  
Morocco

---

## Academic Context

This project was created as part of a final year academic project (PFA) focused on AI automation and e-commerce workflow optimization.
