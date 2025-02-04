# Hospital Chatbot

## Setup

The chatbot uses Gemini, so you'll need to create an [Google API key](https://aistudio.google.com/app/apikey) and store it as `GOOGLE_API_KEY`. 

The three `NEO4J_` variables are used to connect to your Neo4j AuraDB instance. Follow the directions [here](https://neo4j.com/cloud/platform/aura-graph-database/?ref=docs-nav-get-started) to create a free instance.

Once you have a running Neo4j instance, and have filled out all the environment variables in `.env`, you can run the entire project with [Docker Compose](https://docs.docker.com/compose/). You can install Docker Compose by following [these directions](https://docs.docker.com/compose/install/).

Once you've filled in all of the environment variables, set up a Neo4j AuraDB instance, and installed Docker Compose, open a terminal and run:

```console
$ docker-compose up --build
```

After each container finishes building, you'll be able to access the chatbot API at `http://localhost:8000/docs` and the Streamlit app at `http://localhost:8501/`.
