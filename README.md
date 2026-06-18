# Classificador de Mensagens Corporativas com IA

## Objetivo

O Classificador de Mensagens Corporativas é uma aplicação que utiliza inteligência artificial via OpenRouter para analisar mensagens e classificá-las automaticamente em quatro categorias:

- Urgente  
- Dúvida  
- Informativo  
- Solicitação  

O objetivo do sistema é ajudar empresas e equipes a organizarem melhor o fluxo de comunicação, permitindo identificar rapidamente o tipo e a prioridade de cada mensagem.

---

## Como funciona

### Entrada

O usuário envia uma mensagem corporativa em texto simples, como e-mails, mensagens internas ou solicitações de suporte.
- Ex: 
- "Caiu o servidor e não temos nenhum dev dísponivel agora, precisamos acessar os dados o quanto antes"
- "O relatório ta atualizado?"
- "Tem café passado no segundo andar para quem quiser"
- "Consegue me enviar os arquivos, por favor"

---

### Processamento

O backend recebe o texto e o envia para um modelo de inteligência artificial através da API do OpenRouter.

O modelo é instruído a:

- Ler a mensagem  
- Interpretar o contexto  
- Classificar em uma das quatro categorias  
- Justificar brevemente a escolha  

---

### Saída

O sistema retorna:

- Categoria da mensagem  
- Justificativa da classificação
- Ex: "Caiu o servidor e não temos nenhum dev dísponivel agora, precisamos acessar os dados o quanto antes"
- Saída: Urgente.
- Justificativa: Relata um problema crítico que está impactando as operações da empresa e exige ação imediata.

# Instalação do Projeto

Para instalar e executar o projeto localmente, siga os passos abaixo.

Primeiro, é necessário ter o Node.js instalado no computador. Após isso, baixe ou clone o repositório do GitHub e entre na pasta do projeto usando o terminal:

```bash
cd nome-do-projeto
```

Depois disso, instale todas as dependências necessárias com o comando:
````bash
npm install
````
Em seguida, crie um arquivo chamado .env na raiz do projeto e adicione sua chave da OpenRouter: 

OPENROUTER_API_KEY=sua_chave_aqui

No terminal execute:
````bash
npm start
````
Isso abrirá uma aba no navegador com o modelo já funcional.
