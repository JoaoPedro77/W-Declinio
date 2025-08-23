# 🛵 W-Declinio 

## 📖 Descrição

Este projeto é um **jogo de escolhas** feito com **React + TypeScript**.
A interface será dividida em três áreas principais:

* **Painel Esquerdo:** Mostra informações sobre o jogador (itens, status, quests), controlado pelos botões da barra superior.
* **Área Central:** Exibe o texto da cena atual e oferece 3 botões de escolha.
* **Painel Direito:** Mostra apenas o **histórico das escolhas feitas** pelo jogador.

Cada escolha leva a uma nova cena, permitindo criar diferentes caminhos e finais alternativos

---

## 🚀 Tecnologias

* **React + Vite**
* **TypeScript**
* **CSS / Tailwind**

---

## 📂 provavel estrutura do projeto

```bash
W-Declinio/
│── public/
│── src/
│   ├── components/
│   │   ├── TopBar.tsx
│   │   ├── PainelEsquerda.tsx
│   │   ├── PainelPrincipal.tsx
│   │   ├── PainelDireita.tsx
│   ├── types/
│   │   ├── story.ts
│   ├── data/
│   │   ├── story.ts        # cenas da história ( tata vai escrever muito aqui)
│   ├── App.tsx 
│   ├── main.tsx  
│── package.json
│── tsconfig.json
│── README.md
```

---

## 📋 Coisas a Fazer

### 🎨 Layout

* [ ] Criar layout descrito com as 3 colunas;
* [ ] Adicionar barra superior (`Itens`, `Status`, `Quests`);
* [ ] Fazer painel esquerdo exibir dados diferentes conforme botão clicado;

### 🧩 Funcionalidades

* [ ] Exibir texto da cena no painel central.
* [ ] Implementar 3 botões de escolha por cena.
* [ ] Cada escolha muda a cena atual.
* [ ] Registrar no painel direito o histórico apenas das escolhas feitas.


### 🗂️ Tipagem

* [ ] Criar interface `Scene` com:

  ```ts
  interface Scene {
    id: string;
    text: string;
    choices: { text: string; nextId: string }[];
  }
  ```
* [ ] Criar lista de cenas (`story.ts`) seguindo essa tipagem.

### 📚 Narrativa (exemplo inicial)

* [ ] tata escreve historia e poe ideias futuras aqui

### 🔮 Futuro

* [ ] (talvez) implementar sistema de localização de acontecimentos
* [ ] Salvar progresso no `localStorage`.

---

## 🏃 Como rodar

1. Criar projeto com Vite + React + TypeScript:

   ```bash
   npm create vite@latest meu-jogo-escolhas -- --template react-ts
   ```
2. Entrar na pasta:

   ```bash
   cd meu-jogo-escolhas
   ```
3. Instalar dependências:

   ```bash
   npm install
   ```
4. Rodar:

   ```bash
   npm run dev
   ```

---

