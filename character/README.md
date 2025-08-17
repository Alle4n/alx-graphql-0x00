# Character Queries

This directory contains GraphQL queries to fetch Rick and Morty characters from the public API:
👉 https://rickandmortyapi.com/graphql

## 📂 Files
character/
 ├── character-id-1.graphql
 ├── character-id-1-output.json
 ├── character-id-2.graphql
 ├── character-id-2-output.json
 ├── character-id-3.graphql
 ├── character-id-3-output.json
 ├── character-id-4.graphql
 ├── character-id-4-output.json
 ├── characters-page-1.graphql
 ├── characters-page-1-output.json
 ├── characters-page-2.graphql
 ├── characters-page-2-output.json
 ├── characters-page-3.graphql
 ├── characters-page-3-output.json
 ├── characters-page-4.graphql
 ├── characters-page-4-output.json

## 🚀 Queries
### 1. Character by ID

Fetch character details (id, name, status, species, type, gender).

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

### 2. Paginated Characters

Fetch a list of characters by page (id, name, status, image).

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

## 📌 How to Test

Open 👉 https://rickandmortyapi.com/graphql

Copy a query from this folder and paste it into the GraphQL Playground.

Run the query.

Save the JSON response into the corresponding *-output.json file.

## ✅ Learning Goals

Practice fetching single characters by ID

Learn pagination with GraphQL

Work with real-world API responses