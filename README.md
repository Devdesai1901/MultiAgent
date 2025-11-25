# 🌍 Multi-Agent Travel Itinerary Planner  
### Built with LangGraph • Streamlit • Ollama

Your **AI-powered personal travel concierge**, powered by a multi-agent architecture that collaboratively builds smart, personalized itineraries.  
From daily plans to weather forecasting, cultural insights, packing lists, and travel links — this system handles everything.


---

## ✨ Key Features

- 🧠 **Multi-Agent Workflow** driven by LangGraph  
- 🗺️ **Daily itinerary generation** with food, sightseeing & leisure  
- 🎭 **Unique local activity recommendations**  
- ☁️ **Weather forecasting** tailored to your travel month  
- 🎒 **Smart packing checklist** based on climate & activities  
- 🍜 **Food & cultural insights** for an authentic experience  
- 🔗 **Useful travel links** (Top 5 guides) via Serper API  
- 💬 **Chat agent** for any itinerary-related questions  
- 📄 **One-click PDF export**  
- 🧩 **Modular codebase** — easily extend or create new agents  

---

## 🧱 Project Structure

```
MultiAgents-with-Langgraph-TravelItineraryPlanner/
│
├── agents/
│ ├── generate_itinerary.py
│ ├── recommend_activities.py
│ ├── fetch_useful_links.py
│ ├── weather_forecaster.py
│ ├── packing_list_generator.py
│ ├── food_culture_recommender.py
│ └── chat_agent.py
│
├── export_utils.py
├── travel_agent.py
├── requirements.txt
└── .env

```


**agents/** — Individual AI modules, each specializing in one task  
**travel_agent.py** — Main Streamlit UI + LangGraph workflow  
**export_utils.py** — PDF & shared utilities  

---

## 🛠️ Setup

### ✅ Prerequisites
- Python **3.8+**
- **Ollama** installed & running locally  
  ```bash
  ollama pull llama3.2```

#  Installation
```
git clone https://github.com/vikrambhat2/MultiAgents-with-Langgraph-TravelItineraryPlanner.git
cd MultiAgents-with-Langgraph-TravelItineraryPlanner
pip install -r requirements.txt
```
```
Create a .env file:
SERPER_API_KEY=your_api_key_here

#Start Ollam
ollama serve

#run the code
streamlit run travel_agent.py
```
---
# 🧭 How to Use

- Enter your travel preferences (destination, month, duration, interests)

- Click Generate Itinerary

- Explore additional insights:

- Activities

- Weather

- Packing list

- Food & culture

- Useful travel guides

- Ask questions in the chat agent

- Export everything as a PDF
