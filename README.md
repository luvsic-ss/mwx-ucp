# UCP agent profile

This public profile declares the catalog capabilities used by the toulove-product-tracker skill.

Use the CDN URL (serves `application/json`):

```text
https://cdn.jsdelivr.net/gh/luvsic-ss/mwx-ucp@305088af7c132de2a5f10850e6957c1da4af31f4/ucp-agent.json
```

Use it with:

```bash
python scripts/tracker.py collect --ucp \
  --url "https://toulove-store.jp/products/<handle>" \
  --ucp-profile "https://cdn.jsdelivr.net/gh/luvsic-ss/mwx-ucp@305088af7c132de2a5f10850e6957c1da4af31f4/ucp-agent.json" \
  --output runs/ucp-001
```

The profile is public capability metadata; never put tokens or secrets here.

GitHub Raw (`raw.githubusercontent.com`) serves this file as `text/plain`; the store rejects it with `Invalid content type`. Use jsDelivr, GitHub Pages, or another host that returns `application/json`.
