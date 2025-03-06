# langchain_study

### langchain_tut_1.ipynb
 - prompt 생성
   ``` python
   from langchain import PromptTemplate
 - LLM 호출
   ``` python
   from langchain.chat_models import ChatOpenAI
 - 모델성능비교
   ``` python
   from langchain.model_laboratory import ModelLaboratory
   
### langchain_tut_2.ipynb
- data 연결
  ``` python
  #라이브리러 설치
  !pip install langchain
  !pip install openai
  !pip install pypdf
  !pip install tiktoken
  !pip install faiss-cpu
  !pip install sentence_transformers

- PDF 불러오기
  ``` python
  from langchain.document_loaders import PyPDFLoader

- Embedding
  ``` python
  # openai Embeddings
  from langchain.vectorstores import FAISS
  from langchain.embeddings import OpenAIEmbeddings

  # HuggingFaceEmbeddings
  from langchain.embeddings import HuggingFaceEmbeddings

- 검색기(retriever)활용
  ``` python
  from langchain.chains import RetrievalQA

- chain
  ``` python
  from langchain.chains import LLMChain

- memory
  ``` python
  from langchain.chains import ConversationChain

### langchain_tut_3.ipynb
- agent / tool
  ``` python
  # 라이브러리 설치
  !pip install wikipedia
  !pip install numexpr

  # 라이브러리 불러오기  
  from langchain.agents import load_tools
  from langchain.agents import initialize_agent
  from langchain.agents import AgentType


  
