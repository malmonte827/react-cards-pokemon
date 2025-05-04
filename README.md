# 📇 React Cards & Pokémon

> A React app that fetches and displays playing cards and Pokémon cards, refactored to use two custom hooks—`useFlip` for card‐flip logic and `useAxios` for data fetching and state management.

 [![React](https://img.shields.io/badge/react-18%2B-blue)](https://reactjs.org/) [![Axios](https://img.shields.io/badge/axios-0.27%2B-brightgreen)](https://github.com/axios/axios)

---

## 📋 Table of Contents

1. [About](#about)  
2. [Features](#features)  
3. [Tech Stack](#tech-stack)  
4. [Getting Started](#getting-started)  
   - [Prerequisites](#prerequisites)  
   - [Installation](#installation)  
5. [Usage](#usage)  
6. [Custom Hooks](#custom-hooks)  
8. [Contributing](#contributing)  
10. [Contact](#contact)  

---

## 🌟 About

This assignment refactors a React app that displays:

- **Playing cards** drawn from the [Deck of Cards API](https://deckofcardsapi.com/).  
- **Pokémon cards** fetched from the [PokéAPI](https://pokeapi.co/).

---

## ✨ Features

- **Draw Playing Cards:** Click “Draw Card” to fetch and display a new card image.  
- **Browse Pokémon:** Click “Add Pokémon” to fetch a random Pokémon and display its image, name, and type.  
- **Flip Cards:** Click any card to flip it over using shared `useFlip` logic.  
- **Persistent State:** Cards you draw remain on screen until you clear them.  

---

## 🛠 Tech Stack

- **Library:** React 18+  
- **Data Fetching:** Axios  
- **APIs:** Deck of Cards API, PokéAPI  
- **Build Tool:** Create React App (or Vite if preferred)  
- **Styling:** CSS  

---

## 🏁 Getting Started

### Prerequisites

- Node.js v14 or higher  
- npm (bundled with Node.js) or Yarn  

### Installation

```bash
# 1. Clone the repo
git clone https://github.com/malmonte827/react-cards-pokemon.git
cd react-cards-pokemon

# 2. Install dependencies
npm install
# or
yarn

# 3. Start the dev server
npm start
# or
yarn start
```
---
### 📖 Usage

1. Draw Playing Card

   - Click the “Draw Card” button to fetch and display a new card from the deck.

2. Add Pokémon

   - Click “Add Pokémon” to fetch a random Pokémon’s data (name, image, type).

3. Flip Cards

   - Click on any displayed playing card or Pokémon card to flip it face down/up.

4. Clear Cards

   - Use “Clear Cards” buttons in each section to reset that collection.
---
### Custom Hooks
useFlip

  - Encapsulates flip state (isFlipped) and a toggleFlip() function.

  - Used by both PlayingCard and PokemonCard components.

useAxios

   - Takes a base URL and returns [ dataArray, addData ].

   - addData performs an Axios request (optionally appending to the URL) and pushes the result into dataArray state.

   - Used in PlayingCardList and PokeDex to handle all AJAX logic.
---

## Contributing

We welcome contributions! To contribute:

- Fork the repository

- Create a new branch (git checkout -b feature-name)

- Commit your changes (git commit -m 'Add new feature')

- Push to the branch (git push origin feature-name)

- Open a pull request

## Contact

For questions or suggestions, reach out:

- Email: malmonte827@gmail.com
