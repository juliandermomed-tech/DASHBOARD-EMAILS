# Painéis de pedidos — Dermomed

- `index.html` — Pedidos dos e-mails transacionais (página inicial)
- `dados-comparativos.html` — Painel completo: Cupom Cliente DM, E-mails, Roleta e Consolidado

## Atualização automática (aba de e-mails)
1. Na planilha "Controle E-mails Loja Integrada — Pedidos": Arquivo → Compartilhar → Publicar na Web.
2. Escolha a PRIMEIRA aba e o formato "Valores separados por vírgula (.csv)" → Publicar → copie o link.
3. O link já está configurado nos dois arquivos (linha `var CSV_URL = ...`). Se publicar outra planilha, troque o link nessa linha.
4. Envie os arquivos para o GitHub.

A página lê a planilha ao abrir, a cada 5 minutos e quando alguém clica em "Atualizar agora". O botão "Abrir planilha" leva à planilha no Google Sheets. Se não conseguir, mostra os dados de 08/10/2026 guardados no arquivo.
Os pedidos novos precisam continuar na primeira aba da planilha.

## Publicar no GitHub Pages
Settings → Pages → Source: "Deploy from a branch" → branch `main`, pasta `/ (root)` → Save.

Atenção: publicar a planilha na Web deixa os dados dela (inclusive nomes de clientes) acessíveis a quem tiver o link do CSV, assim como o site do GitHub Pages.
