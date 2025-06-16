# Personal Portfolio

This serves as a personal portfolio to showcase my background and work in IT. It is designed for both potential clients and employers to gain a clear understanding of who I am and the value I bring to a project or team. The design is straightforward and functional, without unnecessary complexity. The site includes four main pages: Home, About, Projects, and Contact. Each page provides concise and relevant information, with the Projects page receiving the most focus to highlight my previous work and accomplishments.

## 🚀 Features

- Home, About, Projects, and Contact pages
- Fully responsive design
- Modal-based documentation for detailed project insights
- Links to external user/project pages

## 🛠 Technologies Used 

- **Vite** – Fast build tool for efficient development
- **React** – Component-based frontend framework
- **TypeScript** – Ensures type safety and better code quality
- **MUI** – Prebuilt UI components for consistent design
- **GitHub Pages** – Used for deployment
- **HTML** – Base structure for deployment compatibility
- **CSS** – For global styling and layout

## 🎨 Design Approach

The site was built with a mobile-first approach to ensure responsiveness across all devices, particularly mobile, which is the most commonly used today. The overall layout is minimalist and user-friendly, aimed at delivering essential information quickly. For those interested in exploring more, each project includes links to deeper documentation or live versions.

## ⚙️ Challenges & Solutions

One of the main challenges in this project was deploying a React application to GitHub Pages, which only supports static content. React apps typically rely on browser-based routing, which can break when refreshing or directly accessing routes on GitHub Pages.

To solve this, I used the ``gh-pages`` package, which simplifies the deployment process by pushing the production-ready build to a separate branch configured for GitHub Pages. Additionally, I implemented hash-based routing (``HashRouter`` from ``react-router-dom``) instead of browser-based routing to ensure that all routes function correctly in the static environment.
