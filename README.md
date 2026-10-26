# misomoon proxy templates

One-click proxies that serve [misomoon](https://misomoon.com)'s tracker and forward its
events from your own domain, so ad blockers that drop third-party analytics leave them
alone.

| Platform | Deploy | Then add your subdomain under |
|---|---|---|
| Cloudflare Workers | [![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/jackzard/misomoon-proxy/tree/main/proxy-cloudflare) | Worker → Settings → Domains & Routes |
| Vercel | [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/jackzard/misomoon-proxy/tree/main/proxy-vercel&project-name=misomoon-proxy&repository-name=misomoon-proxy) | Project → Settings → Domains |

Then load the tracker from that subdomain:

```html
<script defer src="https://stats.example.com/m.js?s=your-site"></script>
```

Each folder's README has the details, and [the custom domain
guide](https://docs.misomoon.com/proxy) covers every way to proxy misomoon.

This repository mirrors `templates/` in the misomoon repository. MIT license.
