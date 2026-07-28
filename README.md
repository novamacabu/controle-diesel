# Controle de Diesel — Nova Macabu

Sistema de controle de abastecimento de diesel da Garagem de Conceição de Macabu, com previsão de estoque, programação de recebimentos, registro de abastecimentos da frota e exportação para Excel.

## Arquivos

| Arquivo | Função |
|---|---|
| `index.html` | Aplicação completa (login, painel, previsão, gráfico, exportação) |
| `manifest.json` | Configuração do PWA (instalar como app no celular/computador) |
| `sw.js` | Service worker — cache e funcionamento offline |
| `icon-192.png` / `icon-512.png` | Ícones do app (logo Nova Macabu) |
| `apple-touch-icon.png` | Ícone para iPhone/iPad |

## Como publicar no GitHub Pages

1. Crie um repositório no GitHub (ex.: `diesel-nmb`).
2. Envie **todos os arquivos desta pasta** para a raiz do repositório.
3. Em **Settings → Pages**, selecione a branch `main` e a pasta `/ (root)`.
4. Aguarde 1–2 minutos e acesse `https://SEU_USUARIO.github.io/diesel-nmb/`.

## Acesso

Restrito aos administradores **Admin** e **Ricardo** — mesmas credenciais (usuário e senha) do sistema de Escala da Agência NMB.

## Instalar como aplicativo

- **Android/Chrome:** abra o site → menu ⋮ → "Instalar aplicativo".
- **iPhone/Safari:** abra o site → Compartilhar → "Adicionar à Tela de Início".
- **Computador (Chrome/Edge):** ícone de instalação na barra de endereço.

## Observações

- Os dados ficam salvos no navegador do dispositivo (localStorage). Cada dispositivo tem sua própria base — use **Exportar Excel** para consolidar/backup.
- Para trocar as senhas, gere o SHA-256 da nova senha e substitua o hash correspondente em `ADMIN_ACCOUNTS` no `index.html`.
- Ao atualizar o site, incremente o nome do cache em `sw.js` (`diesel-nmb-v2`, `v3`…) para forçar a atualização nos aparelhos.
