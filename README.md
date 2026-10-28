# MasakaFashion Hub — Internal CSS and JavaScript version

This is a responsive, static online fashion shop for Masaka, Uganda. Every HTML page contains its own CSS in a `<style>` section and JavaScript in `<script>` sections. The website no longer needs separate CSS or JavaScript files.

## Pages
1. `index.html` — Home
2. `shop.html` — searchable/filterable catalogue
3. `women.html` — Women's fashion
4. `men.html` — Men's fashion
5. `shoes-accessories.html` — Shoes and accessories
6. `about.html` — About the shop
7. `cart.html` — Shopping cart
8. `checkout.html` — Checkout form
Additional support pages: `order-confirmation.html` and `contact.html`.

## Run on your computer
1. Extract this ZIP file.
2. Open the `MasakaFashion_Hub` folder.
3. Double-click `index.html` to open the website. For development, open the folder in Visual Studio Code and use the Live Server extension.

## Before publishing
- In each HTML file, find `256700000000` and replace it with the shop's official WhatsApp number in international digits-only format (Uganda: `2567XXXXXXXX`). The configuration script is embedded separately in every page.
- Update sample contact details, opening hours, delivery fees, product descriptions and prices as needed.
- Test every page and mobile layout.

## Product imagery
Product cards, cart thumbnails and the homepage hero use locally stored photos in the `images/` folder. The photos were downloaded from [Unsplash](https://unsplash.com/license) and are used under the Unsplash License. Replace them with images that accurately represent your products before publishing.

## Important: demo vs real e-commerce
This project is a front-end demonstration. Cart and demo order data use browser `localStorage`. It has no server, database, customer account system, inventory sync, email notifications, or live payment processing. MTN Mobile Money and Airtel Money selections record a preference only; they do not send a payment request or collect money.

To accept real payments, integrate a payment provider using a secure server-side backend. Keep secret API credentials off the HTML/JavaScript client, verify provider callbacks on the server, use HTTPS, validate prices and orders on the server, and test with sandbox credentials before launch.
