# AI-Driven E-commerce Sales Agent (Annaqa Brand)

A production-ready AI Sales Agent integrated with Facebook Messenger, designed to automate the full sales cycle for the Egyptian clothing brand "Annaqa". This system uses RAG (Retrieval-Augmented Generation) for policy lookup and dynamic inventory management via Google Sheets.

## 🚀 Features
- **Semantic Product Search:** Powered by Supabase Vector Store for intelligent product recommendations.
- **Dynamic Inventory Management:** Real-time synchronization with Google Sheets for stock levels and pricing.
- **Automated Order Processing:** Intelligent data extraction using a Structured Output Parser to record orders into Google Sheets.
- **Complex Shipping Logic:** Automatically calculates total costs by combining product prices with region-specific shipping fees retrieved via RAG.
- **Human-like Interaction:** Personalized Egyptian-Arabic persona for higher customer engagement.
- **Session Persistence:** Managed via Redis to maintain conversation context across sessions.

## 🛠️ Tech Stack
- **Orchestration:** n8n (Advanced Workflows)
- **LLM:** OpenAI GPT-4o / GPT-3.5
- **Vector Database:** Supabase (Vector)
- **Memory/Cache:** Redis
- **Database/CRM:** Google Sheets API
- **Integration:** Facebook Messenger API (Webhooks)

## 🏗️ Architecture
The system follows a modular "Chain-over-Agent" architecture:
1. **The Brain (AI Agent):** Handles natural conversation and tool selection.
2. **The Guard (IF Node):** Triggers order processing only upon final confirmation.
3. **The Parser (LLM Chain):** Extracts structured JSON from conversation logs for database entry.
4. **The Database (Google Sheets):** Acts as a lightweight CRM and Inventory system.

## 📈 Optimization & Performance
- **Token Efficiency:** Implemented server-side filtering (GQL) for Google Sheets to handle large inventories without exceeding LLM context limits.
- **Error Handling:** Integrated Auto-fix parsers to handle inconsistent LLM outputs.
