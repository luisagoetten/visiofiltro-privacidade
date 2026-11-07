---
title: Política de privacidade do VisioFiltro
lang: pt-BR
---

# Política de privacidade — VisioFiltro

| | |
|---|---|
| **Aplicativo** | VisioFiltro (`com.visiofitro.app`) |
| **Documentos** | Política de privacidade — v1.3 |
| **Vigência** | 31 de outubro de 2026 |
| **Última revisão** | 7 de novembro de 2026 |
| **Contato** | [girassolestudiodigital@gmail.com](mailto:girassolestudiodigital@gmail.com) |

O VisioFiltro é um aplicativo Android que aplica uma camada de cor translúcida sobre a tela. Esta política explica, de forma objetiva, **quais dados** o aplicativo e seus provedores tratam, **para que** servem e **como** isso acontece.

---

## Resumo executivo

| Pergunta | Resposta |
|---|---|
| O desenvolvedor mantém servidor, conta ou backend? | **Não.** Nenhum dado pessoal chega ao desenvolvedor. |
| O aplicativo envia preferências do usuário? | **Não.** Cor, tom, intensidade e desbloqueios ficam no aparelho. |
| Existe publicidade? | **Sim, apenas na versão gratuita** — um banner do Google AdMob na tela principal e um anúncio opcional de apoio, sem recompensa. O **VisioFiltro Completo** remove ambos. |
| Existe venda ou aluguel de dados? | **Não.** |
| O conteúdo da tela é enviado a alguém? | **Não.** O app não captura, lê nem transmite o conteúdo de outros aplicativos. |

Documentos relacionados: [Termos de uso](termos_de_uso.md) e [Permissões do VisioFiltro](permissoes.md).

---

## 1. Preferências locais

A cor selecionada, o tom claro ou escuro, a intensidade e o estado de desbloqueio das cores e do Completo são armazenados apenas no seu aparelho, em preferências locais do aplicativo (Android DataStore sob o sandbox do Android).

- **Envio ao desenvolvedor:** nenhum.
- **Retenção:** até você desinstalar o app ou limpar os dados do aplicativo.
- **Backup do Android:** desativado para os dados do app.

O app não acessa localização do Android, contatos, câmera, microfone, arquivos do usuário ou histórico de uso. O SDK de anúncios pode estimar a localização aproximada a partir do IP, sem pedir a permissão de localização do Android — detalhado na Seção 3.

## 2. Permissão de sobreposição

A permissão especial **“Sobrepor a outros apps”** (`SYSTEM_ALERT_WINDOW`) é usada exclusivamente para desenhar a camada de cor escolhida sobre a tela.

- O VisioFiltro **não lê, grava ou envia** o conteúdo de outros aplicativos.
- Não captura a tela e **não usa serviços de acessibilidade**.
- O pedido é feito com explicação na tela do app e concluído **na tela oficial do Android** (Configurações → Sobrepor a outros apps), jamais por janela do próprio app.
- Pode ser revogada a qualquer momento nas configurações do aparelho.

A finalidade, o pedido e os caminhos de revogação estão detalhados em [Permissões do VisioFiltro](permissoes.md).

## 3. Publicidade (Google AdMob / GMA Next-Gen)

A versão gratuita exibe um banner e oferece um anúncio opcional de apoio, sem recompensa, fornecidos pelos SDKs do **Google Mobile Ads Next-Gen** e do **Google AdMob**. Conforme a página de Data disclosure do Google para esse SDK, ele coleta e compartilha automaticamente, com a Google e com parceiros de anúncios:

| Categoria de dados | Exemplos | Finalidades |
|---|---|---|
| Endereço IP | Endereço usado pelas conexões do SDK | Publicidade, análise, prevenção a fraude |
| Interações com o produto | Abertura do app, toques, visualizações de vídeo | Publicidade, análise |
| Informações de diagnóstico | Tempo de inicialização, falhas, consumo de energia | Análise, melhoria do serviço |
| Identificadores de dispositivo e conta | ID de publicidade Android, app set ID, identificadores de contas conectadas ao dispositivo (quando aplicável) | Publicidade, prevenção a fraude |

Esse tratamento é feito pelo Google, transmitido por TLS e regido pela política de privacidade e pelos termos de tecnologias de publicidade do Google:

