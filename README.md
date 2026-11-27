# klovar.cc

Klovar's personal site.

Hosted on GitHub Pages. `index.html` is the landing page. `404.html` is a simple
not-found page for unknown paths. `.nojekyll` disables Jekyll processing.

## Setup

### 1. GitHub repo
Create a repo named `klovar.cc` under the `Klovar-cc` account and push this folder:

```bash
git remote add origin https://github.com/Klovar-cc/klovar.cc.git
git push -u origin main
```

### 2. Enable GitHub Pages
Repo → Settings → Pages → Source: `Deploy from a branch`, branch `main` / root.
The `CNAME` file already sets the custom domain to `klovar.cc`.

### 3. DNS (at your domain registrar for klovar.cc)
Point the apex domain at GitHub Pages:

| Type  | Name | Value           |
|-------|------|-----------------|
| A     | @    | 185.199.108.153 |
| A     | @    | 185.199.109.153 |
| A     | @    | 185.199.110.153 |
| A     | @    | 185.199.111.153 |
| AAAA  | @    | 2606:50c0:8000::153 |
| AAAA  | @    | 2606:50c0:8001::153 |
| AAAA  | @    | 2606:50c0:8002::153 |
| AAAA  | @    | 2606:50c0:8003::153 |
| CNAME | www  | klovar-cc.github.io |

After DNS propagates, enable **Enforce HTTPS** in the Pages settings.
