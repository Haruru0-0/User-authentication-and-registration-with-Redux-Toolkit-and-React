# User Authentication and Registration with Redux Toolkit and React

A React front end with sign-up and login flows, state managed by Redux Toolkit and protected routes.

## Stack

- React 18 and Vite
- Redux Toolkit and React Redux (`LoginSlice`, `SignUpSlice`)
- React Router 6 with a `PrivateRoute` guard
- React Hook Form for form handling
- Chakra UI for components
- Axios for API calls

## Pages

- `Home`: only reachable when logged in
- `Login` and `SignUp`: forms that call the backend through Redux async thunks

## Run it

```bash
yarn install
yarn dev
```

The app expects an authentication API to talk to; it pairs with the Spring Boot JWT project in this account.