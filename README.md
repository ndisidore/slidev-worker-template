# Slidev + Cloudflare Workers Template

A template for creating [Slidev](https://github.com/slidevjs/slidev) presentations deployed on [Cloudflare Workers](https://workers.cloudflare.com/) using [Workers Assets](https://developers.cloudflare.com/workers/static-assets/).

## Features

- ✨ **Slidev** - Presentation slides for developers
- ⚡ **Cloudflare Workers** - Edge deployment with global CDN
- 📦 **Workers Assets** - Efficient static asset serving
- 🎨 **TypeScript** - Type-safe Worker configuration
- 🚀 **Fast Development** - Local development with `wrangler dev`

## Development

### Local Slidev Development

To start the Slidev development server:

```bash
npm install
npm run dev
```

Visit <http://localhost:3030> to see your presentation.

### Local Workers Development

To test the Workers deployment locally:

```bash
npm run build              # Build Slidev presentation
npm run wrangler:dev       # Start local Workers server
```

### Deployment

Deploy to Cloudflare Workers:

```bash
npm run wrangler:deploy
```

## Project Structure

- `slides.md` - Your presentation content
- `src/index.ts` - Cloudflare Worker script
- `wrangler.jsonc` - Workers configuration
- `dist/` - Built static assets (generated)

## Customization

Edit the [slides.md](./slides.md) to customize your presentation content.

Learn more about Slidev at the [documentation](https://sli.dev/).
