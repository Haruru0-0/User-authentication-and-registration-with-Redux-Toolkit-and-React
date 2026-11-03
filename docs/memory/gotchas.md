# Gotchas

See [[architecture]].

- **No API is included.** Without a running authentication backend, login and sign-up fail. The URL is hard-coded in the slices (for example `http://localhost:8080/api/v1/auth/authenticate`), which is where the JWT demo listens.
- **Run with `yarn install` then `yarn dev`.**
- **`vite.config.js.timestamp-*.mjs` is a committed leftover** from Vite; it can be deleted.
- **`graphify.exe` is blocked on this machine;** use `python -m graphify update .`.
