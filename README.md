# ⚙️ Project Root - Backend API
<p align="center">
<img src="https://img.shields.io/badge/node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js" />
<img src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express" />
<img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black" alt="Swagger" />
<img src="https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white" alt="Jest" />
</p>


# 📝 Descrição
O Project Root é uma API robusta desenvolvida como o núcleo de processamento para aplicações de e-commerce e sistemas de gestão. Construído com foco em escalabilidade e segurança, este projeto representa a fundação backend necessária para gerenciar autenticação, persistência de dados e regras de negócio complexas. Esse projeto backend foi desenvolvido como parte da conclusão do curso de Desenvolvimento Fullstack da Geração Tech 3.0.


# 🔗 Repositório
GitHub: https://github.com/marcosmerencio/project-root


# 🚀 Funcionalidades Principais
- **Documentação Interativa (Swagger):** Interface completa para exploração e teste dos endpoints da API.

- **Testes Automatizados:** Suíte de testes para garantir a confiabilidade e integridade das rotas.

- **Gestão de Usuários e Autenticação:** Fluxos de segurança para proteção de dados e controle de acesso.

- **Gerenciamento de Produtos:** CRUD completo para administração do catálogo.

- **Middleware de Validação:** Camadas de tratamento de erros e validação de requisições.


# 🛠️ Tecnologias Utilizadas
- **Node.js:** Ambiente de execução Javascript no servidor.

- **Express:** Framework para gerenciamento de rotas e middlewares.

- **Swagger UI:** Documentação automática e interativa da API.

- **Jest / Supertest:** Ferramentas para execução de testes unitários e de integração.

- **Dotenv:** Gerenciamento de variáveis de ambiente.

- **CORS:** Configuração de políticas de acesso seguro.


# 📂 Estrutura de Arquivos
```Plaintext
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
```

# ✨ Boas Práticas Aplicadas
O projeto utiliza padrões de engenharia de software que garantem a qualidade do código:

- **Separation of Concerns (SoC):** Organização modular que separa a rede, a lógica e os dados.

- **Environment Isolation:** Proteção de chaves e portas via variáveis de ambiente.

- **Fail-Fast (Middleware):** Bloqueio de requisições inválidas antes do processamento principal.

- **Decoupled Architecture:** Separação do arquivo app.js e server.js, permitindo testes de integração sem instanciar portas de rede desnecessariamente.

- **Self-Documenting API:** Uso de Swagger para manter a documentação técnica sempre sincronizada com o código.


# 📖 Documentação e Testes
## Documentação da API (Swagger)
A documentação completa dos endpoints pode ser visualizada e testada acessando:

http://localhost:3001/api-docs/#/

## Testes Automatizados
Para garantir a integridade do sistema, execute a suíte de testes com o comando:

```Bash
npm run test
```

# ⚙️ Como rodar localmente
## Pré-requisitos:
Antes de começar, verifique se você possui o Node.js (v18+) e o npm instalados:

```Bash
node -v
npm -v
```
Caso não tenha instalado:

- Windows/macOS: Baixe a versão LTS em nodejs.org.

- Linux: sudo apt install nodejs npm.

### Passo a Passo:
**1. Clone o repositório:**
```Bash
git clone https://github.com/marcosmerencio/project-root.git
```

**2. Acesse a pasta do projeto:**
```Bash
cd project-root
```

**3. Instale as dependências:**
```Bash
npm install
```

**4. Configure o arquivo .env (Obrigatório):**
Crie um arquivo chamado .env na raiz do seu projeto e cole o conteúdo abaixo. Substitua os valores indicados para que a API funcione corretamente:
```Snippet de código
# Configurações do Servidor
PORT=3001
NODE_ENV=development

# Configurações do Banco de Dados
# ATENÇÃO: Substitua pelos dados do seu banco de dados local ou remoto
DB_HOST=substitua_pelo_host_do_banco      # Ex: localhost
DB_PORT=substitua_pela_porta_do_banco     # Ex: 27017
DB_USER=substitua_pelo_usuario_do_banco   # Seu usuário
DB_PASS=substitua_pela_senha_do_banco     # Sua senha
DB_NAME=project_root_db                   # Seu banco de dados  

# Segurança e Autenticação
# IMPORTANTE: Crie uma chave secreta forte para o JWT
JWT_SECRET=substitua_por_uma_chave_longa_e_segura
JWT_EXPIRES_IN=7d
```

**5. Inicie o servidor de desenvolvimento:**
```Bash
npm run dev
```


# 📈 Próximos Passos Sugeridos
- **Refresh Tokens:** Implementar estratégia de Refresh Tokens para reduzir o tempo de expiração do Access Token de 7 dias para 15 (ou 30) minutos, aumentando a segurança.

- **Dockerização:** Criar um Dockerfile e docker-compose.yml para facilitar o deploy e padronizar o ambiente de desenvolvimento.

- **Logging:** Integrar bibliotecas como Winston ou Morgan para monitoramento de erros e logs de requisições em tempo real.

- **CI/CD:** Configurar GitHub Actions para rodar a suíte de testes automaticamente a cada novo Pull Request.


# 🙏 Agradecimentos
- A **Deus** pela oportunidade de participar do curso de Desenvolvimento Fullstack da Geração Tech 3.0.

- Ao professor Luan Oliveira pela excelente didática e acompanhamento constante durante todo o curso.

- À monitora Nazaré Almeida, pela sua atenção, disponibilidade, orientação e incentivo durante o curso e no desenvolvimento deste projeto.


# ✒️ Autor
**Marcos Merencio** — Desenvolvedor Fullstack em formação.


# 📄 Licença
O **uso, cópia e distribuição** desse projeto são **permitidos para fins de estudo e aprendizagem.**