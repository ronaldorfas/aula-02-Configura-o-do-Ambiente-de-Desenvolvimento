# 🚀 Aula 02 — Configuração do Ambiente de Desenvolvimento

> **Disciplina:** Frameworks Front-end
> **Professor:** Prof. Me. Deivison S. Takatu
> **Tema:** Configuração do Ambiente de Desenvolvimento

---

## 📚 Sumário

1. 🔄 Introdução ao Versionamento
2. 🔢 Versionamento Semântico — SemVer
3. 🐙 Git e Controle de Versão
4. 🏷️ Tags e Branches
5. 💻 IDE e Visual Studio Code
6. 🟢 Node.js
7. 📦 NPM
8. ⚛️ Criação de Projetos React
9. 📁 Estrutura de um Projeto React
10. 🚀 Deploy e Hospedagem com Vercel
11. 📝 Atividade Prática
12. 📌 Resumo Geral

---

# 1. 🔄 Introdução ao Versionamento

O **versionamento** é o processo de atribuir um identificador único para cada versão de um documento ou software.

Ele permite registrar:

* 📅 Quando uma alteração foi realizada;
* 👤 Quem realizou a alteração;
* 📝 O que foi alterado;
* 🔍 Por que a alteração foi realizada;
* ↩️ Recuperar versões anteriores;
* 🤝 Facilitar o trabalho colaborativo.

O versionamento também proporciona **rastreabilidade e auditoria** das mudanças realizadas no projeto.

---

## 🆚 Versionamento x Backup

| Versionamento                       | Backup                                         |
| ----------------------------------- | ---------------------------------------------- |
| Mantém o histórico das alterações   | Mantém uma cópia do estado atual               |
| Registra quem, quando e o que mudou | Não possui necessariamente rastreio de autoria |
| Permite colaboração                 | Normalmente trabalha com cópias                |
| Permite reversão granular           | Geralmente restaura uma versão completa        |
| Mantém histórico completo           | Pode manter apenas cópias pontuais             |

### 🎯 Por que utilizar versionamento?

Antes dos sistemas de controle de versão, era comum encontrar arquivos como:

`versao_final_agora_sim2.zip`

Isso poderia causar:

* 💾 Arquivos duplicados;
* 🔥 Perda de código;
* ⚠️ Conflitos entre desenvolvedores;
* 🔍 Falta de histórico.

O versionamento resolve esses problemas através do registro organizado das alterações.

---

# 2. 🔢 Versionamento Semântico — SemVer

O **Versionamento Semântico (Semantic Versioning)** utiliza o padrão:

```text
MAJOR.MINOR.PATCH
```

Exemplo:

```text
2.1.3
```

Cada número possui uma função específica.

### 🔴 MAJOR

Indica uma mudança **incompatível** com versões anteriores.

```text
1.0.0 → 2.0.0
```

Exemplo:

Uma alteração na aplicação que faz com que funcionalidades existentes deixem de funcionar.

---

### 🟡 MINOR

Indica a inclusão de uma nova funcionalidade mantendo a compatibilidade.

```text
1.0.0 → 1.1.0
```

---

### 🟢 PATCH

Indica correções de problemas sem alteração significativa na compatibilidade.

```text
1.0.0 → 1.0.1
```

---

## 📌 Exemplos

```text
1.0.0 → Primeira versão estável
1.1.0 → Nova funcionalidade compatível
1.1.1 → Correção de bug
2.0.0 → Alteração incompatível
```

A versão `1.0.0` representa o lançamento público estável, enquanto versões `0.x.x` indicam desenvolvimento inicial.

---

# 3. 🐙 Git e Controle de Versão

O **Git** é um sistema de controle de versão utilizado para registrar e acompanhar alterações em arquivos e projetos.

Ele pode:

* 📜 Registrar versões;
* 🔄 Recuperar versões anteriores;
* 📤 Enviar código para repositórios online;
* 📥 Baixar código de repositórios;
* 👥 Facilitar o trabalho entre desenvolvedores.

O Git é instalado no computador e pode ser utilizado através da linha de comando.

---

## ⚙️ Instalação do Git

Após instalar o Git, é possível verificar sua instalação através do CMD:

```bash
git --version
```

Se uma versão for exibida, a instalação foi realizada corretamente.

### 👤 Configuração do usuário

Caso seja solicitado:

