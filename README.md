# Atividade HuggingFace - RAG

Este projeto foi desenvolvido para a atividade semanal sobre HuggingFace.

## Tema escolhido

RAG - Retrieval Augmented Generation.

## Objetivo

Criar uma pequena aplicação em Python capaz de responder perguntas com base em uma base de textos curta. A ideia é simular um sistema que busca trechos relevantes em documentos e usa um modelo do HuggingFace para responder.

## Problema

Modelos de IA podem gerar respostas genéricas ou incorretas quando não recebem contexto suficiente. O RAG reduz esse problema ao combinar recuperação de informação com geração ou extração de resposta.

## Solução desenvolvida

A aplicação faz o seguinte fluxo:

1. Cria uma pequena base de conhecimento com textos sobre Inteligência Artificial.
2. Usa embeddings com `sentence-transformers` para representar os textos numericamente.
3. Recebe uma pergunta do usuário.
4. Busca o trecho mais parecido com a pergunta.
5. Usa um modelo de Question Answering do HuggingFace para gerar a resposta final com base no trecho encontrado.

## Tecnologias utilizadas

- Python
- Jupyter Notebook
- HuggingFace Transformers
- Sentence Transformers
- Scikit-learn

## Arquivos

- `atividade_rag_huggingface.ipynb`: notebook com o código da aplicação.
- `apresentacao_rag_huggingface.pdf`: apresentação em PDF com 3 slides.
- `apresentacao_rag_huggingface.pptx`: versão editável dos slides.
- `README.md`: explicação do projeto.

## Como executar

No Google Colab ou Jupyter Notebook, execute as células do arquivo `atividade_rag_huggingface.ipynb`.

Caso esteja no Colab, a primeira célula instala as bibliotecas necessárias:

```python
!pip install transformers sentence-transformers scikit-learn torch
```

Depois, basta rodar todas as células e testar perguntas como:

```python
responder("O que é RAG?")
responder("Para que servem embeddings?")
responder("O que é o HuggingFace?")
```

## Integrantes
- Larissa Carvalho Pavan
- Beatriz Mayumi Fernandez de Oliveira
- Thiago Alves Serra
- Guilherme Bezerra de Carvalho
- Samuel Freitas Ribeiro de Castro

## Referências

- HuggingFace: https://huggingface.co/
- HuggingFace Transformers: https://huggingface.co/docs/transformers
- Sentence Transformers: https://www.sbert.net/
- Modelo de embeddings: https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2
- Modelo de Question Answering em português: https://huggingface.co/pierreguillou/bert-base-cased-squad-v1.1-portuguese
