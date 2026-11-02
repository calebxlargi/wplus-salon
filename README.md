# W+ Salon

Responsive static website for W+ Salon at KEDAI KL, MAHSA Avenue, Kuala Lumpur.

## Deploy with Cloudflare Pages

1. In Cloudflare, open Workers & Pages and create a **Pages** project using an existing Git repository.
2. Connect GitHub and select `calebxlargi/wplus-salon`.
3. Production branch: `main`.
4. Framework preset: **None**.
5. Build command: leave blank (or `exit 0` if required).
6. Build output directory: `public`.
7. Deploy. Cloudflare supplies the available `*.pages.dev` address.

The repository can stay private. Give Cloudflare access to this repository when prompted. Future commits to main automatically redeploy.

## Local preview

Run `python3 -m http.server 8000 --directory public` and visit localhost:8000.

## Content

- `public/index.html`: page content, opening hours, address, directions.
- `public/app.js`: service menu, rates, selections, massage duration and WhatsApp request.
- `public/style.css`: responsive styles.
- `public/assets/`: optimized photographs provided by the salon and SVG logo assets.

Confirmed prices: men's haircut with wash RM50; wash & blow RM15; head & shoulder massage RM1/minute. Other starting prices were selected with the owner using indicative KL rates. Confirm final quotes with clients.

Hours: Tuesday–Sunday 10 am–6 pm; closed Monday. Appointment requests go to +60 14-669 2096. Customers must press Send in WhatsApp; no message is sent automatically. No booking data is stored or processed by a server.

Logo: manually reconstructed SVG paths from the provided raster reference. The original font has not been identified; this is a visual reconstruction, not a verified exact-font reproduction. Photographs and branding remain the owner's property.

No database, API keys, paid WhatsApp API or build dependencies are needed. Website fonts are loaded from Google Fonts, with local system fallbacks.
