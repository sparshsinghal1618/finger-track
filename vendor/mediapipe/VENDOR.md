# Vendored: MediaPipe Hands

These files are an unmodified copy of the **`@mediapipe/hands`** npm package for
offline use by the FINGER TRACK demo.

- **Package:** `@mediapipe/hands`
- **Version:** `0.4.1675469240`
- **Source:** https://www.npmjs.com/package/@mediapipe/hands
- **Upstream:** https://github.com/google/mediapipe
- **License:** Apache License 2.0 (© Google LLC) — https://www.apache.org/licenses/LICENSE-2.0

`index.html` loads `hands.js` from this folder and points MediaPipe's
`locateFile` at it, so no network access is required at runtime.

## Updating

```bash
npm pack @mediapipe/hands@<version>
tar -xzf mediapipe-hands-<version>.tgz --strip-components=1 -C vendor/mediapipe
```

Then verify `index.html` still references `vendor/mediapipe/` for both the
`<script src>` and the `locateFile` callback.
