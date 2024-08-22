---
title: React
---

React is a user interface library

Deploying a React project (with Vite and GitHub)  

1. cd new-project
2. npm create vite@latest . -- -- template react
3. npm install
4. npm run dev
5. (Write code in App.jsx)

git init, set origin

1. git init
2. git add .
3. git commit -m 'Initial commit'
4. git remote add origin https://github.com/username/repo-name
5. git remote -v

Install gh-pages, edit package.json / vite.config.js, edit GitHub repo settings

1. npm install gh-pages --save-dev
2. package.json:
		"predeploy": "npm run build",
		"deploy": "gh-pages -d build"
3. vite.config.js:
		base: "/repo-name"
4. npm run build
5. npm run deploy
6. GitHub repo > Settings > Pages > Deploy from a branch (gh-pages)
