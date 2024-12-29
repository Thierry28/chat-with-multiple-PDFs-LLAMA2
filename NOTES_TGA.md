ollama pull llama2:70b-chat
    pulling manifest 
    pulling manifest 
    pulling manifest 
    pulling 68bbe6dc9cf4... 100% ▕█████████████████████████████████████████████████████████▏  38 GB                         
    pulling 8c17c2ebb0ea... 100% ▕█████████████████████████████████████████████████████████▏ 7.0 KB                         
    pulling 7c23fb36d801... 100% ▕█████████████████████████████████████████████████████████▏ 4.8 KB                         
    pulling 2e0493f67d0c... 100% ▕█████████████████████████████████████████████████████████▏   59 B                         
    pulling fa304d675061... 100% ▕█████████████████████████████████████████████████████████▏   91 B                         
    pulling 7c96b46dca6c... 100% ▕█████████████████████████████████████████████████████████▏  558 B                         
    verifying sha256 digest 
    writing manifest 
    success 

conda create -n chat-with-pdf python=3.9
conda activate chat-with-pdf

To deactivate an active environment, 
$ conda deactivate

pip install -r requirements.txt

pip install streamlit
pip install python-dotenv
pip install PyPDF2
pip install langchain
pip install -U langchain-community

pip install pycryptodome

ollama pull llama2:70b-chat
ollama list 

streamlit run app.py


 You can now view your Streamlit app in your browser.

  Local URL: http://localhost:8501
  Network URL: http://192.168.1.103:8501

  For better performance, install the Watchdog module:

  $ xcode-select --install
  $ pip install watchdog
            
/Users/thierryg/Documents/PROJETS/RAG/chat-with-multiple-PDFs-LLAMA2/app.py:5: LangChainDeprecationWarning: Importing OllamaEmbeddings from langchain.embeddings is deprecated. Please replace deprecated imports:

>> from langchain.embeddings import OllamaEmbeddings

with new imports of:

>> from langchain_community.embeddings import OllamaEmbeddings
You can use the langchain cli to **automatically** upgrade many imports. Please see documentation here <https://python.langchain.com/docs/versions/v0_2/>
  from langchain.embeddings import OllamaEmbeddings
/Users/thierryg/Documents/PROJETS/RAG/chat-with-multiple-PDFs-LLAMA2/app.py:6: LangChainDeprecationWarning: Importing FAISS from langchain.vectorstores is deprecated. Please replace deprecated imports:

>> from langchain.vectorstores import FAISS

with new imports of:

>> from langchain_community.vectorstores import FAISS
You can use the langchain cli to **automatically** upgrade many imports. Please see documentation here <https://python.langchain.com/docs/versions/v0_2/>
  from langchain.vectorstores import FAISS
/opt/anaconda3/envs/chat-with-pdf/lib/python3.9/site-packages/langchain/chat_models/__init__.py:33: LangChainDeprecationWarning: Importing chat models from langchain is deprecated. Importing from langchain will no longer be supported as of langchain==0.2.0. Please import from langchain-community instead:

`from langchain_community.chat_models import ChatOllama`.

