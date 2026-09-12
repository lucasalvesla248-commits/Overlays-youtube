IRL PRO HUD — YOUTUBE LIVE CHAT REAL

Esta versão já está configurada para a live de teste enviada:
https://youtube.com/live/vA0P9ChPTpY?feature=share

IMPORTANTE
O chat real usa a YouTube Data API v3. O GitHub Pages não consegue esconder uma chave de API; por isso, a chave deve ser criada por você no Google Cloud e restringida ao domínio do seu GitHub Pages.

COMO CONFIGURAR
1. Crie/ative um projeto no Google Cloud.
2. Ative a YouTube Data API v3.
3. Crie uma API Key.
4. No Google Cloud, restrinja a chave por HTTP referrer ao seu domínio do GitHub Pages e limite a API à YouTube Data API v3.
5. No index.html, substitua:
   youtubeApiKey:'COLOQUE_SUA_CHAVE_DA_API_AQUI'
   pela sua chave.

A versão atual já contém o ID da sua live de teste:
   youtubeVideoId:'vA0P9ChPTpY'

ALTERNATIVA POR URL
Você também pode manter o arquivo sem editar e abrir:
https://SEU-USUARIO.github.io/SEU-REPO/?video=vA0P9ChPTpY&key=SUA_CHAVE

ATENÇÃO SOBRE LIVE PRIVADA
Uma transmissão marcada como PRIVADA não pode ser consultada normalmente por uma página pública usando apenas uma API key. Para este teste, coloque a transmissão como NÃO LISTADA (Unlisted) ou PÚBLICA enquanto estiver testando. Se você precisa obrigatoriamente manter a live PRIVADA, a solução correta é um backend com OAuth/autorização da sua conta do YouTube; eu posso preparar essa versão também.

FUNCIONAMENTO
- Descobre o liveChatId da transmissão automaticamente.
- Busca mensagens reais do chat.
- Mostra somente o nome do autor no HUD, mantendo o visual transparente.
- Não gera nomes/mensagens fictícios.
- Respeita o intervalo de polling informado pela API para reduzir consumo de cota.

A documentação oficial informa que liveChatMessages.list requer o liveChatId e que o liveChatId da transmissão é obtido a partir de liveBroadcast.snippet.liveChatId. O chat fica disponível enquanto o evento ao vivo está ativo.