```bash
git config --global user.name "<Nome>"
git config --global user.email "<Email>"
```

Essas informações identificam o autor dos commits.

---

# 4. 🏷️ Tags no Git

As **tags** são marcadores utilizados para identificar pontos específicos do histórico de um projeto.

Normalmente são utilizadas para representar versões importantes, como:

```text
v1.0
v2.0
v2.1
```

Existem dois tipos apresentados na aula:

### 🏷️ Lightweight

É apenas um nome associado a um commit específico.

### 📝 Annotated

Armazena informações adicionais, como:

* Autor;
* Data;
* Mensagem.

---

## ⌨️ Comandos de Tags

Listar tags:

```bash
git tag
```

Criar uma tag:

```bash
git tag <nome-da-tag>
```

Exemplo:

```bash
git tag 1.0.0
```

Enviar uma tag:

```bash
git push origin <nome-da-tag>
```

---

# 5. 🌿 Branches e Boas Práticas

Branches permitem desenvolver funcionalidades ou correções sem alterar diretamente a branch principal.

A aula recomenda:

* 📌 Fazer commits pequenos e frequentes;
* 📝 Utilizar mensagens de commit claras;
* 🌿 Utilizar branches para novas funcionalidades;
* 🧪 Testar alterações antes do merge;
* 🔒 Manter a branch principal estável.

---

# 6. 💻 IDE e Visual Studio Code

**IDE** significa:

> **Integrated Development Environment — Ambiente de Desenvolvimento Integrado.**

É uma ferramenta que reúne recursos necessários para:

* 👨‍💻 Desenvolver;
* 🧪 Testar;
* ▶️ Executar;
* 🐞 Depurar software.

O **Visual Studio Code (VS Code)** é um editor de código que, através de extensões e ferramentas integradas, oferece diversos recursos encontrados em uma IDE.

---

# 7. 🟢 Node.js

O **Node.js** é um ambiente de execução JavaScript que permite executar código no **backend**, ou seja, no servidor.

Uma de suas principais características é permitir utilizar JavaScript tanto:

```text
Frontend
   +
Backend
```

Isso facilita a integração entre as partes da aplicação.

---

## ⚙️ Testando o Node.js

Depois da instalação:

```bash
node --version
```

Se o terminal apresentar a versão instalada, o Node.js está funcionando corretamente.

---

# 8. 📦 NPM — Node Package Manager

O **NPM (Node Package Manager)** é o gerenciador de pacotes do Node.js.

Ele permite:

* 📥 Instalar bibliotecas;
* 🔄 Atualizar pacotes;
* 🗑️ Remover dependências;
* 📦 Gerenciar frameworks;
* 🤝 Compartilhar módulos;
* ⚙️ Automatizar o gerenciamento das dependências.

O NPM é instalado automaticamente junto com o Node.js.

---

## 📄 package.json

O arquivo:

```text
package.json
```

registra informações importantes sobre as dependências do projeto.

Para instalar as dependências registradas:

```bash
npm install
```

Isso facilita a configuração do projeto em diferentes computadores.

---

# 9. ⚛️ Criando um Projeto React

A aula apresenta o comando:

```bash
npx create-react-app <nome>
```

O comando cria uma aplicação React com uma estrutura inicial pronta para desenvolvimento.

---

## 🛠️ Passo a passo

### 1️⃣ Criar o projeto

```bash
npx create-react-app meu-projeto-react
```

### 2️⃣ Entrar na pasta

```bash
cd meu-projeto-react
```

### 3️⃣ Abrir no VS Code

```bash
code .
```

### 4️⃣ Executar o servidor local

```bash
npm start
```

---

# 10. 📁 Estrutura do Projeto React

Um projeto React possui diferentes arquivos e diretórios.

## 📦 node_modules

Contém os pacotes instalados e as bibliotecas utilizadas pelo projeto.

```bash
npm i
```

pode ser utilizado para instalar dependências.

---

## 🌐 public

Contém arquivos públicos da aplicação, como:

* HTML;
* JSON;
* Imagens.

---

## ⚛️ src

Contém os arquivos JavaScript/React utilizados no projeto.

---

## 🚫 .gitignore

Define arquivos e diretórios que devem ser ignorados pelo Git.

Pode ser utilizado, por exemplo, para evitar o versionamento de informações que não devem ser enviadas ao repositório.

---

## 📦 package.json

