[TYPESCRIPT__BADGE]: https://img.shields.io/badge/typescript-D4FAFF?style=for-the-badge&logo=typescript
[REACT__BADGE]: https://img.shields.io/badge/React-005CFE?style=for-the-badge&logo=react
[PROJECT__BADGE]: https://img.shields.io/badge/📱Visit_this_project-000?style=for-the-badge&logo=project
[PROJECT__URL]: https://eplay-monosodrac.vercel.app/
[NODE_BADGE]: https://img.shields.io/badge/node.js-20.16.0-43853D?style=for-the-badge&logo=node.js

<h1 align="center" style="font-weight: bold;">Ebac Games 💻</h1>

![react][REACT__BADGE]
![typescript][TYPESCRIPT__BADGE]
![node][NODE_BADGE]

<details open="open">
<summary>Table of Contents</summary>
 
- [📌 About](#about)
- [⚙️ Project Architecture](#architecture)
- [🚀 Getting started](#started)
  - [Prerequisites](#prerequisites)
  - [Cloning](#cloning)
  - [Backend Setup (JSON Server)](#api)
  - [Starting Frontend](#frontend)
- [🧠 Main Features](#features)
- [🧩 Technologies Used](#tech)
- [🤝 How to reach me](#reach)
  
</details>

---

<h2 id="about">📌 About</h2>

**Ebac Games** is a web-based game store built with **React**, **TypeScript**, and **Redux Toolkit**.  

The application simulates an online game shop where users can add products to a shopping cart with dynamic total calculation.  

---

<h2 id="architecture">⚙️ Project Architecture</h2>

The project follows a **modular React + Redux architecture**:

```
src/
├── assets/ # Images and icons
├── components/ # Reusable UI components
│ ├── Header/ # Header with dynamic cart info
│ └── Produto/ # Individual game card component
├── containers/
│ └── Produtos/ # Product list fetched from API
├── services/
│ └── api.ts # RTK Query configuration
├── store/
│ ├── index.ts # Redux store setup
│ └── reducers/ # Cart slice (Carrinho)
├── styles/ # Global styles and theme
└── App.tsx # Main app structure
```


The application is fully **state-managed with Redux Toolkit** and **RTK Query** for API integration, following best practices of a modern front-end architecture.

---

<h2 id="started">🚀 Getting started</h2>

<h3 id="prerequisites">Prerequisites</h3>

- [NodeJS](https://nodejs.org/en/download)
- [JSON Server](https://www.npmjs.com/package/json-server)

---

<h3 id="cloning">Cloning</h3>

```bash
git clone https://github.com/monosodrac/ebac-games-redux.git
```

<h3 id="api">Backend Setup (JSON Server)</h3>

To simulate the backend API used by the app, install and run JSON Server:

```
npm install -g json-server
```

Then, start the mock API:

```
npx json-server db.json --port 4000
```
This will make the data available at http://localhost:4000/produtos, which is used by the app via RTK Query.

<h3 id="frontend">Starting Frontend</h3>

In another terminal tab, start the React app:

```
cd ebac-games-redux
npm install
npm start
```

<h2 id="features">🧠 Main Features</h2>

- 🛍️ Shopping cart system using Redux Toolkit
- 💾 State persistence handled via slices
- 🌐 Data fetching with RTK Query connected to http://localhost:4000/produtos
- 💰 Dynamic price calculation and cart total
- 💅 Styled Components for modular styling
- 🧱 Component-based structure with reusable UI patterns

<h2 id="tech">🧩 Technologies Used</h2>

| Category                 | Technologies                         |
| ------------------------ | ------------------------------------ |
| **Frontend**             | React, TypeScript, Styled Components |
| **State Management**     | Redux Toolkit, RTK Query             |
| **Backend Mock**         | JSON Server                          |
| **Build Tools**          | React Scripts                        |
| **Linting / Formatting** | ESLint, Prettier                     |

<h2 id="reach">🤝 How to reach me</h2>

<table>
  <tr>
    <td align="center">
      <a href="https://linktr.ee/monosodrac">
        <img src="https://avatars.githubusercontent.com/u/141099551?v=4" width="100px;" alt="Mono Cardoso Profile Picture"/><br>
        <sub>
          <b>Mono</b>
        </sub>
      </a>
    </td>
  </tr>
</table>

💡 Note: This project was developed as a learning exercise to explore state management, asynchronous requests, and UI componentization in a React + TypeScript environment.
