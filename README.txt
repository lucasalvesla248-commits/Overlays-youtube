IRL Pro — YouTube Chat SEM Google Apps Script

1. Abra index.html em um editor de texto.
2. Troque COLE_SUA_CHAVE_AQUI pela sua chave da YouTube Data API v3.
3. Se quiser outra live, use ?video=ID_DA_LIVE no endereço.
4. Publique o index.html no GitHub Pages.
5. No IRL Pro: Overlays > Web Overlays > New Web Overlay e use a URL do GitHub Pages.

IMPORTANTE: como a chave fica no navegador, restrinja a chave no Google Cloud:
- Application restrictions: Websites (HTTP referrers)
- API restrictions: YouTube Data API v3
- Referrer: https://lucasalvesla248-commits.github.io/Overlays-youtube/*

A página usa a YouTube Data API v3 diretamente. Não usa Google Apps Script.
