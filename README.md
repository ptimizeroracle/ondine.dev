# ondine.dev

Landing page for [Ondine](https://github.com/ptimizeroracle/ondine). A prompt is a column.

## Development

```bash
# Preview locally
npx serve src

# Or just open src/index.html in a browser
```

## Deployment

Auto-deploys to [Render](https://render.com) on push to `main`. Config lives in [`render.yaml`](./render.yaml) at the repo root: static site, publish dir `./src`, SPA-style rewrites to `/index.html`, PR previews enabled, long cache on `/assets/*`, secure default headers.

### First-time setup

1. On Render: **New → Blueprint**, point at this repo. Render picks up `render.yaml` automatically.
2. Add the custom domain `ondine.dev` in the Render dashboard and follow the DNS instructions (ALIAS or CNAME to the Render hostname).
3. Disable any previous Cloudflare Pages / Vercel deployment that points at the same domain.

## Links

- [Ondine SDK](https://github.com/ptimizeroracle/ondine)
- [Documentation](https://docs.ondine.dev)
- [PyPI](https://pypi.org/project/ondine/)
