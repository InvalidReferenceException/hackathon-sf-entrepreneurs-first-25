Repo for the August 2025 SF Hackathon organized by Entrepreneurs First

# 🌍 Explorer – Your Personal Travel & Itinerary Agent

Explorer is an intelligent travel assistant that plans your perfect day out — tailored to your interests, location, budget, and schedule.

Whether you’re looking for a scenic run, a tech event, a cozy dinner spot, or a full-day adventure, Explorer handles all the planning. Just tell it what you want to do, and it’ll generate a personalized itinerary with real locations, routes, and times — all optimized for your day.

⸻

✨ What Explorer Can Do
	•	📍 Location-aware: Suggests nearby places and events based on where you are (or where you want to go)
	•	🕐 Time- and date-sensitive: Takes into account your available time window and the day of the week
	•	💸 Budget-conscious: Finds options within your price range — from budget eats to luxury spots
	•	🧭 Activity-based planning: Handles any mix of activities — restaurants, workouts, events, hotels, and more
	•	🗺️ Smart itineraries: Builds a logical route and timing flow so everything fits neatly into your day

⸻

🚀 How It Works
	1.	Tell Explorer what you’re in the mood for — e.g.
“I’m free Friday afternoon in San Francisco with a $100 budget. I want to go for a walk, find a French restaurant, and see an AI art exhibit.”
	2.	Explorer plans your outing using real data:
	•	Finds relevant POIs near you
	•	Builds a walking route or commute plan
	•	Adjusts for opening hours and distances
	3.	Get a ready-to-use itinerary, complete with:
	•	Locations and times
	•	Google Maps links
	•	Optional Notion-style summary or exported plan

⸻

🧠 Powered By

Explorer uses a combination of:
	•	LLM-based reasoning to understand and segment your request
	•	Real-time APIs (Google Places, Maps, Events, etc.)
	•	Modular agents that specialize in hotels, events, restaurants, and more

⸻

🔧 Use Cases
	•	Last-minute weekend planning
	•	City exploration while traveling
	•	Planning a perfect date or birthday surprise
	•	Discovering new events or hidden gems near you


 Absolutely — here’s a technical stack section in Markdown that fits alongside your Explorer project description:

⸻

# 🛠 Tech Stack

Explorer is built using a modular, no-code–friendly architecture that combines automation, AI, and real-world data sources:

🔄 n8n (Workflow Automation Framework)
	•	Acts as the orchestration layer for all logic and API interactions
	•	Handles AI agent routing, tool execution, and structured output parsing
	•	Enables scalable and modular design with reusable agents (e.g., restaurantAgent, eventAgent, itineraryAgent)

🤖 AI Agents via n8n LangChain-style Tooling
	•	AI models (Anthropic, OpenAI) make decisions about what tools to call
	•	Inputs like time, location, budget, and activity preferences are parsed and delegated to specific agents

🌐 HTTP API Integrations
	•	Google Places & Maps API:
Used for geocoding, place search (searchText), and walking route generation
	•	Booking.com API (via HTTP):
Fetches hotel data and availability based on user preferences
	•	(Optional) Event APIs or Ticketmaster:
To fetch time-sensitive cultural or tech event listings in a given city

🗂️ Notion Integration
	•	Final itineraries and day plans can be exported or synced to Notion as rich, shareable pages
	•	Useful for users planning in groups or wanting a permanent itinerary archive

⸻

🔧 Modular Tool Design

Each activity type is handled by its own tool/agent:

Tool / Agent	Function
restaurantAgent	Finds food options by cuisine, area, budget
eventAgent	Surfaces events by category + date
workoutAgent	Generates run/walk loops near start point
hotelAgent	Pulls nearby hotel options
itineraryAgent	Builds day-flow and Google Maps links
contentCreator	Formats the plan into a Notion page


⸻

Let me know if you want a visual architecture diagram or a CLI/dev-ops variant of this description.
