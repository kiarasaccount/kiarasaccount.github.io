This repository contains the frontend code for my personal portfolio website, hosted using GitHub Pages.
It includes a homepage, alongside a link to two additional pages and a fully-functioning chatbot.
For more details on the chatbot, please see my backend repository!

Technologies used: HTML, CSS, JavaScript, GitHub Pages
Inside index.html, the chatbot’s JavaScript sends the message to the backend using:

const response = await fetch("https://kiara-chatbot-backend.onrender.com/ask", {
  method: "POST",
  headers: { "Content-Type": "application/json" },
  body: JSON.stringify({ question })
});

The widget uses a floating avatar image that I sourced from Canva.
This image is stored locally in the assets folder for fast global loading.
The site automatically deploys via GitHub Pages whenever you push changes to main.

The chat widget will only work if your backend is online.
The site is static, so all interactions happen through JavaScript.
