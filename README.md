UdaPlay AI Agent

UdaPlay is an AI research assistant for the video game industry. It allows users to ask natural language questions about video games and provides accurate, structured, and well-cited answers using a combination of internal data (RAG) and web search.

Features

Answer Game Queries: Retrieve information about game titles, release dates, platforms, genres, and publishers.

RAG Pipeline: Uses a vector database (ChromaDB) for fast semantic search.

Web Search Fallback: Uses Tavily API if internal data is insufficient.

Evaluation: Assesses the quality of retrieved data before responding.

Stateful Agent: Maintains conversation history and session-based context.

Long-term Memory: Stores useful information for future queries.

Project Structure

Udaplay_01_solution_project.ipynb – Offline RAG setup with vector database.

Udaplay_02_solution_project.ipynb – AI Agent implementation with retrieval, evaluation, and web search tools.

games/ – JSON files containing game data for vector database.

How to Run

Clone the repository:

git clone https://github.com/sanjeet207/UdaPlay-AI-Agent.git


Install dependencies:

pip install -r requirements.txt


Create a .env file with your API keys:

OPENAI_API_KEY="your_openai_key"
TAVILY_API_KEY="your_tavily_key"


Run the notebooks in order:

Udaplay_01_solution_project.ipynb – Set up vector database.

Udaplay_02_solution_project.ipynb – Test agent queries.

Example Queries

“When was Pokémon Gold and Silver released?”

“Which was the first 3D Mario platformer?”

“Was Mortal Kombat X released for PlayStation 5?”

License

This project is licensed under the MIT License.
