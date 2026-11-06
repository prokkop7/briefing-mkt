# Briefing Estratégico — MediaMorphix

Página de pré-diagnóstico comercial responsiva para clientes e prospects.

## Funcionalidades
- 7 etapas com progresso;
- perguntas objetivas, escolhas simples e múltiplas;
- análise indicativa de prioridades: atendimento, integração ou captação;
- resumo final personalizado;
- botão para copiar o diagnóstico;
- compartilhamento voluntário via WhatsApp (22) 99876-3570.

Não existe backend ou armazenamento automático. O formulário roda diretamente no navegador; o envio das respostas depende de ação voluntária da pessoa.

## Publicar no GitHub Pages
1. Abra **Settings → Pages** deste repositório.
2. Em **Build and deployment**, selecione **Deploy from a branch**.
3. Escolha a branch **main** e a pasta **/ (root)** e clique em **Save**.
4. Confira o endereço público: https://prokkop7.github.io/briefing-mkt/

Antes de compartilhar com clientes, teste em celular, confirme o número do WhatsApp e, se for incluir coleta automatizada, implemente política de privacidade, consentimento e controles de segurança.

**MediaMorphix — A melhor solução começa entendendo o que precisa mudar.**

## Nova identidade e integração n8n

Marca horizontal oficial em `assets/logo-horizontal.png` e paleta azul-marinho/champagne/marfim aplicada ao formulário.

O envio automático começa **desativado**. Para ativar, inserir a URL HTTPS pública de **produção** em `window.MEDIAMORPHIX_CONFIG.n8nWebhookUrl` no cabeçalho do HTML. O n8n precisa aceitar requisições POST JSON e CORS da origem `https://prokkop7.github.io`. A pessoa precisa marcar a autorização; não são transmitidos dados sem ela. Não usar credenciais privadas no HTML; para autenticação, rate limit e proteção anti-spam, usar um proxy seguro.
