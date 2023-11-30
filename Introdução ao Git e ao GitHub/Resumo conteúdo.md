## Visão Geral do Curso e Ferramentas

### O que é versionamento de código?

- São softwares que controlam as versões de um arquivo ao longo do tempo.
  - Registra o histórico de atualizações de um arquivo.
  - Gerencia quais foram as alterações, a data, o autor, etc.
  - Organização, controle e segurança.

### Tipos de Sistemas de Controle de Versão (VCS)

- **VCS Centralizado (CVCS)**
  - Contém apenas um servidor que irá conter todos os arquivos responsáveis pelo controle de versão.
  - Desvantagens:
    - Caso fique fora do ar, não será possível salvar, colaborar ou alterar nos projetos versionados no servidor.
    - Se algum arquivo for corrompido ou houver perca de dados no servidor, existe a possibilidade de perca do projeto.
  - Ex.: CVS, Subversion.
- **VCS Distribuído (DVCS)**
  - Clona o repositório completo, o que inclui o histórico de versões.
    - Cada clone é como um backup
    - Possibilita um fluxo de trabalho flexível
    - Possibilidade de trabalhar sem conexão à rede
  - Ex.: Git, Mercurial.

> ###### Repositório: 
>
> - é o local onde vai estar sendo armazenado tanto os seus arquivos quanto os responsáveis pela gestão dessas versões.

### O que é Git?

- Sistema de Controle de Versão Distribuído.
  - Gratuito e Open Source (código aberto)
  - Ramificações (branching) e fusões (merging) eficientes
  - Leve e rápido
- Fluxo Básico no Git:
  - git clone - clonar o repositório remoto para uma pasta local.
  - git commit - grava alterações no repositório.
  - git pull - “puxa” as alterações do repositório remoto para o local (busca e mescla).
  - git push - “empurra” as alterações do repositório local para o remoto.

[Git](https://git-scm.com/)

### O que é o GitHub?

- Plataforma de hospedagem de código para controle de versão com Git e colaboração.

> [GitHub: Let’s build from here](https://github.com/)

## Primeiros Passos com Git e GitHub

> [GitHub - elidianaandrade/dio-curso-git-github: Repositório do curso Versionamento de Código com Git e GitHub da Digital Innovation One.](https://github.com/elidianaandrade/dio-curso-git-github)

### Criando e Clonando Repositórios

Existem duas formas de obter um repositório Git na sua máquina:

1. Transformando um diretório local que não está sob controle de versão, num repositório git
   - Usa-se: git init
2. Clonando um repositório Git existente.
   - Usa-se: git clone

> mkdir - make directory

### Trabalhando com Branches

De maneira simplista, uma Branch (em tradução, “Ramo”), é uma ramificação do seu projeto.

- É um ponteiro móvel para um commit no histórico do repositório.
- Quando você cria uma nova Branch a partir de outra existente, a nova se inicia apontando para o mesmo commit da Branch que estava sendo criada.

> “Imagine que você quer adicionar uma funcionalidade nova para o seu projeto mas não tem certeza se quer aplicar. Então você cria uma Branch, que seria como um universo paralelo do seu projeto, e você pode testar suas funcionalidades sem afetar a Branch principal.”