- https://policies.google.com/privacy
- https://policies.google.com/technologies/ads
- Página de Data disclosure do GMA Next-Gen: https://developers.google.com/admob/android/next-gen/privacy/play-data-disclosure

**Limites do anúncio no VisioFiltro:** o banner aparece apenas na tela principal. Não há anúncio no overlay, na notificação, no Tile de Configurações rápidas nem sobre outros apps. O anúncio de tela inteira só é carregado e exibido após toques explícitos na tela de apoio; nunca na abertura, ativação, desativação ou nos ajustes do filtro. O app funciona integralmente quando o anúncio não carrega. O app não envia o conteúdo da tela — sua cor, tom ou intensidade — ao Google.

## 4. Compras (Google Play Billing)

As compras de cores individuais e do VisioFiltro Completo são **únicas e opcionais**, processadas pela Google Play.

- O app usa a conexão à internet para consultar produtos, abrir o fluxo de compra e restaurar compras.
- O app recebe da Play Store a confirmação da compra, o identificador do produto e o estado do pedido (concluída ou pendente). **Não recebe** o número de cartão, dados bancários ou endereço de cobrança.
- O Google trata os dados de pagamento conforme a política de privacidade do Google.
- O app guarda localmente o identificador do produto desbloqueado; uma consulta bem-sucedida à Play Store atualiza esse cache, inclusive refletindo reembolsos.
- Reembolsos, cobranças e disputas seguem as regras da Google Play. O desenvolvedor não processa dados de cartão nem mantém histórico de pagamentos em servidor.

## 5. Consentimento e controles

- Onde exigido (EEE, Reino Unido e Suíça), o app apresenta a mensagem de consentimento do **Google UMP** antes de solicitar anúncios.
- Você pode revisar ou alterar suas escolhas em **“Opções de privacidade”** no app, quando disponível.
- O **ID de publicidade** pode ser redefinido ou excluído nas configurações do Android (Configurações → Privacidade → Anúncios). Ao excluí-lo, o app recebe zeros.
- Se você não consentir, os anúncios podem não ser exibidos; **todas as funções do filtro continuam disponíveis**.

O VisioFiltro não é direcionado a crianças (Seção 8); nenhuma opção separada de tratamento como público infantil é aplicável.

## 6. Notificações

A notificação do filtro é gerada localmente para informar que a camada está ativa e oferecer a ação “Desligar”. Na versão gratuita, se as notificações estiverem habilitadas, o Android pode exibir um convite local de apoio a cada três dias. Tocar no convite abre a tela de apoio, onde o anúncio só é solicitado por ação explícita. É possível desativar o convite nas configurações de notificações do Android. As notificações não contêm anúncios e não são enviadas por servidor.

## 7. Compartilhamento e registro

- O desenvolvedor **não vende, aluga ou compartilha** dados pessoais — não há para quem compartilhar, pois o app não tem backend, analytics ou SDK de relatório de falhas.
- Provedores envolvidos: **Google Play** (processamento de compras) e **Google AdMob / GMA Next-Gen** (publicidade), salvo conforme suas próprias políticas.

## 8. Segurança, retenção e direitos

| Tema | Como funciona |
|---|---|
| Dados sob controle do desenvolvedor | Nenhum — não há servidor |
| Preferências locais | No aparelho, sob sandbox Android; removidas ao desinstalar ou limpar dados |
| Histórico de compras | Associado à conta do Google Play (fonte: Google) |
| Dados de publicidade | Regidos pelas políticas e prazos do Google |
| Localização, contatos, arquivos | Nunca solicitados pelo app |
| Crianças | O VisioFiltro não é direcionado a crianças e não coleta intencionalmente dados de crianças |
| Pedidos GDPR/LGPD | Não há dados do usuário sob controle do desenvolvedor; pedidos sobre compras → canais da Google Play; sobre publicidade → controles do Google e do Android |

## 9. Alterações

Esta política pode ser atualizada para refletir mudanças no aplicativo, nos provedores ou na legislação. A data da vigência e a última revisão ficam no topo desta página e na tela de privacidade do app. Mudanças relevantes serão destacadas antes de entrarem em vigor.
