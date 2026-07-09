# Deploy automático — GitHub → Cloudflare Pages

O workflow de CI/CD está criado em `.github/workflows/deploy.yml` e o
secret `CLOUDFLARE_API_TOKEN` está configurado no repositório.

Para ativar o deploy automático no push, é necessário:

1. Atualizar o token do GitHub CLI com scope `workflow`:
   ```
   gh auth refresh -h github.com -s workflow
   ```
   (Isso abre o navegador para autorização interativa)

2. Fazer push do commit com o workflow:
   ```
   git push
   ```

Enquanto isso, deploys manuais podem ser feitos com:
```
npx wrangler pages deploy dist --project-name=christiane-moyses
```

Após o push do workflow, qualquer commit na branch `master` acionará
deploy automático no Cloudflare Pages via GitHub Actions.
