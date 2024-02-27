# R3F - Webflow boilerplate

Build R3F to plug into Webflow

Head tag for webflow project (can be removed on Production build)

```html
<script type="module">
import RefreshRuntime from "http://localhost:5173/@react-refresh"
RefreshRuntime.injectIntoGlobalHook(window)
window.$RefreshReg$ = () => {}
window.$RefreshSig$ = () => (type) => type
window.__vite_plugin_react_preamble_installed__ = true
</script>
```

To add this at the end of the body tag (for development)
Verify your own localhost:xxxx URL
Change to production URL & update the _headers file in the public folder when ready to deploy (to avoid CORS ERROR)

```html
<script type="module" src="http://localhost:5173/@vite/client"></script>
<script type="module" src="http://localhost:5173/src/main.jsx"></script>
```

For Webflow rendering, add a div with the `id="root"` and apply the appropriate size.

### Credit

Initial fork: https://github.com/Jacobferdinand/React-Three-Fiber-Webflow

