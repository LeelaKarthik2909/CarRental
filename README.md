# DriveEase Car Rental System

A beginner-friendly, frontend-only car rental demo built with HTML, CSS and JavaScript. It runs as a static site (VS Code Live Server is recommended) and stores sample vehicles, accounts, bookings and maintenance tasks in your browser LocalStorage.

## Run it

Open this folder in VS Code and start Live Server from `index.html`. You can also open `index.html` directly in a browser, though Live Server gives the most consistent results. No build step or package installation is needed.

## Accounts and access

**Admins:** sign in directly at `login.html` with any of these (password `admin123` for all): `nanda@gmail.com`, `leela@gmail.com`, `nihitha@gmail.com`. No registration is needed; these accounts are created automatically in LocalStorage.

**Customers:** every other user must click **Register here** on the login page and create an account first, then sign in with it. Booking requires sign-in, and the admin dashboard, collections, maintenance, and service manager pages require the admin account. Use Log out between people sharing a device.

## Pages

- `index.html`: rental search and featured vehicles
- `cars.html`: searchable, filterable vehicle inventory
- `register.html`, `login.html`, `logout.html`: account validation, sign-in, and a logout flow for shared devices
- `booking.html`, `payment.html`, `confirmation.html`: date-based quote, driver licence name, number, issuing region, expiry validation, licence proof upload, and simulated checkout
- `admin-dashboard.html`: manage fleet, bookings and customers
- `collections.html`: summary of demo payments
- `maintenance.html`: create, complete and delete simple service tasks
- `service-manager.html`: fleet condition, due/overdue service, repair notes, estimated service duration, and work orders
- `user-history.html`: the signed-in user’s past rentals, prices, and saved-car wish list

Car photos go in `images/cars/` and are named `<make>-<model>.jpg` (for example `toyota-corolla-cross.jpg`; see `images/cars/README.txt` for the full list). If a photo is missing, the site falls back to the illustrations in `images/car-*.svg`. Other artwork is stored locally in `images/`. Checkout is simulated; this project does not process real payments. The booking flow collects a driver’s licence name, number, issuing region, and expiry date, then accepts a licence image or PDF (up to 2 MB) so an admin can review the details in the bookings table. Do not use real sensitive documents in this frontend-only demo. Rental history includes bookings made after signing in; historical bookings created before the daily-rate field was added show an estimated rate. Saved-car wish lists are per user. LocalStorage data is specific to the browser and device where the demo runs. Use the browser developer tools to clear LocalStorage and restore the sample data.
