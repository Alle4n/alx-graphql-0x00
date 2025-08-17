# alx-graphql-0x00

This project contains GraphQL queries and outputs for the Rick and Morty GraphQL API.
It demonstrates how to query characters and episodes using the public GraphQL endpoint:

👉 https://rickandmortyapi.com/graphql

## 📂 Structure
alx-graphql-0x00/
 ├── character/
 │    ├── character-id-1.graphql
 │    ├── character-id-1-output.json
 │    ├── character-id-2.graphql
 │    ├── character-id-2-output.json
 │    ├── character-id-3.graphql
 │    ├── character-id-3-output.json
 │    ├── character-id-4.graphql
 │    ├── character-id-4-output.json
 │    ├── characters-page-1.graphql
 │    ├── characters-page-1-output.json
 │    ├── characters-page-2.graphql
 │    ├── characters-page-2-output.json
 │    ├── characters-page-3.graphql
 │    ├── characters-page-3-output.json
 │    ├── characters-page-4.graphql
 │    ├── characters-page-4-output.json
 │    └── README.md
 ├── episode/
 │    ├── episode-page-1.graphql
 │    ├── episode-page-1-output.json
 │    └── README.md

## 🚀 Queries
Characters by ID

Fetch character details (id, name, status, species, type, gender) by ID.

Example (character-id-1.graphql):

query {
  character(id: 1) {
    id
    name
    status
    species
    type
    gender
  }
}

## Paginated Characters

Fetch characters by page (id, name, status, image).

Example (characters-page-1.graphql):

query {
  characters(page: 1) {
    results {
      id
      name
      status
      image
    }
  }
}

## Episode by ID

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

## 📌 How to Run Queries

Go to 👉 https://rickandmortyapi.com/graphql

Copy the query from .graphql file.

Paste into the GraphQL Playground.

Save the JSON response into the corresponding *-output.json file.

## ✅ Learning Goals

Understand GraphQL queries and parameters

Practice fetching data by ID and by pagination

Work with real-world API data outputs