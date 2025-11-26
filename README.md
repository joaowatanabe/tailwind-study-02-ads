# Estudos Tailwind — Projeto 02

**Overview**

Este é um projeto para estudar e aperfeiçoar habilidades de front-end, com foco no Tailwind CSS. O objetivo é experimentar utilitários, configurar um fluxo de trabalho simples e praticar componentes responsivos e acessíveis.

**Objetivos do Projeto**

- **Aprender**: entender a filosofia utility-first do Tailwind.
- **Configurar**: criar um fluxo de trabalho de desenvolvimento com `input.css` e `output.css`.
- **Praticar**: construir componentes responsivos e layouts usando classes do Tailwind.

**Estrutura do Projeto**

- **`index.html`**: ponto de entrada do projeto.
- **`src/css/input.css`**: arquivo de entrada com diretivas do Tailwind (ex.: `@tailwind base; @tailwind components; @tailwind utilities;`).
- **`src/css/output.css`**: arquivo gerado pelo build do Tailwind (não comitar se for gerado automaticamente).
- **`img/`**: imagens usadas no projeto.
- **`package.json`**: scripts e dependências do projeto.

**Requisitos**

- Node.js (recomendado v16+)
- npm ou yarn

**Instalação Rápida**

No macOS (zsh), rode:

```bash
npm install
```

Se você ainda não instalou o Tailwind no projeto, pode adicionar com:

```bash
npx tailwindcss init -p
```

**Comandos úteis**

- Desenvolvimento (watch):

```bash
npx tailwindcss -i ./src/css/input.css -o ./src/css/output.css --watch
```

- Build para produção (minificado):

```bash
npx tailwindcss -i ./src/css/input.css -o ./src/css/output.css --minify
```

Sugestão de scripts em `package.json`:

```json
"scripts": {
	"dev": "npx tailwindcss -i ./src/css/input.css -o ./src/css/output.css --watch",
	"build": "npx tailwindcss -i ./src/css/input.css -o ./src/css/output.css --minify"
}
```

**Boas práticas**

- Use o modo JIT (Just-in-Time) do Tailwind para desenvolvimento rápido.
- Configure `content` no `tailwind.config.js` para incluir os caminhos corretos (`./index.html`, `./src/**/*.{html,js}`) e reduzir o tamanho do CSS final.
- Evite comitar o `output.css` se ele for gerado automaticamente; prefira gerar no CI ou localmente.

**Exercícios sugeridos**

- Recriar uma landing page simples usando utilitários do Tailwind.
- Implementar um componente de menu responsivo com acessibilidade (teclado e ARIA).
- Criar variações de tema com CSS variables e `@apply`.

**Recursos**

- Documentação oficial do Tailwind: https://tailwindcss.com/docs
- Guia de prática: artigos e exemplos na web (procure por "Tailwind components" e "Tailwind examples").

**Próximos passos**

- Adicionar scripts em `package.json` (se desejar).
- Configurar `tailwind.config.js` com o `content` correto.
- Começar a implementar componentes e commits pequenos para acompanhar a evolução.

---

Se quiser, eu posso:

- Atualizar `package.json` com os scripts sugeridos.
- Gerar um `tailwind.config.js` inicial com `content` configurado.
- Criar exemplos de componentes (ex.: navbar responsiva).
