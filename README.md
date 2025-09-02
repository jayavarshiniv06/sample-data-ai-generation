# ai_data_generation
AI-Powered Realistic Data Generator
This project is a sophisticated, AI-driven tool for generating realistic, referentially-intact sample data from a database schema.
It leverages Google's Gemini API to intelligently analyze a schema from a .sql or .xlsx file and generates a complete, executable plan to create high-quality test data using the Faker library.

🚀 Key Features
Dual Schema Input: Accepts either a raw SQL DDL file or a structured Excel file as input.
AI-Powered Planning: Uses Gemini API to analyze schemas, determine table generation order, and select the best data generation strategy for each column.
Referential Integrity: Ensures foreign keys always reference valid primary keys.
Scalable by Design: Batch + streaming architecture supports millions of rows with constant memory usage.
Flexible & Interactive: Specify the number of rows per table individually.
Maintainable OOP Design: Core logic split into clear classes:
SchemaReader – Reads schema from SQL/Excel.
AIPlanner – Generates the plan using Gemini.
PlanExecutor – Executes plan, generates data.
📦 Getting Started
✅ Prerequisites
Python 3.8+
A Google Gemini API Key (get one from Google AI Studio)
