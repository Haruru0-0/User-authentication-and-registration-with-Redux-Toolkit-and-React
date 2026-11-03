# Roadmap

Open items only; what exists is in [[features-built]].

- Move the API base URL into an environment variable (it is hard-coded in `LoginSlice.jsx` and `SignUpSlice.jsx`).
- Delete the stray `vite.config.js.timestamp-*.mjs` file.
- Add tests for the slices and the private route.
- Refresh the code map with `python -m graphify update .` after larger changes.