To install langchain-community run `pip install -U langchain-community`.
  warnings.warn(
Starting Streamlit app...
Loaded environment variables
/Users/thierryg/Documents/PROJETS/RAG/chat-with-multiple-PDFs-LLAMA2/app.py:5: LangChainDeprecationWarning: Importing OllamaEmbeddings from langchain.embeddings is deprecated. Please replace deprecated imports:

>> from langchain.embeddings import OllamaEmbeddings

with new imports of:

>> from langchain_community.embeddings import OllamaEmbeddings
You can use the langchain cli to **automatically** upgrade many imports. Please see documentation here <https://python.langchain.com/docs/versions/v0_2/>
  from langchain.embeddings import OllamaEmbeddings
/Users/thierryg/Documents/PROJETS/RAG/chat-with-multiple-PDFs-LLAMA2/app.py:6: LangChainDeprecationWarning: Importing FAISS from langchain.vectorstores is deprecated. Please replace deprecated imports:

>> from langchain.vectorstores import FAISS

with new imports of:

>> from langchain_community.vectorstores import FAISS
You can use the langchain cli to **automatically** upgrade many imports. Please see documentation here <https://python.langchain.com/docs/versions/v0_2/>
  from langchain.vectorstores import FAISS
/opt/anaconda3/envs/chat-with-pdf/lib/python3.9/site-packages/langchain/chat_models/__init__.py:33: LangChainDeprecationWarning: Importing chat models from langchain is deprecated. Importing from langchain will no longer be supported as of langchain==0.2.0. Please import from langchain-community instead:

`from langchain_community.chat_models import ChatOllama`.

To install langchain-community run `pip install -U langchain-community`.
  warnings.warn(
Starting Streamlit app...
Loaded environment variables
/Users/thierryg/Documents/PROJETS/RAG/chat-with-multiple-PDFs-LLAMA2/app.py:5: LangChainDeprecationWarning: Importing OllamaEmbeddings from langchain.embeddings is deprecated. Please replace deprecated imports:

>> from langchain.embeddings import OllamaEmbeddings

with new imports of:

>> from langchain_community.embeddings import OllamaEmbeddings
You can use the langchain cli to **automatically** upgrade many imports. Please see documentation here <https://python.langchain.com/docs/versions/v0_2/>
  from langchain.embeddings import OllamaEmbeddings
/Users/thierryg/Documents/PROJETS/RAG/chat-with-multiple-PDFs-LLAMA2/app.py:6: LangChainDeprecationWarning: Importing FAISS from langchain.vectorstores is deprecated. Please replace deprecated imports:

>> from langchain.vectorstores import FAISS

with new imports of:

>> from langchain_community.vectorstores import FAISS
You can use the langchain cli to **automatically** upgrade many imports. Please see documentation here <https://python.langchain.com/docs/versions/v0_2/>
  from langchain.vectorstores import FAISS
Starting Streamlit app...
Loaded environment variables
Processing PDFs...

Function get_pdf_text Took 0.1531 seconds
Processing text...
Splitting text into chunks...
Length of text: 18482

Function get_text_chunks Took 0.0002 seconds
Processing vector store...
Creating vector store...
Number of text chunks: 23
/Users/thierryg/Documents/PROJETS/RAG/chat-with-multiple-PDFs-LLAMA2/app.py:59: LangChainDeprecationWarning: The class `OllamaEmbeddings` was deprecated in LangChain 0.3.1 and will be removed in 1.0.0. An updated version of the class exists in the :class:`~langchain-ollama package and should be used instead. To use it run `pip install -U :class:`~langchain-ollama` and import as `from :class:`~langchain_ollama import OllamaEmbeddings``.
  embeddings = OllamaEmbeddings(
2024-12-29 18:09:27.436 Uncaught app execution
Traceback (most recent call last):
  File "/opt/anaconda3/envs/chat-with-pdf/lib/python3.9/site-packages/streamlit/runtime/scriptrunner/exec_code.py", line 88, in exec_func_with_error_handling
    result = func()
  File "/opt/anaconda3/envs/chat-with-pdf/lib/python3.9/site-packages/streamlit/runtime/scriptrunner/script_runner.py", line 579, in code_to_exec
    exec(code, module.__dict__)
  File "/Users/thierryg/Documents/PROJETS/RAG/chat-with-multiple-PDFs-LLAMA2/app.py", line 148, in <module>
    main()
  File "/Users/thierryg/Documents/PROJETS/RAG/chat-with-multiple-PDFs-LLAMA2/app.py", line 140, in main
    vectorstore = get_vectorstore(text_chunks)
  File "/Users/thierryg/Documents/PROJETS/RAG/chat-with-multiple-PDFs-LLAMA2/app.py", line 22, in timeit_wrapper
    result = func(*args, **kwargs)
  File "/Users/thierryg/Documents/PROJETS/RAG/chat-with-multiple-PDFs-LLAMA2/app.py", line 63, in get_vectorstore
    vectorstore = FAISS.from_texts(texts=text_chunks, embedding=embeddings)
  File "/opt/anaconda3/envs/chat-with-pdf/lib/python3.9/site-packages/langchain_community/vectorstores/faiss.py", line 1043, in from_texts
    embeddings = embedding.embed_documents(texts)
  File "/opt/anaconda3/envs/chat-with-pdf/lib/python3.9/site-packages/langchain_community/embeddings/ollama.py", line 214, in embed_documents
    embeddings = self._embed(instruction_pairs)
  File "/opt/anaconda3/envs/chat-with-pdf/lib/python3.9/site-packages/langchain_community/embeddings/ollama.py", line 202, in _embed
    return [self._process_emb_response(prompt) for prompt in iter_]
  File "/opt/anaconda3/envs/chat-with-pdf/lib/python3.9/site-packages/langchain_community/embeddings/ollama.py", line 202, in <listcomp>
    return [self._process_emb_response(prompt) for prompt in iter_]
  File "/opt/anaconda3/envs/chat-with-pdf/lib/python3.9/site-packages/langchain_community/embeddings/ollama.py", line 176, in _process_emb_response
    raise ValueError(
ValueError: Error raised by inference API HTTP code: 404, {"error":"model \"llama2\" not found, try pulling it first"}
