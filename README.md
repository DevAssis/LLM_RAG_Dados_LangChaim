# LLM_RAG_Dados_LangChaim
### Pipeline de Perguntas e Respostas com RAG, Vetorização e Embedding(QA)


Este repositório apresenta um pipeline completo para construir um sistema de perguntas e respostas (QA) utilizando técnicas avançadas de Retrieval Augmented Generation (RAG), vetorização e embedding. O sistema processa dados não estruturados brutos e permite interação em linguagem natural.

## Etapas do Pipeline

1. **Carregamento e Pré-processamento**:
   - Carrega dados não estruturados de diversas fontes utilizando o LangChain Integration Hub.
   - Divide os documentos em partes menores (chunks) com o `RecursiveCharacterTextSplitter`, otimizando o tamanho dos chunks com `tiktoken`.

2. **Vetorização e Embedding**:
   - Converte os chunks de texto em representações vetoriais (embeddings) utilizando o modelo "sentence-transformers/all-MiniLM-L6-v2" do HuggingFace Embeddings.
   - Armazena os chunks e suas embeddings em um banco de dados vetorial ChromaDB, permitindo busca eficiente por similaridade.

3. **RAG e Geração de Respostas**:
   - Implementa a técnica de RAG, recuperando chunks relevantes do banco de dados vetorial com base na similaridade semântica com a pergunta do usuário.
   - Utiliza o modelo de linguagem GPT-4 da OpenAI e LangChain RetrievalQA para gerar respostas precisas e informativas, combinando o conhecimento do modelo com as informações relevantes dos chunks recuperados.

4. **Interação com o Usuário**:
   - Permite que o usuário faça perguntas em linguagem natural e receba respostas contextuais e informativas.

## Próximos Passos

- Refinar o sistema com técnicas avançadas de engenharia de prompts e Prompt Templates do LangChain.

## Habilidades Demonstradas

- Retrieval Augmented Generation (RAG)
- Vetorização de Texto
- Técnicas de Embedding
- Processamento de Linguagem Natural (PNL)
- Inteligência Artificial (IA)
- LangChain
- OpenAI GPT-4
- HuggingFace Embeddings
- ChromaDB
- Python

Este repositório demonstra expertise na construção de sistemas de perguntas e respostas inteligentes utilizando técnicas de RAG, vetorização e embedding. É ideal para empresas e recrutadores que buscam profissionais com habilidades em PNL, IA e desenvolvimento de soluções de busca e recuperação de informações.

## Fontes

- [medium.com/@onkarmishra/using-langchain-for-question-answering-on-own-data-3af0a82789ed](https://medium.com/@onkarmishra/using-langchain-for-question-answering-on-own-data-3af0a82789ed)
- [adasci.org/build-a-question-answering-pipeline-with-weaviate-vector-store-and-langchain/](https://adasci.org/build-a-question-answering-pipeline-with-weaviate-vector-store-and-langchain/)
- [medium.com/@aneesha161994/a-z-of-rag-question-answering-methods-in-langchain-0b0d2464c61d](https://medium.com/@aneesha161994/a-z-of-rag-question-answering-methods-in-langchain-0b0d2464c61d)
- [www.analyticsvidhya.com/blog/2023/12/building-a-rag-pipeline-for-semi-structured-data-with-langchain/](https://www.analyticsvidhya.com/blog/2023/12/building-a-rag-pipeline-for-semi-structured-data-with-langchain/)
