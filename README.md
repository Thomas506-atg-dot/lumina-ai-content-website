Lumina — AI Content & Virtual Influencer Agency

A single-page marketing website for an AI content creation agency, built with HTML, CSS, and vanilla JavaScript.

Live site: https://lumina-labs.netlify.app/

Features
Live contact form — submissions are sent directly to a Google Sheet in real time via a Google Apps Script web app, so incoming enquiries can be tracked without a backend server.
Calendly booking integration — visitors can toggle between sending a message or booking a call directly, via an embedded Calendly widget.
WhatsApp quick-chat button — one-tap direct messaging for visitors who want an instant response.
Scroll-triggered animations — sections fade in as the user scrolls, implemented with the native IntersectionObserver API (no animation library dependency).
Gallery lightbox — a custom lightbox for viewing gallery images at full size, closable via click or the Escape key.
Responsive glassmorphic navigation — a floating, blurred nav bar that condenses on scroll and highlights the active section as the user scrolls through the page.
Tech stack
HTML5 / CSS3 (custom properties for a consistent design token system — colors, spacing, typography — defined once and reused throughout)
Vanilla JavaScript (no frontend framework)
Bootstrap 5 (bundle JS, for minor UI utilities)
Font Awesome (icons)
Google Fonts — Inter (body) and Syne (display/headings)
Google Apps Script (serverless form handling → Google Sheets)
Calendly embed (scheduling)
Project structure

Everything — HTML structure, CSS, and JavaScript — currently lives in a single index.html file for simplicity, since this is a static one-page site with no build step.

index.html
Running locally

No installation or build tools required — just open index.html directly in a browser, or serve the folder with any static file server.

Notes

The contact form posts to a Google Apps Script endpoint that appends submissions as rows in a connected Google Sheet. The Calendly link and WhatsApp number are configured directly in the HTML/JS for easy editing.
