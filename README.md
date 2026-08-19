# 🚀 Aula 02 — Configuração do Ambiente de Desenvolvimento

> **Disciplina:** Frameworks Front-end
> **Professor:** Prof. Me. Deivison S. Takatu
> **Tema:** Configuração do Ambiente de Desenvolvimento

---

<a id="sumario"></a>

## 📚 Sumário

1. [🔄 Introdução ao Versionamento](#introducao-versionamento)
2. [🔢 Versionamento Semântico — SemVer](#versionamento-semantico)
3. [🐙 Git e Controle de Versão](#git-controle-versao)
4. [🏷️ Tags no Git](#tags-git)
5. [🌿 Branches e Boas Práticas](#branches-boas-praticas)
6. [💻 IDE e Visual Studio Code](#ide-vscode)
7. [🟢 Node.js](#nodejs)
8. [📦 NPM — Node Package Manager](#npm)
9. [⚛️ Criação de Projetos React](#projeto-react)
10. [📁 Estrutura de um Projeto React](#estrutura-react)
11. [📝 Atividade Prática](#atividade-pratica)
12. [📋 Atividade Complementar](#atividade-complementar)
13. [🚀 Deploy e Vercel](#deploy-vercel)
14. [🧠 Resumo para Estudo](#resumo-estudo)
15. [🎯 O que você precisa saber](#o-que-saber)
16. [📌 Comandos Principais](#comandos-principais)
17. [🏁 Conclusão](#conclusao)

---

<a id="introducao-versionamento"></a>

# 1. 🔄 Introdução ao Versionamento

O **versionamento** é o processo de atribuir um identificador único para cada versão de um documento ou software.

Ele permite registrar:

* 📅 Quando uma alteração foi realizada;
* 👤 Quem realizou a alteração;
* 📝 O que foi alterado;
* 🔍 Por que a alteração foi realizada;
* ↩️ Recuperar versões anteriores;
* 🤝 Facilitar o trabalho colaborativo.

O versionamento proporciona **rastreabilidade e auditoria** das mudanças realizadas no projeto.

---

## 🆚 Versionamento x Backup

| Versionamento                       | Backup                                         |
| ----------------------------------- | ---------------------------------------------- |
| Mantém o histórico das alterações   | Mantém uma cópia do estado atual               |
| Registra quem, quando e o que mudou | Não possui necessariamente rastreio de autoria |
| Permite colaboração                 | Normalmente trabalha com cópias                |
| Permite reversão granular           | Geralmente restaura uma versão completa        |
| Mantém histórico completo           | Pode manter apenas cópias pontuais             |

### 🎯 Benefícios do Versionamento

* 👥 Trabalho simultâneo;
* 🔄 Menos retrabalho;
* 🔍 Auditoria e rastreabilidade;
* ↩️ Recuperação de versões;
* 🤝 Colaboração eficiente;
* 🧪 Melhor gerenciamento da qualidade;
* 📈 Aprimoramento contínuo;
* 🔗 Integração com outras ferramentas.

---

## 💾 O Caos Antes do Versionamento

Era comum encontrar arquivos como:

```text
versao_final_agora_sim2.zip
```

Isso poderia causar:

* 💾 Arquivos duplicados;
* 🔥 Perda de código;
* ⚠️ Conflitos entre desenvolvedores;
* 🔍 Falta de histórico.

---

<a id="versionamento-semantico"></a>

# 2. 🔢 Versionamento Semântico — SemVer

O **Versionamento Semântico (Semantic Versioning)** utiliza o padrão:

```text
MAJOR.MINOR.PATCH
```

Exemplo:

```text
2.1.3
```

### 🔴 MAJOR

Mudança incompatível com versões anteriores.

```text
1.0.0 → 2.0.0
```

### 🟡 MINOR

Nova funcionalidade compatível com versões anteriores.

```text
1.0.0 → 1.1.0
```

### 🟢 PATCH

Correção de bugs sem alteração da compatibilidade.

```text
1.0.0 → 1.0.1
```

### 📌 Exemplos

```text
1.0.0 → Primeira versão estável
1.1.0 → Adição de funcionalidade compatível
1.1.1 → Correção de bug
2.0.0 → Mudança incompatível
```

---

<a id="git-controle-versao"></a>

# 3. 🐙 Git e Controle de Versão

O **Git** é um sistema de controle de versão utilizado para registrar e acompanhar alterações em arquivos e projetos.

Ele permite:

* 📜 Registrar versões;
* 🔄 Recuperar versões anteriores;
* 📤 Enviar código para repositórios online;
* 📥 Baixar código de repositórios;
* 👥 Facilitar o trabalho colaborativo.

### ⚙️ Verificar instalação

```bash
git --version
```

### 👤 Configurar usuário

```bash
git config --global user.name "<Nome>"
git config --global user.email "<Email>"
```

---

<a id="tags-git"></a>

# 4. 🏷️ Tags no Git

As **tags** são marcadores utilizados para identificar pontos específicos do histórico de um projeto.

São normalmente usadas para marcar versões importantes:

```text
v1.0
v2.0
v2.1
```

### 🏷️ Lightweight

Apenas um nome associado a um commit específico.

### 📝 Annotated

Armazena informações adicionais, como autor, data e mensagem.

### ⌨️ Comandos

Listar tags:

```bash
git tag
```

Criar uma tag:

```bash
git tag 1.0.0
```

Enviar uma tag:

```bash
git push origin 1.0.0
```

---

<a id="branches-boas-praticas"></a>

# 5. 🌿 Branches e Boas Práticas

Branches permitem desenvolver funcionalidades ou correções sem alterar diretamente a branch principal.

### ✅ Boas práticas

* 📌 Fazer commits pequenos e frequentes;
* 📝 Utilizar mensagens de commit claras;
* 🌿 Utilizar branches para novas funcionalidades;
* 🧪 Testar alterações antes do merge;
* 🔒 Manter a branch principal estável.

---

<a id="ide-vscode"></a>

# 6. 💻 IDE e Visual Studio Code

**IDE** significa:

> **Integrated Development Environment — Ambiente de Desenvolvimento Integrado.**

É uma ferramenta que reúne recursos necessários para:

* 👨‍💻 Desenvolver;
* 🧪 Testar;
* ▶️ Executar;
* 🐞 Depurar software.

O **Visual Studio Code (VS Code)** é um editor de código que, por meio de extensões e ferramentas integradas, oferece diversos recursos típicos de uma IDE.

---

<a id="nodejs"></a>

# 7. 🟢 Node.js

O **Node.js** é um ambiente de execução JavaScript que permite executar código no **backend**, ou seja, no servidor.

Uma de suas características é possibilitar o uso de JavaScript tanto no frontend quanto no backend.

### ⚙️ Verificar instalação

```bash
node --version
```

---

<a id="npm"></a>

# 8. 📦 NPM — Node Package Manager

O **NPM (Node Package Manager)** é o gerenciador de pacotes do Node.js.

Ele permite:

* 📥 Instalar bibliotecas;
* 🔄 Atualizar pacotes;
* 🗑️ Remover dependências;
* 📦 Gerenciar frameworks;
* 🤝 Compartilhar módulos;
* ⚙️ Automatizar o gerenciamento das dependências.

### 📄 package.json

O arquivo `package.json` registra informações importantes sobre as dependências e configurações do projeto.

Para instalar as dependências:

```bash
npm install
```

---

<a id="projeto-react"></a>

# 9. ⚛️ Criação de Projetos React

A aula apresenta o comando:

```bash
npx create-react-app <nome>
```

### 🛠️ Passo a passo

#### 1️⃣ Criar o projeto

```bash
npx create-react-app meu-projeto-react
```

#### 2️⃣ Entrar na pasta

```bash
cd meu-projeto-react
```

#### 3️⃣ Abrir no VS Code

```bash
code .
```

#### 4️⃣ Executar o servidor local

```bash
npm start
```

---

<a id="estrutura-react"></a>

# 10. 📁 Estrutura de um Projeto React

### 📦 node_modules

Contém os pacotes e bibliotecas instalados no projeto.

### 🌐 public

Contém arquivos públicos da aplicação, como HTML, JSON e imagens.

### ⚛️ src

Contém os arquivos JavaScript/React utilizados no projeto.

### 🚫 .gitignore

Define arquivos e diretórios que devem ser ignorados pelo Git.

### 📦 package.json

Contém informações sobre o projeto, dependências e comandos.

### 🔒 package-lock.json

Registra informações relacionadas às dependências utilizadas no projeto.

---

## 🧩 Principais arquivos

### `index.js`

Ponto de entrada do React.

### `App.js`

Componente raiz da aplicação.

### `App.css`

Estilos relacionados ao componente `App`.

### `index.css`

Estilos globais da aplicação.

---

<a id="atividade-pratica"></a>

# 11. 📝 Atividade Prática

A atividade proposta consiste em desenvolver uma aplicação React utilizando o **Visual Studio Code** como ambiente de desenvolvimento.

O projeto deverá:

1. ⚛️ Desenvolver uma aplicação React;
2. 💻 Utilizar o VS Code;
3. 🐙 Utilizar Git para versionamento;
4. 📌 Realizar commits;
5. 📤 Fazer push para um repositório no GitHub;
6. ▲ Publicar a aplicação na Vercel;
7. 🔗 Conectar o repositório à Vercel;
8. 🌎 Disponibilizar o projeto através de uma URL pública da Vercel.

---

## 🔗 Link do Projeto

### ▲ Projeto publicado na Vercel

**URL:**

```text
[COLE_AQUI_O_LINK_DO_PROJETO](https://projeto-aula2-lemon.vercel.app)
```

### 🐙 Repositório no GitHub

**URL:**

```text
https://github.com/ronaldorfas/projeto-aula2
```

<a href="#sumario">⬆️ Voltar ao Sumário</a>

---

<a id="atividade-complementar"></a>

# 12. 📋 Atividade Complementar

Em grupos, escolher um **Framework Front-end** e elaborar um relatório técnico em PDF com **mínimo de 5 páginas**.

O relatório deve apresentar:

* 📌 Principais características;
* ✅ Vantagens;
* 🏢 Aplicações no mercado;
* 💻 Exemplo de utilização em um projeto Web.

---

<a href="#sumario">⬆️ Voltar ao Sumário</a>

---

<a id="deploy-vercel"></a>

# 13. 🚀 Deploy e Vercel

## 🚀 O que é Deploy?

**Deploy** é o processo de colocar uma aplicação ou software em produção, tornando-o acessível aos usuários finais.

### 🔄 Etapas comuns

```text
Código
   ↓
Compilação
   ↓
Configuração
   ↓
Testes finais
   ↓
Publicação
```

---

## ▲ Vercel

A **Vercel** é uma plataforma voltada para facilitar o deploy de sites estáticos e aplicações modernas.

### ⭐ Principais características

* 🚀 Deploy simplificado;
* 🔗 Integração com GitHub, GitLab e Bitbucket;
* ⚛️ Suporte a frameworks modernos;
* 🔄 Deploy automático após um push;
* ↩️ Possibilidade de rollback;
* ⚡ Deploys rápidos.

### ☁️ Serverless Functions

Permitem executar funções de backend sem a necessidade de gerenciar diretamente os servidores.

### 🌐 CDN Global

Distribui conteúdos através de uma rede de alta performance.

---

<a id="resumo-estudo"></a>

# 14. 🧠 Resumo para Estudo

| Conceito         | Função                                           |
| ---------------- | ------------------------------------------------ |
| 🔄 Versionamento | Controlar o histórico das alterações             |
| 🔢 SemVer        | Identificar versões através de MAJOR.MINOR.PATCH |
| 🐙 Git           | Controlar versões do código                      |
| 🏷️ Tag          | Marcar versões importantes                       |
| 🌿 Branch        | Desenvolver alterações isoladamente              |
| 💻 VS Code       | Editar e desenvolver código                      |
| 🟢 Node.js       | Executar JavaScript fora do navegador            |
| 📦 NPM           | Gerenciar pacotes e dependências                 |
| ⚛️ React         | Criar aplicações utilizando componentes          |
| 🚀 Deploy        | Publicar uma aplicação                           |
| ▲ Vercel         | Hospedar e realizar deploy                       |

---

<a id="o-que-saber"></a>

# 15. 🎯 O que você precisa saber?

### ⭐ Versionamento

Entender por que ele é diferente de um simples backup.

### ⭐ SemVer

Memorizar:

```text
MAJOR → Mudança incompatível
MINOR → Nova funcionalidade compatível
PATCH → Correção de bug
```

### ⭐ Git

Conhecer os conceitos de:

* Commit;
* Branch;
* Tag;
* Repositório.

### ⭐ Node.js + NPM

Entender a função do Node.js e do NPM no desenvolvimento.

### ⭐ React

Conhecer o processo básico de criação e execução de um projeto.

### ⭐ Deploy

Entender o processo de colocar uma aplicação em produção.

### ⭐ Vercel

Conhecer sua função como plataforma de hospedagem e deploy.

---

<a id="comandos-principais"></a>

# 16. 📌 Comandos Principais

```bash
# Verificar Git
git --version

# Configurar usuário
git config --global user.name "<Nome>"
git config --global user.email "<Email>"

# Verificar Node.js
node --version

# Criar projeto React
npx create-react-app meu-projeto-react

# Entrar no projeto
cd meu-projeto-react

# Abrir no VS Code
code .

# Executar projeto
npm start

# Instalar dependências
npm install

# Listar tags
git tag

# Criar tag
git tag 1.0.0

# Enviar tag
git push origin 1.0.0
```

---

<a id="conclusao"></a>

# 17. 🏁 Conclusão

A Aula 02 apresenta a preparação de um ambiente básico para desenvolvimento **Front-end**, passando pelo controle de versões com **Git**, criação de aplicações **React** e publicação através da **Vercel**.

O fluxo geral pode ser representado por:

```text
💻 VS Code
     ↓
⚛️ React
     ↓
📦 NPM
     ↓
🐙 Git
     ↓
💾 Commit
     ↓
🌐 GitHub
     ↓
▲ Vercel
     ↓
🚀 Deploy
     ↓
🌎 Aplicação Online
```

---

<a href="#sumario">⬆️ Voltar ao Sumário</a>

---

## 📚 Referência da Aula

**Aula 02 — Configuração do Ambiente de Desenvolvimento**
**Disciplina:** Frameworks Front-end
**Professor:** Prof. Me. Deivison S. Takatu
