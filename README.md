# n8n AI-Powered Inventory Manager

A modern, AI-driven inventory management system built with **n8n**, **Airtable**, and **OpenAI**.  
This workflow allows you to automatically track product inventory, search records, and update prices based on AI-driven inputs, all via a conversational interface.

## Features

- **AI Chat Integration**: Receive instructions via chat and let the AI determine which products to update.
- **Airtable Integration**: Seamlessly search and update your Airtable inventory database.
- **Price Management**: Automatically update both retail and manufacturer prices.
- **Memory Buffer**: Keep context across AI interactions to handle complex workflows.
- **Dynamic Tool Usage**: AI decides when and how to perform record updates.

## Workflow Overview

1. **When chat message received** – Trigger workflow based on incoming messages.
2. **AI Agent** – Processes the message using OpenAI and decides which tools to use.
3. **OpenAI Chat Model** – Handles natural language understanding.
4. **Simple Memory** – Maintains a conversation context for multi-step tasks.
5. **Search records in Airtable** – Finds the relevant product records in your inventory.
6. **Update record in Airtable** – Updates the product price and manufacturer price based on AI recommendations.

## Setup

1. Clone this repository.
2. Import the workflow JSON into your n8n instance.
3. Configure credentials:
   - OpenAI API Key
   - Airtable Personal Access Token
4. Update the workflow with your Airtable Base and Table IDs.
5. Activate the workflow and start sending chat commands to manage inventory.

## Example Commands

- "Update the price of Product X to $25."
- "Increase Manufacturer Price of Product Y by 10%."
- "Check inventory for The High Street store."

## Tech Stack

- [n8n](https://n8n.io) – Workflow automation
- [Airtable](https://airtable.com) – Cloud database for inventory
- [OpenAI GPT](https://openai.com) – Conversational AI for decision making

## License

This project is licensed under the MIT License.  

---
