Chatbot Project
A natural language interface chatbot that provides users with product and supplier information. Built with FastAPI, MySQL, and PyTorch, it allows users to query details about products and suppliers efficiently.

Features
Retrieve products by brand: "Show me all products under brand X."
Find suppliers by category: "Which suppliers provide laptops?"
Get product details: "Give me details of product ABC."
Installation
Clone the Repository

bash
Copy
Edit
git clone <repository-url>
cd chatbot-frontend/backend
Set Up Virtual Environment

bash
Copy
Edit
python -m venv venv
venv\Scripts\activate  # For Windows
Install Dependencies

bash
Copy
Edit
pip install fastapi uvicorn sqlalchemy pymysql transformers torch
Set Up MySQL Database

Create a database: chatbot_db
Execute SQL schema and sample data (provided in the repo).
Run FastAPI Server

bash
Copy
Edit
uvicorn main:app --reload
API Endpoint
POST /chat
Handles user queries and provides appropriate responses.
Database Schema
Suppliers: Stores supplier information.
Products: Stores product details with foreign key linking to suppliers.
