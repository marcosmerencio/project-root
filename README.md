# ⚙️ Project Root - Backend API

## 📝 Descrição
O Project Root é uma API robusta desenvolvida como o núcleo de processamento para aplicações de e-commerce e sistemas de gestão. Construído com foco em escalabilidade e segurança, este projeto representa a fundação backend (Root) necessária para gerenciar autenticação, persistência de dados e regras de negócio complexas. O projeto foi desenvolvido como parte do curso de Desenvolvimento Fullstack da Geração Tech 3.0.

## 🔗 Repositório
GitHub: https://github.com/marcosmerencio/project-root

## 🚀 Funcionalidades Principais
- Documentação Interativa (Swagger): Interface completa para exploração e teste dos endpoints da API.

- Testes Automatizados: Suíte de testes para garantir a confiabilidade e integridade das rotas e lógica de negócio.

- Gestão de Usuários e Autenticação: Fluxos de segurança para proteção de dados e controle de acesso.

- Gerenciamento de Produtos: CRUD completo para administração do catálogo.

- Middleware de Validação: Camadas de tratamento de erros e validação de requisições.

## 🛠️ Tecnologias Utilizadas
- Node.js: Ambiente de execução Javascript no servidor.

- Express: Framework para gerenciamento de rotas e middlewares.

- Swagger UI: Documentação automática e interativa da API.

- Jest / Supertest: Ferramentas para execução de testes unitários e de integração.

- Dotenv: Gerenciamento de variáveis de ambiente.

- CORS: Configuração de políticas de acesso seguro.

## 📂 Estrutura de Arquivos
Plaintext
project-root/
├── src/
│   ├── controllers/   # Lógica de controle das rotas e regras de negócio
│   ├── models/        # Definição dos esquemas de dados (Data Modeling)
│   ├── routes/        # Definição dos endpoints da API
│   ├── middlewares/   # Filtros de segurança e validação
│   ├── services/      # Comunicação com serviços externos ou lógica complexa
│   ├── database/      # Configuração da conexão com o banco de dados
│   ├── app.js         # Configuração central da aplicação Express
│   └── server.js      # Inicialização do servidor HTTP e escuta de porta
├── tests/             # Arquivos de testes automatizados (.test.js)
└── package.json       # Dependências e scripts do projeto

## ✨ Boas Práticas Aplicadas
O projeto utiliza padrões de engenharia de software que garantem a qualidade do código:

- Separation of Concerns (SoC): Organização modular que separa a rede, a lógica e os dados.

- Environment Isolation: Proteção de chaves e portas via variáveis de ambiente.

- Fail-Fast (Middleware): Bloqueio de requisições inválidas antes do processamento principal.

- Decoupled Architecture: Separação do arquivo app.js e server.js, permitindo testes de integração sem instanciar portas de rede desnecessariamente.

- Self-Documenting API: Uso de Swagger para manter a documentação técnica sempre sincronizada com o código.

## 📖 Documentação e Testes
### Documentação da API (Swagger)
A documentação completa dos endpoints pode ser visualizada e testada acessando:
👉 http://localhost:3001/api-docs/#/

### Testes Automatizados
Para garantir a integridade do sistema, execute a suíte de testes com o comando:
```Bash
npm run test
```
## ⚙️ Como rodar localmente
### Pré-requisitos:
Node.js (https://nodejs.org/en/) - Versão 18 ou superior

npm (https://www.npmjs.com/) - Geralmente instalado junto com o Node

Para verificar se você já os possui, digite no terminal: node -v e npm -v. Caso não estejam instalados, utilize os links citados anteriormente para baixá-los e faça a instalação.

### Passo a Passo:
(Os comandos abaixo devem ser utilizados no terminal Git Bash)

1. Clone o repositório: 
```Bash
git clone https://github.com/marcosmerencio/project-root.git
```

2. Acesse a pasta do projeto: 
```Bash
cd project-root
```

3. Instale as dependências: 
```Bash
npm install
```

4. Inicie o servidor de desenvolvimento: 
```Bash
npm run dev
```

## 🙏 Agradecimentos
A Deus pela oportunidade de participar do curso de Desenvolvimento Fullstack da Geração Tech 3.0.

Ao professor Luan Oliveira pela excelente didática e acompanhamento constante durante todo o curso.

À monitora Nazaré Almeida pela sua atenção, disponibilidade, orientação e incentivo durante o curso e no desenvolvimento desse projeto.

## ✒️ Autor
Marcos Merencio — Desenvolvedor Fullstack em formação.

## 📄 Licença
O uso, cópia e distribuição desse projeto são permitidos para fins de estudo e aprendizagem.