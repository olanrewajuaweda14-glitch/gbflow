# GBFlow

**One connected flow from the factory to the corner shop.**

GBFlow is a route-to-market platform that links small retailers, distributors and the manufacturer on a single shared system. When a retailer runs low on stock, the distributor sees the demand, the delivery gets planned, and the manufacturer sees what is selling and where, all in real time.

---

## The problem

In informal and semi-formal retail, the chain from manufacturer to distributor to shop runs on phone calls, paper and guesswork.

- Retailers run out of stock without warning, or over-order and tie up cash.
- Distributors plan routes and inventory without clear demand signals.
- Manufacturers cannot see what happens after goods leave the warehouse.
- Small retailers struggle to get working capital to restock.

## The solution

GBFlow puts all three parties on the same live data.

| Role | What they get |
|---|---|
| **Retailer** | Smart restock suggestions, easy ordering, order tracking, access to demo financing, and a growth passport that builds a record of their business |
| **Distributor** | Incoming orders, demand clusters by area, route planning, delivery tracking and live inventory |
| **Manufacturer** (shown as GBfoods in the app) | A command centre showing network-wide demand, opportunities and retailer coverage |

---

## Features

### Retailer
- Stock advisor that recommends what to reorder
- Product catalogue, cart and checkout
- Order tracking from placed to delivered
- Demo financing flow (draft, submitted, under review, approved, disbursed, repaid)
- Growth passport and notifications

### Distributor
- Order queue with confirm, prepare, ready, out for delivery and delivered stages
- Retailer list and demand clusters
- Map view and route planning
- Inventory tracking: available, reserved, out for delivery, delivered

### Manufacturer
- Command centre with network-wide demand
- Opportunity detection
- Retailer network overview

### Across the whole app
- **Shared state:** an order placed by a retailer appears for the distributor and updates the manufacturer's view immediately.
- **Order lifecycle:** a clear status flow, with cancel and decline handling.
- **Demo accounts:** one-click access to each role, plus real sign-up and sign-in.
- **Reset Demo:** wipes the demo data and starts fresh.
- **Accessibility:** keyboard navigation and reduced-motion support.
- **Responsive:** works on desktop, tablet and phone.

---

## How to try it

1. Open `index.html` in any modern browser.
2. Click **Explore the demo** and choose a role.
3. Suggested walkthrough:
   1. As a **Retailer**, open the stock advisor, add items to the cart and place an order.
   2. Switch to the **Distributor** and confirm the order, then move it through preparing, ready and out for delivery.
   3. Switch back to the **Retailer** and watch the tracker update.
   4. Open the **Manufacturer** view to see the demand reflected.
4. Use **Reset Demo** to return everything to the starting state.

---

## Run locally

No installation is needed.

1. Download `index.html`.
2. Double-click it, or open it from your browser.

---

## How it works

- **One file.** The whole app is a single `index.html` with plain HTML, CSS and JavaScript. There is no build step and no dependencies.
- **Shared state.** All three roles read and write the same data store, so changes show up everywhere.
- **Saved in the browser.** Data is kept in `localStorage`, and open tabs stay in sync with each other.
- **Order state machine.** Orders can only move through valid steps, which keeps inventory and tracking consistent.
- **Route planning.** Deliveries are ordered with a nearest-neighbour approach.
- **Separate demo data.** Demo and real accounts use separate data so they never mix.

---

## Important notes

- **All data is simulated.** Retailers, orders, prices and figures are made up for demonstration.
- **Financing is a demo only.** GBFlow is not a bank or a lender, and no real money moves.
- **Accounts live in your browser only.** There is no server, so an account made on one device will not exist on another. Passwords are hashed in the browser, which is fine for a prototype but not a replacement for real authentication. Do not reuse a real password.
- **No real map service.** Locations and routes are illustrative.

---

## Roadmap

- A real backend (for example Supabase) so data is shared across devices and users
- Real authentication with email verification and password reset
- Live map and routing with a mapping provider
- Integration with a licensed financing partner
- Mobile app wrapper and offline support for low-connectivity areas
- Analytics on demand, stockouts and delivery performance

---

## License

All rights reserved unless a license is added.
