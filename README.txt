IRL PRO HUD LIMPO — versão com preparação para YouTube Live Chat

Base preservada: localização/GPS, velocidade, horário, temperatura, Arial em negrito e posições originais do HUD.

Alterações desta versão:
- Hora + temperatura permanecem no HUD original; o bloco fica livre para posicionamento acima do chat.
- Chat do YouTube preparado para aparecer no canto inferior esquerdo.
- Nenhum logo, marca d'água ou Netlify.
- Compatível com hospedagem estática, incluindo Cloudflare Pages.

CANAL CONFIGURADO:
https://youtube.com/@explorandofelicidadesofc

ATIVAR O CHAT DE UMA LIVE:
1. Publique o site no Cloudflare Pages.
2. Pegue o ID do vídeo da live no YouTube (ex.: https://www.youtube.com/watch?v=ABC123 -> ABC123).
3. Abra o HUD adicionando ?video=ID_DA_LIVE ao endereço do site.
   Exemplo: https://seu-site.pages.dev/?video=ABC123
4. O chat será carregado automaticamente no canto inferior esquerdo.

Observação: o link do canal, sozinho, não fornece de forma confiável o ID da transmissão atual para um site estático sem usar a API do YouTube. Por isso a versão está pronta para receber o ID da live pela URL, sem alterar o HUD original.
