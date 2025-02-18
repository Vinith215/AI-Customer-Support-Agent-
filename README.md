# AI-Customer-Support-Agent-

This Streamlit app features an AI-driven customer support agent powered by OpenAI's GPT-4o. 
It leverages synthetic data generated with GPT-4o and utilizes the Mem0 library for memory retention, with Qdrant serving as the vector store.

Features:

Interactive chat interface for engaging with the AI-powered customer support agent
Retains customer interactions and profiles for a seamless experience
Generates synthetic data for testing and demonstrations
Leverages OpenAI's GPT-4o model to provide intelligent and context-aware responses

How to get started?

1. Install the required dependencies:
  pip install -r requirements.txt

2. Make sure Qdrant is running: The application requires Qdrant to be active on localhost:6333. If your setup differs, update the configuration in the code accordingly.
  docker pull qdrant/qdrant 
  docker run -p 6333:6333 -p 6334:6334 -v "${PWD}/qdrant_storage:/qdrant/storage" qdrant/qdrant

3. Run the Streamlit App
  streamlit run customer_support_agent.py
