# Life Pass Filter — Plugins

Source of the Life Pass Filter plugin page, served with GitHub Pages.

## Add or update a plugin

Edit the `PLUGINS` list at the top of the `<script>` block in `index.html`:

```js
{
  name: "Facet", repo: "LPF_Facet", added: "2026-11-12", version: "0.1",
  status: "beta",            // "released" | "beta" | "soon"
  blurb: "One or two sentences.",
  formats: ["VST3", "AU"], platforms: ["Mac", "Windows"],
  files: { Mac: "Facet-macOS.zip", Windows: "Facet-Windows.zip" }
}
```

`files` are the asset names attached to each GitHub Release of the plugin repo.
Download buttons always point to the latest release, so publishing a new release
updates the site automatically. The plugin repo must be public.

Donation links are set in `DONATE` in the same block.
