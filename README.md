# Vercel AI SDK RAG Guide Starter Project

Este projeto de estudo usa como base [Retrieval-Augmented Generation (RAG) guide](https://sdk.vercel.ai/docs/guides/rag-chatbot).

# Passos
1. Executar **docker compose up** para criar um docker container com o postgres que será nosso banco de dados vetorial
2. Renomear o arquivo **.env.example** para **.env**
3. Configurar no **.env** a string de conexão com o postgres
4. Executar **npm run db:migrate** para:
    - Adicionar extensão **pgvector** ao banco de dados
    - Criar uma nova tabela chamada **resources** com 4 colunas (id, content, createdAt, e updatedAt)