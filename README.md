# AzureCognitiveSearch
Projeto da DIO, com o objetivo de aplicar técnicas de organização e pesquisa de documentos por meio da ingestão de dados e indexação utilizando ferramentas de inteligência artificial
# **Relatório do Desafio: Organização e Pesquisa de Documentos com IA**  

## **1. Introdução**  
Este desafio teve como objetivo aplicar técnicas de **ingestão de dados, indexação inteligente e exploração de documentos** utilizando ferramentas de IA. O processo envolveu a organização de grandes volumes de informação para permitir buscas eficientes e extração de conhecimento.  


---

## **2. Etapas Realizadas**  

### **2.1. Ingestão de Conteúdo para IA**  
- **Fonte de dados**: Utilizamos documentos em formato `.txt`, `.pdf` e `.csv`.  
- **Ferramentas**:  
  - **LangChain** para carregamento e processamento de texto.  
  - **PyPDF2** para extração de conteúdo de arquivos PDF.  
- **Processo**:  
  - Os documentos foram carregados e pré-processados (remoção de stopwords, tokenização).  
  - Dados estruturados foram armazenados em um banco de dados vetorial (FAISS).  

### **2.2. Criação de Índices Inteligentes**  
- **Embeddings**: Usamos o modelo **OpenAI Embeddings** para transformar texto em vetores.  
- **Indexação**:  
  - Os vetores foram armazenados em um **índice FAISS** para buscas semânticas rápidas.  
  - Implementamos um sistema de **RAG (Retrieval-Augmented Generation)** para melhorar respostas com base no contexto.  

### **2.3. Exploração Prática dos Dados**  
- **Busca Semântica**: Realizamos consultas usando similaridade de cosseno para encontrar documentos relevantes.  
- **Visualização**: Utilizamos **PCA** para reduzir a dimensionalidade e plotar os embeddings em 2D.  

---

## **3. Insights Obtidos**  
- **Eficiência na Busca**: A indexação com FAISS permitiu respostas rápidas mesmo em grandes volumes de dados.  
- **Desafios**:  
  - Pré-processamento de PDFs com tabelas exigiu ajustes adicionais.  
  - Modelos de embeddings podem ter custo elevado em escala.  

---

## **4. Conclusão**  
Este projeto demonstrou como técnicas de IA podem melhorar a organização e recuperação de documentos. A combinação de **ingestão automatizada, indexação vetorial e busca semântica** mostrou-se eficaz para extrair conhecimento de dados não estruturados.  

**Próximos passos**:  
- Implementar um frontend para consultas interativas.  
- Explorar fine-tuning de modelos para domínios específicos.  

---

## **5. Referências**  
Documentação do LangChain.

Tutoriais sobre FAISS e OpenAI Embeddings.
