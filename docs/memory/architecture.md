# Architecture

See [[features-built]] and [[gotchas]].

React 18 + Vite front end. Redux Toolkit and React Redux for state, React Router 6 with a `PrivateRoute` guard, React Hook Form for forms, Chakra UI for components, Axios for API calls.

- `src/main.jsx`, `src/App.jsx`, `src/Router.jsx`: entry, shell and routes. `src/PrivateRoute.jsx`: redirects when not logged in.
- `src/pages/`: `Home` (login required), `Login`, `SignUp`. `src/components/Navbar.jsx`.
- `src/store/store.jsx` with slices `LoginSlice.jsx` and `SignUpSlice.jsx`: async thunks that call the backend.
- `vite.config.js` (plus a stray `vite.config.js.timestamp-*.mjs` build artifact).

It expects an authentication API and pairs with the Spring Boot JWT project in this account.
