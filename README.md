# Top Obra Casa e Construção — site de apresentação

Site estático (HTML + CSS + JS, sem build). Boa Vista/RR · Av. João Alencar, 1437 — Cauamé.

## Estrutura
```
index.html          → página completa
assets/img/         → logos, fotos da loja, banners, favicon, imagem de compartilhamento (og.jpg)
assets/video/       → vídeos (loja, entrega, oferta)
vercel.json         → cache dos arquivos estáticos
```
Bibliotecas carregadas por CDN: GSAP 3.12.5 + ScrollTrigger e Three.js r128 (cdnjs). Fontes: Archivo e Figtree (Google Fonts).

## Publicar no GitHub + Vercel
1. Crie um repositório novo no GitHub (ex.: `topobra-site`).
2. Envie o conteúdo desta pasta (a pasta com o `index.html` na raiz):
   - Pelo site: **Add file → Upload files**, arraste tudo e clique em **Commit changes**; ou
   - Pelo terminal:
     ```bash
     git init
     git add .
     git commit -m "Site Top Obra"
     git branch -M main
     git remote add origin https://github.com/SEU-USUARIO/topobra-site.git
     git push -u origin main
     ```
3. Em vercel.com → **Add New… → Project** → importe o repositório.
4. Framework Preset: **Other**. Build Command e Output Directory: deixe em branco. Clique em **Deploy**.
5. Domínio próprio: Vercel → Project → **Settings → Domains**.

## Editar
- Telefone do WhatsApp: no `index.html`, procure `const WA='5595991250790'`.
- Trocar fotos: substitua os arquivos em `assets/img/` mantendo o mesmo nome.
- Depois de publicar, troque `og:image` por uma URL completa (ex.: `https://seudominio.com.br/assets/img/og.jpg`) para a prévia aparecer certinho no WhatsApp.
