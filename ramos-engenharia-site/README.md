# Ramos Engenharia e Vistoria — Landing Page

Landing page institucional e de conversão da **Ramos Engenharia e Vistoria**
(L. Xavier Ramos LTDA), especializada em vistoria técnica de imóveis em
Campo Grande - MS e região.

## Estrutura

| Arquivo | Descrição |
| --- | --- |
| `index.html` | Página completa — HTML, CSS e JS em arquivo único, sem build |
| `assets/logo.svg` | Logotipo vetorizado, usa `currentColor` (herda a cor via CSS) |
| `assets/imagens-origem.txt` | URLs das imagens ainda hospedadas no CDN do site anterior |

## Publicação

Não há build nem dependências. Basta servir o `index.html` a partir da raiz
do domínio. Funciona em GitHub Pages, Netlify, Vercel ou hospedagem comum.

Para testar localmente:

```bash
python3 -m http.server 8000
```

## Pendências antes de ir ao ar

1. **Formulário sem back-end.** O atributo `action` do `<form>` está como
   `[URL_DO_SEU_FORMULARIO]`. Definir um endpoint (Formspree, Web3Forms ou
   o servidor próprio) antes de publicar.
2. **Imagens no CDN antigo.** As fotos ainda apontam para
   `static.wixstatic.com`. Baixar os arquivos listados em
   `assets/imagens-origem.txt`, colocá-los em `assets/img/` e trocar as URLs,
   para desacoplar a página da hospedagem anterior.

## Identidade visual

Paleta oficial da marca, aplicada como CSS custom properties:

| Cor | Hex | Uso |
| --- | --- | --- |
| Marrom | `#704F31` | Cor primária, títulos e botões |
| Oliva | `#4B5940` | Grafismo diagonal, ícones de confirmação |
| Creme | `#ECE1CD` | Fundos de seção |
| Terracota | `#AC764F` | Grafismo diagonal, rótulos e destaques |

Tipografia: **Jost** (títulos e rótulos) e **Karla** (texto corrido),
carregadas do Google Fonts.

A página respeita o tema claro e escuro do sistema do visitante.

## Contato da empresa

- WhatsApp: (67) 99958-3183
- E-mail: ramosengenhariaevistoria@gmail.com
- Instagram: [@ramosengenhariaevistoria](https://www.instagram.com/ramosengenhariaevistoria)
- Responsável técnica: Luana Ramos — CREA-MS 70573
