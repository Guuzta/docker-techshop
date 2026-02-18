# Projeto Docker Techshop - Frontend + API

Este repositório é um exemplo de aplicação fullstack em **Docker**, com frontend em **Next.js** e backend em **Node.js/Prisma**, gerenciado pelo **docker-compose**.

## Estrutura do projeto

```
docker-techshop/
├─ 📁 api_techshop/        ← submodule do backend
├─ 📁 Techshop/   ← submodule do frontend
├─ 📄 docker-compose.yml ← gerencia todos os containers
├─ 📁 nginx/      ← configuração do reverse proxy
└─ 📄 README.md
```

## Pré-requisitos

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/)

## Configuração inicial

1. Clone o repositório com submodules:

```bash
git clone --recursive <URL_DO_REPOSITORIO>
```

2. Copie os arquivos de exemplo `.env`:

```bash
cp api_techshop/.env.example api_techshop/.env
cp Techshop/.env.example Techshop/.env
```

## Rodando o projeto

No diretório raiz do projeto, execute:

```bash
docker compose up -d --build
```

## Pronto! Agora você pode acessar a aplicação totalmente funcional

- **Frontend:** [http://localhost/](http://localhost/)

- **API:** [http://localhost/api/](http://localhost/api/)
