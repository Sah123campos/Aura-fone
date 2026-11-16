# AURA One

Landing page de produto em português do Brasil, com visual escuro, fone 3D procedural e interações responsivas.

## Executar

O site está inteiramente em `index.html`, na raiz. Não exige instalação ou build.

Para testar com um servidor local:

```sh
python3 -m http.server 3000
```

Abra `http://localhost:3000`. É necessário acesso à internet para carregar os CDNs, as fontes e os retratos.

## Personalizar

1. **Marca e textos:** ajuste `CONFIG.brand`, `CONFIG.product`, `CONFIG.copy` e os textos das seções no HTML.
2. **Cores e fontes:** edite as variáveis CSS em `:root` e os acabamentos em `CONFIG.colors`.
3. **Objeto 3D:** altere `createHeadphones()`, seus materiais e as posições das peças.
4. **Oferta:** configure `price`, `originalPrice`, `installments` e `campaignEnd` em `CONFIG`.
5. **Compra e contato:** preencha `CONFIG.checkoutUrl` com o endereço HTTPS do checkout e `CONFIG.whatsapp` com país, DDD e número, somente dígitos.

Ao publicar em um domínio próprio, acrescente a meta `og:url` com a URL definitiva e atualize os metadados de SEO.

## Recursos

- Three.js com materiais físicos e environment map gerado em memória.
- Rotação por arraste e teclado, parallax, acabamentos e visualização das peças separadas.
- GSAP, ScrollTrigger e Lenis via CDN.
- Pós-processamento reduzido no celular, limite de pixel ratio e respeito a `prefers-reduced-motion`.
- FAQ, contadores, resumo de seleção e barra de compra móvel.
- Ilustração de reserva quando WebGL não está disponível.

## Conteúdo demonstrativo

AURA One é uma marca e um produto fictícios. Especificações, oferta, comparações e depoimentos são ilustrativos; substitua-os por informações verificadas antes de operar comercialmente. Os retratos são de banco de imagens. Com os links de compra e contato vazios, a página mostra diálogos demonstrativos, sem pagamentos ou envio de pedidos.
