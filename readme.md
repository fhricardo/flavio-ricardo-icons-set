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

Basta apontar o atributo `src` da sua tag `<img>` para a URL onde a API está hospedada:

### 1. Linha única padrão (Fundo escuro, quadrado, tamanho 2rem)
```html
<img src="https://flavioricardo.com.br/iconSetAPI/?icon=html,css,js,php" alt="Minha Stack">
```

### 2. Grade de 4 colunas (Perfeito para o perfil do GitHub)
Se você passar 12 ícones e definir cols=4, a API gera automaticamente uma grade de 4x3 perfeitamente alinhada
```html
<img src="http://localhost/icon-set/?icon=html,css,js,php,mysql,laravel,python,aws,git,docker,linux,react&cols=4" alt="Minhas Techs">
```
<img src="http://localhost/icon-set/?icon=html,css,js,php,mysql,laravel,python,aws,git,docker,linux,react&cols=4" alt="Minhas Techs">
