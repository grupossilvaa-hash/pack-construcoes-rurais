# Pack Construções Rurais — página de vendas

Landing estática de venda do **Pack Construções Rurais**: acervo de +400 projetos de
construção rural (galpão, curral, galinheiro, baia, silo, área de ordenha, casa de
máquinas, depósito de ração, bebedouro e cocho) com planta baixa, corte, medidas reais e
**lista de material quantificada**.

- **Avatar:** pequeno e médio produtor rural, sitiante e dono de chácara (30–60 anos).
- **Dor:** sem projeto na mão, quem decide o custo da obra é o empreiteiro.
- **Mecanismo:** a lista de material quantificada de cada projeto devolve o controle do
  orçamento pra quem paga a obra.

## Stack

HTML + CSS + JS puros, arquivo único (`index.html`). Sem build, sem dependência, sem
servidor — dá pra abrir o arquivo direto no navegador. Imagens em `img/`.

Gerada a partir de `padrao-paginas-de-vendas/base/index.html` (mesma estrutura, seletores
e scripts do padrão da linha; mudam só copy, imagens, fontes e paleta).

- **Fontes:** Archivo (display) + Source Sans 3 (texto), via Google Fonts.
- **Paleta:** verde-mata `#1F5F3E` (primária) · laranja `#D97B29` (CTA) ·
  teal `#10695F` (sucesso) · vermelho `#E2635C` (alerta).

## Planos e checkout

| Plano | Preço | Campanha (UTM) |
|---|---|---|
| Completo | R$ 27,90 (de R$ 47,00) | `pcr-completo` |
| Básico | R$ 19,90 | `pcr-basico` |
| Downsell (exit-intent) | R$ 19,90 | `pcr-downsell` |

> ⚠️ **Pendente:** as três URLs de checkout estão como `SKU-COMPLETO`, `SKU-BASICO` e
> `SKU-DOWNSELL`. Trocar pelos SKUs reais da Kiwify antes de subir campanha.
> O `window.pixelId` da UTMify também está como placeholder.
> O bloco do Meta Pixel está vazio, aguardando o código.

## Onde publica

Vercel, via Git. Todo push na `main` publica em produção.
