# CV + Wiki técnica — GitHub Pages

Este pacote contém uma cópia do CV atualizado (sem a experiência de formador em destaque) e uma Wiki com o mesmo estilo visual.

## Publicar

1. Fazer cópia de segurança do repositório atual.
2. Copiar **todo o conteúdo** desta pasta para a raiz do repositório usado no GitHub Pages, preservando as subpastas `wiki/` e `assets/`.
3. Confirmar que a raiz do site tem `index.html` e que `wiki/index.html` abre corretamente.
4. Publicar as alterações com um commit. Não colocar ficheiros de autenticação no repositório.

> Se o GitHub Pages estiver configurado para publicar a partir de `/docs` em vez da raiz, colocar estes ficheiros na pasta de publicação configurada.

## Adicionar capturas reais

Os ficheiros SVG em `assets/img/wiki/` são **marcadores de posição**, não capturas reais.

Opção simples: guardar uma imagem sanitizada em `assets/img/wiki/proxmox-real.webp` e, em `wiki/proxmox.html`, mudar `src="../assets/img/wiki/proxmox.svg"` para `src="../assets/img/wiki/proxmox-real.webp"`. Atualizar também a legenda e o atributo `alt` para descrever o conteúdo real.

Repetir para Homarr, Home Assistant, pfSense, monitorização, radioamadorismo e fotografia. Preferir WebP/JPEG para fotografias e PNG/WebP para capturas de interface.

## Segurança e privacidade

Antes de publicar, ocultar IPs e domínios públicos ou internos relevantes, MACs, números de série, nomes pessoais, tokens, chaves, sessões iniciadas, códigos QR e dados de dispositivos. Nunca publicar ficheiros de backup ou configurações com credenciais. Evitar capturas que mostrem interfaces administrativas acessíveis e dados de localização detalhados.

## Conteúdo futuro

- Substituir marcadores de posição por capturas reais dos serviços.
- Adicionar artigos e imagens do site de radioamadorismo e de fotografia, com origem indicada.
- Documentar um ou dois casos reais por página: objetivo, problema, solução e resultado.
- Manter a atividade de formador fora do CV e Wiki enquanto estiver em testes.

## Ficheiros

- `index.html` — CV e ligação para a Wiki.
- `wiki/index.html` — índice da Wiki.
- `wiki/*.html` — páginas de cada área.
- `assets/css/wiki.css` — estilo partilhado pelas páginas da Wiki.
- `assets/img/wiki/*.svg` — placeholders e diagrama genérico.

Não necessita de servidor, base de dados ou dependências externas; funciona em GitHub Pages.

## Sites pessoais integrados
- https://ct1jqj.eu/ — radioamadorismo e eletrónica, com ligações diretas aos artigos selecionados.
- https://miragens.org/ — fotografia, artigos e galerias, com ligações diretas.
- As imagens nos blocos de galeria são provisórias. A Wiki não republica integralmente os artigos.
