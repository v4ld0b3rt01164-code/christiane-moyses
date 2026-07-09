# Deploy — Cloudflare Pages

## URLs

- **Produção:** https://christiane-moyses.pages.dev
- **Repo:** https://github.com/v4ld0b3rt01164-code/christiane-moyses

## Stack

- **Framework:** Astro 5 (static output)
- **Build:** `npm run build` → `dist/`
- **Deploy:** `npx wrangler pages deploy dist --project-name=christiane-moyses`

## Deploy manual

```bash
npx astro build
npx wrangler pages deploy dist --project-name=christiane-moyses
```

É necessário ter a env var `CLOUDFLARE_API_TOKEN` configurada.

## CI/CD (GitHub Actions)

Workflow criado em `.github/workflows/deploy.yml`. Secret `CLOUDFLARE_API_TOKEN` configurado no repo.

Para ativar, o token GitHub precisa do scope `workflow`:

```bash
gh auth refresh -h github.com -s workflow
git push
```
