# Alurit Tech — Site (Jekyll + GitHub Pages)

Site institucional simples, pronto para publicar no GitHub Pages.

## Publicar no GitHub Pages
1. Crie o repositório (p.ex. `alurit-site`).
2. Faça upload de todos os arquivos deste pacote na branch `main`.
3. Vá em **Settings → Pages → Build and deployment**:
   - Source: `Deploy from a branch`
   - Branch: `main` e `/(root)`
4. Aguarde o build do Pages. O site ficará acessível em `https://SEU-USUARIO.github.io/` ou `https://SEU-USUARIO.github.io/alurit-site/`.

### Domínio customizado
- Crie um arquivo `CNAME` na raiz contendo:
  ```
  alurit.com.br
  ```
- No provedor DNS, aponte:
  - Registros A para: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
  - (Opcional) `www` como CNAME para `SEU-USUARIO.github.io`
- Em **Settings → Pages**, marque **Enforce HTTPS**.

## Desenvolver localmente
- Opcional: instale Ruby e Jekyll para rodar local:
  ```bash
  bundle install
  bundle exec jekyll serve
  ```

## Personalização
- Imagens em `assets/img/`
- Estilos em `assets/css/style.css`
- Layout em `_layouts/default.html`
- Cabeçalho e rodapé em `_includes/`