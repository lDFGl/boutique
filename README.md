# All Boutique — protótipo visual de e-commerce de joias

Esta primeira entrega é uma **visualização parcial e interativa** da loja, feita em HTML/CSS/JS puro para facilitar prévia rápida via GitHub Pages.

## O que está incluído
- Identidade visual All Boutique: rosa perolado, rosé gold e monograma AB em SVG.
- Layout responsivo para desktop e mobile.
- Home de marca com banner, benefícios, vitrine, seção editorial e redes sociais.
- Filtros de categoria.
- Cards de produto com imagens e preços demonstrativos.
- Sacola lateral funcional (quantidade e total na sessão).
- Painel ADMIN demonstrativo com indicadores e pedidos fictícios.
- Avisos claros de que os dados e o painel são de demonstração.

## Limitações atuais (não é produção)
- Sem banco de dados ou persistência de carrinho.
- ADMIN sem autenticação: somente prévia visual.
- Checkout/pagamento, Correios, rastreio, chat, cadastro, login e gestão real não estão conectados.
- Métricas e conteúdo de produtos são demonstrativos.
- Redes sociais precisam ser configuradas com os perfis reais.
- Imagens e fontes carregam de provedores externos.

## Publicar no GitHub Pages com GitHub Actions
O workflow `.github/workflows/deploy-pages.yml` já está configurado para publicar automaticamente a cada `push` na branch `main`, além de permitir execução manual.

1. Abra **Settings → Pages** neste repositório.
2. Em **Build and deployment → Source**, selecione **GitHub Actions** (não use `Deploy from a branch`).
3. Faça um novo commit na branch `main` ou abra **Actions → Deploy All Boutique to GitHub Pages → Run workflow** para iniciar manualmente.
4. Acompanhe as etapas `build` e `deploy` na aba **Actions**.
5. Após a primeira publicação, o endereço esperado é `https://ldfgl.github.io/boutique/`.

**Observação:** a primeira publicação depende de selecionar GitHub Actions em Settings → Pages. O workflow não configura essa opção automaticamente.

## Próximas etapas
1. Definir identidade visual e nome real da marca.
2. Conectar Supabase (Postgres, Auth, Storage e políticas RLS).
3. Criar ADMIN autenticado com autorização server-side.
4. Implementar catálogo e estoque persistidos.
5. Integrar gateway de pagamento com webhooks.
6. Integrar Correios para CEP, cotação, prazos e rastreio conforme contrato/API.
7. Implementar suporte, avaliações e moderação.
8. Adequar políticas, consentimentos e processos à LGPD.
