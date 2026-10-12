# Políticas públicas — BMS Prisma

Páginas estáticas exigidas pelo Google Cloud para publicar a tela de consentimento OAuth
do aplicativo interno **“Backup do parque”** (uma configuração do
[rclone](https://rclone.org) que envia backups dos servidores da BMS Prisma ao Google Drive).

- [`privacidade.html`](privacidade.html) — Política de Privacidade
- [`termos.html`](termos.html) — Termos de Serviço

## Por que este repositório é público

O Google exige que a política de privacidade e os termos de serviço de um aplicativo OAuth
estejam acessíveis publicamente, sem autenticação. É o único motivo. Não há código aqui.

## Por que o aplicativo pede tão pouco

O escopo solicitado é `https://www.googleapis.com/auth/drive.file`, que alcança **apenas os
arquivos criados pelo próprio aplicativo**. É uma restrição imposta pelo Google, não uma
promessa nossa: o restante do Drive é invisível para o token, mesmo para quem tenha acesso
administrativo à máquina onde ele está guardado.
