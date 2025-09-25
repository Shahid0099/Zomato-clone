# Copilot Instructions for Zomato-Clone

## Project Overview
- This is a Zomato-like food delivery web app built with React (Create React App).
- The app is organized by feature: Home, Collection, Filter, Food, Restaurant, Cart, Payment, Authentication, etc.
- UI components are grouped in `src/Components/` by domain (e.g., `Delivery/`, `DetailsPage/`, `DinningOut/`, `CartPage/`, `PaymentPage/`).
- Data and configuration are in `src/Components/Data/` and `src/firebase.config.js`.
- Static assets (images, icons) are in `src/Components/Images/` and `src/Components/Icons/`.

## Key Files & Structure
- `src/App.js`: Main app entry, sets up routing and layout.
- `src/Components/AllRoutes/AllRoutes.jsx`: Centralizes all route definitions.
- `src/Components/Authentication/`: Login, Signup, and PopUp components for user auth.
- `src/Components/Delivery/` and `src/Components/DetailsPage/`: Food category and detail views.
- `src/Components/CartPage/CartPage.jsx`: Shopping cart logic.
- `src/Components/PaymentPage/`: Payment and success flow.
- `db.json`: Local mock database for development (if used).

## Developer Workflows
- **Start dev server:** `npm start` (runs on http://localhost:3000)
- **Run tests:** `npm test` (Jest, see `App.test.js`)
- **Build for production:** `npm run build`
- **Firebase config:** Set up in `src/firebase.config.js` (not committed, add your own keys if needed)

## Project Conventions
- **Component Naming:** PascalCase for components and files (e.g., `CartPage.jsx`).
- **CSS:** Each feature/component has its own CSS file in the same folder.
- **Routing:** All routes are managed in `AllRoutes.jsx`.
- **Data Flow:** Props drilling is common; no global state management (Redux, Context) is present by default.
- **Testing:** Minimal, mostly in `App.test.js`.
- **No TypeScript:** All code is JavaScript.

## Integration & Patterns
- **Firebase:** Used for authentication (see `firebase.config.js`).
- **Mock Data:** Some data is hardcoded or in `db.json`/`FilterData.js`.
- **Images/Icons:** Use relative imports from `Images/` and `Icons/` folders.
- **No backend/server code** in this repo; all logic is client-side.

## Examples
- To add a new food category: create a new component in `Delivery/` and a detail view in `DetailsPage/`, then add a route in `AllRoutes.jsx`.
- To update authentication: edit components in `Authentication/` and update Firebase config as needed.

## References
- See `README.md` for screenshots and basic usage.
- For new features, follow the folder/component structure and naming conventions above.

---

_If any section is unclear or missing, please provide feedback for further refinement._
