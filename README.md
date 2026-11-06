# UCP agent profile

This public profile declares the catalog capabilities used by the toulove-product-tracker skill.

Raw URL after publishing:

```text
https://raw.githubusercontent.com/<owner>/<repo>/main/ucp-agent.json
```

Use it with:

```bash
python scripts/tracker.py collect --ucp \
  --url "https://toulove-store.jp/products/<handle>" \
  --ucp-profile "https://raw.githubusercontent.com/<owner>/<repo>/main/ucp-agent.json" \
  --output runs/ucp-001
```

The profile is public capability metadata; never put tokens or secrets here.
