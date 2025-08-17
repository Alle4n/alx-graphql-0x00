# Episode Queries

This directory contains GraphQL queries to fetch Rick and Morty episodes from the public API:
👉 https://rickandmortyapi.com/graphql

## 📂 Files
episode/
 ├── episode-page-1.graphql
 ├── episode-page-1-output.json

## 🚀 Queries
### Episode by ID

Fetch episode details (id, name, air_date, episode).

Example (episode-page-1.graphql):

query {
  episode(id: 1) {
    id
    name
    air_date
    episode
  }
}

## 📌 How to Test

Open 👉 https://rickandmortyapi.com/graphql

Copy the query from episode-page-1.graphql and paste it into the GraphQL Playground.

Run the query.

Save the JSON response into episode-page-1-output.json.

## ✅ Learning Goals

Learn how to fetch an episode by ID

Understand how GraphQL fields map to episode properties