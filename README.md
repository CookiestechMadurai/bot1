Dialogflow Event Query Project README
Overview
This project is a Dialogflow agent designed to help users query event details based on their input. The agent responds with event information such as event name, location, date, and category. Users can ask for events happening in specific cities or on specific dates, and the agent will provide the relevant event details.

Features:
Dialogflow Intents: The project uses Dialogflow intents to capture user queries regarding events.
Event Data: The agent is configured to return pre-defined event information stored within Dialogflow's intents or entities.
Prerequisites
Before running the Dialogflow agent, ensure the following:

Google Cloud Project:

Create a Google Cloud project in the Google Cloud Console.
Enable the Dialogflow API.
Dialogflow Agent:

Create a Dialogflow agent in the Dialogflow Console.
Set up intents and entities relevant to your event queries (e.g., EventDetails intent with parameters like city, event_date, etc.).
Setup
Create a Dialogflow Agent:

If you haven’t already, go to the Dialogflow Console and create a new agent.
Set the default language and time zone.
Create Intents:

Set up an intent (e.g., GetEventDetails) to capture queries like:
"What events are happening in Chennai?"
"Tell me about events on 2025-08-02"
Define parameters such as city, event_date, and event_category.
Train the agent to recognize variations of user queries.
Create Entities (Optional):

You can create custom entities like @city for cities (e.g., "Chennai", "Mumbai") and @event_category for event categories (e.g., "Music", "Tech").
Set up Fulfillment (Optional):

If you want to integrate external data, set up a webhook to provide real-time event data.
If not, you can define event details directly within the intent responses.
Enable Webhook (Optional):

If using external sources (like a database or API), enable webhook fulfillment to fetch event details dynamically.
Set up the webhook URL and configure it in the Fulfillment section of Dialogflow.
Testing the Agent:

Use the Dialogflow console’s Try it now section to interact with the agent.
Type queries like "What events are happening in Chennai on August 2, 2025?"
Verify that the correct responses are provided based on the predefined event details.