Contém informações sobre o projeto, dependências e comandos.

---

## 🔒 package-lock.json

Registra informações relacionadas às dependências utilizadas pelo projeto.

---

# 11. 🧩 Principais Arquivos React

### `index.js`

É o ponto de entrada do React e realiza a renderização da aplicação no DOM.

### `App.js`

É o componente raiz da aplicação.

### `App.css`

Contém estilos relacionados ao componente `App`.

### `index.css`

Contém estilos globais que podem afetar toda a aplicação.

---

# 12. 🚀 Deploy

**Deploy** é o processo de colocar uma aplicação ou software em produção, tornando-o acessível aos usuários finais.

O objetivo é garantir que a aplicação funcione corretamente no ambiente de produção.

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

# 13. ▲ Vercel

A **Vercel** é uma plataforma voltada para facilitar o deploy de sites estáticos e aplicações modernas.

Entre suas características apresentadas na aula estão:

* 🚀 Deploy simplificado;
* 🔗 Integração com GitHub, GitLab e Bitbucket;
* ⚛️ Suporte a frameworks modernos;
* 🔄 Deploy automático após um push;
* ↩️ Possibilidade de rollback;
* ⚡ Deploys rápidos.

---

## 🌎 Outros recursos da Vercel

A aula também apresenta:

### ☁️ Serverless Functions

Permitem executar funções de backend sem a necessidade de gerenciar diretamente os servidores.

### 🌐 CDN Global

Distribui conteúdos por uma rede de alta performance, buscando reduzir a latência.

### ⚡ Performance e Escalabilidade

A plataforma é apresentada como voltada para aplicações web modernas, oferecendo performance, escalabilidade automática e segurança.

---

# 14. 📝 Atividade Prática

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

# 15. 📋 Atividade Complementar

A aula também propõe uma atividade em grupos:

> Escolher um Framework Front-end e elaborar um relatório técnico em PDF com **mínimo de 5 páginas**.

O relatório deve apresentar:

* 📌 Principais características;
* ✅ Vantagens;
* 🏢 Aplicações no mercado;
* 💻 Exemplo de utilização em um projeto Web.

---

# 🧠 Resumo para Estudo

| Conceito         | Função                                           |
| ---------------- | ------------------------------------------------ |
| 🔄 Versionamento | Controlar o histórico das alterações             |
| 🔢 SemVer        | Identificar versões através de MAJOR.MINOR.PATCH |
| 🐙 Git           | Controlar versões do código                      |
| 🏷️ Tag          | Marcar versões/pontos importantes                |
| 🌿 Branch        | Trabalhar em alterações isoladamente             |
| 💻 VS Code       | Editar e desenvolver código                      |
| 🟢 Node.js       | Executar JavaScript fora do navegador            |
| 📦 NPM           | Gerenciar pacotes e dependências                 |
| ⚛️ React         | Criar aplicações utilizando componentes          |
| 🚀 Deploy        | Publicar uma aplicação                           |
| ▲ Vercel         | Hospedar e realizar deploy de aplicações         |

---

# 🔥 Fluxo Completo da Aula

O fluxo geral apresentado pode ser entendido assim:

```text
💻 VS Code
     ↓
⚛️ Criar projeto React
     ↓
📦 NPM / Dependências
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
🌎 Aplicação disponível online
```

---

# 🎯 O que você precisa saber para a prova/atividade?

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

Saber sua finalidade e os conceitos de commit, branch e tag.

### ⭐ Node.js + NPM

Entender que o Node.js executa JavaScript fora do navegador e que o NPM gerencia pacotes e dependências.

### ⭐ React

Conhecer o processo básico de criação e execução de um projeto.

### ⭐ Deploy

Entender que é o processo de colocar a aplicação em produção.

### ⭐ Vercel

Conhecer sua função como plataforma de hospedagem e deploy.

---

# 📌 Comandos Principais

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

## 🏁 Conclusão

A Aula 02 apresenta a preparação de um ambiente básico para desenvolvimento **Front-end**, passando desde o controle de versões com **Git** até a criação de aplicações **React** e sua publicação através da **Vercel**.

O fluxo fundamental é:

**Git → VS Code → Node.js → NPM → React → GitHub → Vercel → Deploy**

Esse conjunto de ferramentas permite desenvolver, versionar, compartilhar e publicar aplicações Web de forma organizada e colaborativa.
