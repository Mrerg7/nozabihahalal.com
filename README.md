# nozabihahalal.com

Sister site to [nozabiha.com](https://nozabiha.com/), [nozabihahalal.com](https://nozabihahalal.com/), [islamophobe.me](https://islamophobe.me/), and [industrialterrorism.com](https://industrialterrorism.com/).

Static Astro site on Cloudflare Workers static assets. Free plan.

## Deploy

```bash
npm install
npm run deploy
```

Then in the Cloudflare dashboard, attach the custom domain `nozabihahalal.com` to the worker `nozabihahalal-comv2`.

Workers & Pages → Create → Import this GitHub repo also works:

- Build command: `npm run build`
- Deploy command: `npx wrangler deploy`
- Output lives in `dist/` and is bound as the `ASSETS` fetcher

`www.nozabihahalal.com` and `http` on the apex redirect to `https://nozabihahalal.com/`.
