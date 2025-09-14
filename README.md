# Trello REST APIs — Postman Collection

## 📌 Overview

This repository contains a Postman collection and related configuration files for interacting with the [Trello REST API](https://developer.atlassian.com/cloud/trello/rest/api-group-actions/). It enables developers and testers to:

- Send authenticated requests to Trello endpoints.
- Perform operations like creating boards, lists, cards, etc.
- Use environment and global variables for better request management.

---

## 📁 Repository Contents

| File Name                              | Description                                                                 |
|----------------------------------------|-----------------------------------------------------------------------------|
| `Trello.postman_collection (1).json`   | Main Postman collection with Trello API requests.                          |
| `Live.postman_environment.json`        | Environment file with base URL, API key/token placeholders.                |
| `workspace.postman_globals.json`       | Global variables shared across environments.                               |     |

---

## 🚀 Getting Started

### Prerequisites

- [Postman](https://www.postman.com/downloads/) (desktop or web version)
- Trello account
- Trello API Key and Token  
  - Get them from: https://trello.com/app-key

---

### Setup Instructions

1. Clone this repository or download the ZIP.
2. Open Postman.
3. Go to **File → Import**, then import:
   - `Trello.postman_collection (1).json`
   - `Live.postman_environment.json`
   - `workspace.postman_globals.json` (optional but recommended)
4. In Postman, select the **Live** environment from the top-right dropdown.
5. Update the following variables in the environment:
   - `key` → Your Trello API key
   - `token` → Your Trello API token
   - `baseUrl` → Usually `https://api.trello.com/1`
   - Any board/list/card IDs as needed

---

## ⚙️ Postman Variables

### Environment Variables (`Live.postman_environment.json`)

| Variable | Description                    |
|----------|--------------------------------|
| `key`    | Trello API Key                 |
| `token`  | Trello API Token               |
| `baseUrl`| Trello API Base URL            |
| `boardId`| ID of a Trello board           |
| `listId` | ID of a list within a board    |
| `cardId` | ID of a card                   |
| `...`    | Add others as needed           |

---

## 📬 Collection Details

The Postman collection includes the following types of requests:

<!-- TODO: Update the list of endpoints with accurate categories and descriptions -->
- ✅ **Board Operations**
  - Create board
  - Delete board
  - Get board details

- ✅ **List Operations**
  - Create a list
  - Get lists on board

- ✅ **Card Operations**
  - Create card
  - Update card
  - Move card to another list

- ✅ **Label Operations**
  - Add label to card
  - Get card labels

- ⛔ **More endpoints...**
  - <!-- TODO: Add any other endpoint groups you've included -->

Each request uses environment or global variables for authentication and URLs.

---

## 🧪 Tests & Automation

Some requests may include Postman test scripts that validate:
- Response status codes
- Response body structure
- Variable extraction for chaining requests

---

