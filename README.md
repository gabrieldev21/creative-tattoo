# 🎨 TattooCreativity

Aplicativo web desenvolvido com **Next.js** voltado à inspiração e criatividade para tatuagens. Artistas e entusiastas podem explorar ideias, referências e conceitos visuais.

O projeto segue boas práticas de arquitetura, organização modular e padrões de código limpo.

---

## 🚀 Tech Stack

- **Next.js** (App Router)
- **TypeScript**
- **React 18**
- **ESLint + Prettier**
- **Stitches** (estilização)
- **Axios / Fetch API**
- **Vercel** (deploy)
- **GitHub Actions** (CI/CD)

---

## 🏗️ Arquitetura e Estrutura de Pastas

A estrutura do projeto segue um padrão escalável e organizada, por exemplo:

```
src/
├── @types/         # Tipos globais e declarações
├── @interfaces/    # Interfaces de dados e contratos
├── @enums/         # Enumerações reutilizáveis
├── common/
│   ├── constants/  # Constantes globais e valores fixos
│   └── utils/      # Funções utilitárias
├── components/     # Componentes reutilizáveis
│   ├── ui/         # Elementos básicos (botões, inputs, etc.)
│   ├── layout/     # Estruturas (Header, Footer, etc.)
│   └── sections/   # Blocos específicos da página
├── hooks/          # Custom hooks
├── services/       # Comunicação com APIs
├── app/            # Estrutura do App Router (Next.js 13+)
├── styles/         # Temas e configurações do Stitches
├── assets/         # Imagens, ícones e SVGs
└── tests/          # Testes unitários e de integração
```

---

## 🧩 Padrões de Desenvolvimento

- Use nomes em inglês em todo o código.
- Reaproveite código existente quando possível, evitando duplicação.
- Segmente componentes grandes em partes menores e reutilizáveis.
- Evite alterar código desnecessariamente.
- Siga boas práticas de UI/UX.
- Rode **ESLint** e **Prettier** antes de cada commit.
- Respeite a arquitetura e convenções do Next.js.

---

## 💡 Padrões de Nomenclatura

| Entidade          | Convenção          | Exemplo                  |
| ----------------- | ------------------ | ------------------------ |
| Components        | `PascalCase`       | `TattooCard.tsx`         |
| Functions / Hooks | `camelCase`        | `useFetchInspiration.ts` |
| Enums             | `UPPER_SNAKE_CASE` | `TATTOO_CATEGORY`        |
| Interfaces        | Prefixo `I`        | `IUserProfile`           |
| Types             | Prefixo `T`        | `TColorPalette`          |
| Constants         | `UPPER_SNAKE_CASE` | `API_BASE_URL`           |

---

## 📦 Exemplo de Enum

```ts
// src/@enums/TattooCategory.ts
export enum TATTOO_CATEGORY {
  MINIMALIST = "Minimalist",
  TRIBAL = "Tribal",
  GEOMETRIC = "Geometric",
  REALISTIC = "Realistic",
}
```

---

## 🧠 Boas práticas de Pull Request (PR)

### Título

Use um tipo/escopo resumido seguido por uma descrição curta. Exemplos:

- `feat: add tattoo inspiration component`
- `fix: correct header responsive behavior`
- `chore: update dependencies`
- `refactor: refactor code`
- `config: project settings`
- `docs: documentation settings`

### Descrição

Inclua um breve contexto da alteração, prints (se aplicável) e detalhes relevantes.

### Checklist

- Testes atualizados/criados
- Lint e formatação executados (ESLint/Prettier)
- Sem breaking changes (quando aplicável)

### Regras e branches

- Commits pequenos e descritivos
- 1 PR = 1 propósito
- Revisão obrigatória por pelo menos 1 dev
- Branch base: `main`
- Branches de feature: `feature/<feature-name>`
- Branches de bugfix: `fix/<bug-name>`

---

## 🧪 Testes

- Utilize **Jest** e **Testing Library**.
- Nomeie arquivos de teste com sufixo `.spec.tsx`.

Exemplo:

```
src/components/ui/Button.spec.tsx
```

---

## 🧰 Scripts disponíveis

Use o gerenciador de pacotes do projeto (ex.: `pnpm`).

| Comando      | Descrição                            |
| ------------ | ------------------------------------ |
| `pnpm dev`   | Inicia o servidor de desenvolvimento |
| `pnpm build` | Cria o build de produção             |
| `pnpm start` | Executa em modo produção             |
| `pnpm lint`  | Roda o ESLint                        |
| `pnpm test`  | Executa os testes unitários          |

---

## 🌐 Deploy

O deploy é realizado automaticamente via Vercel a cada merge na branch `main`.

Ai, n sei se é coincidência, mas no codex normalmente meus promps são assim
 
---

## 💻 Uso de Prompt
 
Regras obrigatórias:

- Utilize nomes em inglês.
- Aproveite o código que já está criado.
- Utilize a pasta "/src/@types" pra armazenar types, 
- Utilize a pasta "/src/@interface para armazenar interfaces
- Utilize a pasta "/src/@enums para armazenar enums 
- Utilize a pasta "/src/common/constants" para armazenar as constants
- Caso o componente permita, segmente-o em menores
- Utilize as boas práticas de codificação e de Next.js
- Sigas as melhores práticas de UI/UXs
- Altere somente oq for necessário
 
Contexto
	- <descrição da tarefa>
 
---

## 🧾 Licença

Este projeto está sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.
