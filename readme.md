# Flavio Ricardo Icons Set API

Uma API leve e extremamente customizável para gerar grades e linhas de ícones dinamicamente em formato SVG. Ideal para exibir suas tecnologias, stacks e ferramentas diretamente no seu portfólio, landing pages ou no `README.md` do seu perfil do GitHub com uma única tag `<img>`.

---

## ✨ Funcionalidades

- 🧩 **Múltiplos Ícones:** Carregue um ou dezenas de ícones em uma única requisição.
- 📐 **Grade Flexível (`cols`):** Exiba os ícones em linha única ou quebre-os em colunas dinamicamente (ex: grades de 3x4, 4x3, 6x2).
- 📏 **Dimensões Ajustáveis (`s`):** Suporte nativo a múltiplos tamanhos baseados em `rem` (2rem, 3rem e 4rem).
- ↔️ **Espaçamento Controlado (`g`):** Ajuste o respiro entre os ícones da grade de forma simples.
- 🌓 **Modos Claro e Escuro (`m`):** Altere as cores de fundo e do ícone de acordo com o tema da sua página.
- 📦 **Fallback Inteligente:** Se um ícone tiver variações específicas para temas (ex: `aws-dark.svg` e `aws-light.svg`), a API carrega o correto. Se não, usa o arquivo neutro padrão.
- 📐 **Tipo de Container (`t`):** Ícones em formato quadrado, redondo ou com cantos arredondados.

---

## 🛠️ Como Usar (Exemplos)

Basta apontar o atributo `src` da sua tag `<img>` para a URL da API:
```https://flavioricardo.com.br/iconSetAPI/```

### 1. Linha única padrão (Fundo escuro, quadrado, tamanho 2rem)
```html
<img src="https://flavioricardo.com.br/iconSetAPI/?icon=html,css,js,php" alt="Minha Stack">
```
<img src="https://flavioricardo.com.br/iconSetAPI/?icon=html,css,js,php" alt="Minha Stack">

### 2. Grade de 4 colunas (Perfeito para o perfil do GitHub)
Se você passar 12 ícones e definir cols=4, a API gera automaticamente uma grade de 4x3 perfeitamente alinhada
```html
<img src="https://flavioricardo.com.br/iconSetAPI/?icon=html,css,js,php,mysql,laravel,python,aws,git,docker,linux,react&cols=4" alt="Minhas Techs">
```
<img src="https://flavioricardo.com.br/iconSetAPI/?icon=html,css,js,php,mysql,laravel,python,aws,git,docker,linux,react&cols=4" alt="Minhas Techs">

### 3. Totalmente customizado (Ícones grandes, redondos, modo claro e bem espaçados)

```html
<img src="https://flavioricardo.com.br/iconSetAPI/?icon=html,css,js&s=3&g=4&m=l&t=r" alt="Techs Redondas">
```
<img src="https://flavioricardo.com.br/iconSetAPI/?icon=html,css,js&s=3&g=4&m=l&t=r" alt="Techs Redondas">

### 4.Parâmetros Disponíveis
| Parâmetro | Descrição | Valores Aceitos | Padrão |
| :--- | :--- | :--- | :--- |
| `icon` | Lista de ícones separados por vírgula | `nome-do-arquivo` (sem o `.svg`) | *Obrigatório* |
| `cols` | Limite de ícones por linha (colunas) | Qualquer número inteiro maior que 0 | Total de ícones |
| `s` | Tamanho do container do ícone | `1` (2rem/32px), `2` (3rem/48px), `3` (4rem/64px) | `1` |
| `g` | Espaçamento (Gap) entre os ícones | `1` (0.25rem), `2` (0.5rem), `3` (1rem), `4` (1.5rem), `5` (2rem) | `1` |
| `m` | Modo (Tema de cores do container) | `d` (Escuro: Fundo `#1e1e1e`), `l` (Claro: Fundo `#f5f5f5`) | `d` |
| `t` | Tipo/Formato do container | `s` (Quadrado), `r` (Redondo), `rs` (Quadrado Arredondado) | `s` |

### 5. Relação de ícones disponível (em 29 de maio de 2026):
(em ordem alfabética)
| Imagem | código para uso | Nome | 
| :--- | :--- | :--- |
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=acrobat&m=d&s=2"> | acrobat | Adobe Acrobat | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=adobe-fonts-dark&m=d&s=2"> | adobe-fonts | Adobe Fonts | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=ae&m=d&s=2"> | ae | Adobe After Efects | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=ai&m=d&s=2"> | ai | Adobe Illustrator | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=antigravity&m=d&s=2"> | antigravity | Google Antigravity | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=apple&m=d&s=2"> | apple | Apple | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=au&m=d&s=2"> | au | Adobe Audition | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=c#&m=d&s=2"> | c# | C# | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=c++&m=d&s=2"> | c++ | C++ | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=c&m=d&s=2"> | c | C | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=ch&m=d&s=2"> | ch | Adobe Character Animator | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=chatgpt-dark&m=d&s=2"> | chatgpt | ChatGPT | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=claude&m=d&s=2"> | claude | Claude | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=css&m=d&s=2"> | css | CSS3 | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=deepseek&m=d&s=2"> | deepseek | DeepSeek | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=dn&m=d&s=2"> | dn | Adobe Dimension | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=docker&m=d&s=2"> | docker | Docker | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=ds&m=d&s=2"> | ds | Substance 3D Designer | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=dw&m=d&s=2"> | dw | Adobe Dreamweaver | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=figma&m=d&s=2"> | figma | Figma | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=fr&m=d&s=2"> | fr | Adobe Fresco | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=git&m=d&s=2"> | git | Git | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=github&m=d&s=2"> | github | GitHub | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=go&m=d&s=2"> | go | Go | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=html&m=d&s=2"> | html | HTML5 | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=ic&m=d&s=2"> | ic | Adobe InCopy | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=id&m=d&s=2"> | id | Adobe InDesign | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=js&m=d&s=2"> | js | JavaScript | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=laravel&m=d&s=2"> | laravel | Laravel | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=linux&m=d&s=2"> | linux | Linux | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=lr&m=d&s=2"> | lr | Adobe Lightroom | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=me&m=d&s=2"> | me | Adobe Media Encoder | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=ms&m=d&s=2"> | ms | Microsoft | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=mysql&m=d&s=2"> | mysql | MySQL | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=php-dark&m=d&s=2"> | php | PHP | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=pr&m=d&s=2"> | pr | Adobe Premiere | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=ps&m=d&s=2"> | ps | Adobe Photoshop | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=pt&m=d&s=2"> | pt | Substance 3D Painter | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=python&m=d&s=2"> | python | Python | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=ruby&m=d&s=2"> | ruby | Ruby | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=sa&m=d&s=2"> | sa | Substance 3D Sampler | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=sg&m=d&s=2"> | sg | Substange 3D Stager | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=ts&m=d&s=2"> | ts | TypeScript | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=vscode&m=d&s=2"> | vscode | Visual Studio Code | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=windows&m=d&s=2"> | windows | Microsoft Windows | 
| <img src="https://flavioricardo.com.br/iconSetAPI/?icon=xd&m=d&s=2"> | xd | Adobe XD | 