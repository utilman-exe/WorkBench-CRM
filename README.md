# Workbench CRM

A free, open-source CRM built for small computer and device repair shops. Everything runs in a single HTML file — no server, no backend, no account required. Open the file in a browser and start working.

---

## What it does

Workbench CRM covers the full workflow of a repair shop:

- **Repairs** — track tickets from intake to completion, log status changes, attach photos, record parts used, print thermal tickets
- **For Sale** — manage device listings with full specs, ad text, profit calculator, bundled accessories and photo gallery
- **Inventory** — parts and devices with category-specific fields (RAM speed/type, SSD health, CPU, GPU, charger wattage and more), shipping status, low-stock alerts
- **Customers** — contact cards, full repair history, merge duplicates
- **Invoices** — line items, VAT/ÁFA, link to repairs, print A4
- **Notes** — colour-coded sticky notes, pin important ones to the dashboard
- **Dashboard** — at-a-glance view of due and overdue repairs, low stock, pinned notes, weekly revenue
- **Reports** — monthly repair and revenue charts, device type breakdowns, for-sale status analysis

---

## Features at a glance

| Category | Details |
|---|---|
| **Data** | All data stored in browser `localStorage` — nothing leaves the device |
| **Export / Import** | Full JSON backup and restore, CSV export for repairs, inventory and for-sale |
| **Currency** | Selectable: €, £, $, Ft, Kč, zł, kr, lei, CHF |
| **Themes** | Dark, Light, OLED |
| **PIN lock** | Optional PIN to protect data on shared devices |
| **Photos** | Attach up to 6 photos per repair or listing, auto-compressed |
| **Search** | Global search across all tabs |
| **Keyboard shortcuts** | `N` new repair, `1–8` tabs, `Ctrl+S` save, `Esc` close |
| **Print** | Thermal 80mm repair tickets, A4 invoices |
| **Offline** | Works with no internet after first load (fonts/icons from CDN) |

---

## Laptop & device fields

Workbench CRM has deep spec tracking for the devices you handle most:

- **Laptops** — CPU model, RAM, storage, battery health, SSD health (SMART), OS, screen condition, screen resolution, serial number, fingerprint reader, IR camera, charger included, BIOS password, GPU, repaste history
- **Desktop PCs** — CPU, RAM, storage, GPU, form factor, OS
- **Smartphones / Tablets** — model, storage, condition, battery health
- **Monitors** — size, resolution, panel type, refresh rate
- **Inventory parts** — RAM (type/speed/maker/form factor), SSD/HDD (interface/health/M.2 size), CPU, GPU, PSU, chargers (wattage/connector), and more

---

## Getting started

### Option 1 — GitHub Pages (recommended)

1. Fork this repository
2. Go to **Settings → Pages**
3. Set source to `main` branch, root `/`
4. Your CRM will be live at `https://yourusername.github.io/workbench-crm/WorkbenchCRM.html`

### Option 2 — Local file

1. Download `WorkbenchCRM.html`
2. Open it in any modern browser (Chrome, Firefox, Edge, Safari)
3. Bookmark it — that's your app

### Option 3 — Self-hosted

Drop `WorkbenchCRM.html` onto any web server or file host. No configuration needed.

---

## Data & privacy

All data is stored in your browser's `localStorage`. Nothing is sent anywhere. No analytics, no tracking, no accounts.

**Backups:** Use the **Export** button regularly to download a full JSON backup. Import it on any device or browser to restore everything.

Storage limit: browsers allow roughly 5–10 MB of localStorage. If you store many high-resolution photos this limit may be approached — the app will warn you before it becomes a problem and photos are automatically compressed on upload.

---

## Customisation

| Setting | Where |
|---|---|
| Currency | Header `€` button → pick from 11 currencies |
| Theme | Header theme toggle (Dark / Light / OLED) |
| PIN lock | Header 🔒 button |

---

## Keyboard shortcuts

| Key | Action |
|---|---|
| `N` | New repair ticket |
| `1` – `8` | Switch tabs |
| `Ctrl + S` | Save open form |
| `Ctrl + F` | Focus search |
| `Esc` | Close modal |

---

## Screenshots

> Add your own screenshots to the `screenshots/` folder and link them here.

---

## Contributing

Contributions are welcome. If you find a bug or want to suggest a feature:

1. Open an issue describing the problem or idea
2. Fork the repo and create a branch
3. Make your changes to `WorkbenchCRM.html`
4. Open a pull request

Since the entire app is a single HTML file, changes are straightforward to review and test. Just open the file in a browser.

---

## Stack

| Layer | Technology |
|---|---|
| UI | Vanilla HTML/CSS/JS — zero frameworks |
| Icons | [Tabler Icons](https://tabler.io/icons) (CDN) |
| Fonts | [IBM Plex Sans & Mono](https://fonts.google.com/specimen/IBM+Plex+Sans) (CDN) |
| Storage | Browser `localStorage` |
| Build | None — single file |

---

## Roadmap ideas

- [ ] Multi-device sync via a lightweight backend or Cloudflare Worker
- [ ] Supplier contact book
- [ ] Recurring repair templates
- [ ] Barcode / QR code scanning for serial numbers
- [ ] Email / SMS notification hooks
- [ ] Dark-mode PDF invoice export

---

## License

MIT License — free to use, modify and distribute. See [LICENSE](LICENSE) for details.

---

> Built for repair shops, by someone who knows the workbench.
