RAG - Financial Law Question Answering System

Hệ thống Retrieval-Augmented Generation (RAG) hỗ trợ truy vấn và hỏi đáp trên các tài liệu luật tài chính Việt Nam bằng ngôn ngữ tự nhiên.

Công nghệ sử dụng
Python 3.12
LangChain
PhoBERT
ChromaDB
HyDE (Hypothetical Document Embedding)
Gemini/OpenAI API
Kiến trúc hệ thống
Documents → Chunking → PhoBERT Embeddings → ChromaDB
                                  ↑
User Query → HyDE → Retriever (MMR) → Summarization → Final Answer
Tính năng
Truy xuất tài liệu dựa trên ngữ nghĩa.
Mở rộng truy vấn bằng HyDE để tăng độ chính xác.
Tìm kiếm tài liệu liên quan với Similarity Search và MMR.
Tổng hợp thông tin từ nhiều nguồn bằng LLM.
Giảm hallucination nhờ kiến trúc RAG.
Cài đặt
1. Tạo môi trường ảo
virtualenv --python=3.12 env-3.12
2. Kích hoạt môi trường

Windows

.\env-3.12\Scripts\activate

MacOS/Linux

source env-3.12/bin/activate
3. Cài đặt thư viện
pip install -r requirements.txt
4. Chạy ứng dụng
python main.py
Kết quả
Tăng độ chính xác truy xuất tài liệu bằng HyDE.
Giảm thông tin trùng lặp với MMR.
Hỗ trợ tra cứu văn bản luật tài chính nhanh chóng và hiệu quả.
