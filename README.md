# 🗂️ LlamaIndex 🦙

[![PyPI - Downloads](https://img.shields.io/pypi/dm/llama-index)](https://pypi.org/project/llama-index/)
[![Build](https://github.com/run-llama/llama_index/actions/workflows/build_package.yml/badge.svg)](https://github.com/run-llama/llama_index/actions/workflows/build_package.yml)
[![GitHub contributors](https://img.shields.io/github/contributors/jerryjliu/llama_index)](https://github.com/jerryjliu/llama_index/graphs/contributors)
[![Discord](https://img.shields.io/discord/1059199217496772688)](https://discord.gg/dGcwcsnxhU)
[![Twitter](https://img.shields.io/twitter/follow/llama_index)](https://x.com/llama_index)
[![Reddit](https://img.shields.io/reddit/subreddit-subscribers/LlamaIndex?style=plastic&logo=reddit&label=r%2FLlamaIndex&labelColor=white)](https://www.reddit.com/r/LlamaIndex/)
[![Ask AI](https://img.shields.io/badge/Phorm-Ask_AI-%23F2777A.svg?&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNSIgaGVpZ2h0PSI0IiBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxwYXRoIGQ9Ik00LjQzIDEuODgyYTEuNDQgMS40NCAwIDAgMS0uMDk4LjQyNmMtLjA1LjEyMy0uMTE1LjIzLS4xOTIuMzIyLS4wNzUuMDktLjE2LjE2NS0uMjU1LjIyNmExLjM1MyAxLjM1MyAwIDAgMS0uNTk1LjIxMmMtLjA5OS4wMTItLjE5Mi4wMTQtLjI3OS4wMDZsLTEuNTkzLS4xNHYtLjQwNmgxLjY1OGMuMDkuMDAxLjE3LS4xNjkuMjQ2LS4xOTFhLjYwMy42MDMgMCAwIDAgLjItLjEwNi41MjkuNTI5IDAgMCAwIC4xMzgtLjE3LjY1NC42NTQgMCAwIDAgLjA2NS0uMjRsLjAyOC0uMzJhLjkzLjkzIDAgMCAwLS4wMzYtLjI0OS41NjcuNTY3IDAgMCAwLS4xMDMtLjIuNTAyLjUwMiAwIDAgMC0uMTY4LS4xMzguNjA4LjYwOCAwIDAgMC0uMjQtLjA2N0wyLjQzNy43MjkgMS42MjUuNjcxYS4zMjIuMzIyIDAgMCAwLS4yMzIuMDU4LjM3NS4zNzUgMCAwIDAtLjExNi4yMzJsLS4xMTYgMS40NS0uMDU4LjY5Ny0uMDU4Ljc1NEwuNzA1IDRsLS4zNTctLjA3OUwuNjAyLjkwNkMuNjE3LjcyNi42NjMuNTc0LjczOS40NTRhLjk1OC45NTggMCAwIDEgLjI3NC0uMjg1Ljk3MS45NzEgMCAwIDEgLjMzNy0uMTRjLjExOS0uMDI2LjIyNy0uMDM0LjMyNS0uMDI2TDMuMjMyLjE2Yy4xNTkuMDE0LjMzNi4wMy40NTkuMDgyYTEuMTczIDEuMTczIDAgMCAxIC41NDUuNDQ3Yy4wNi4wOTQuMTA5LjE5Mi4xNDQuMjkzYTEuMzkyIDEuMzkyIDAgMCAxIC4wNzguNThsLS4wMjkuMzJaIiBmaWxsPSIjRjI3NzdBIi8+CiAgPHBhdGggZD0iTTQuMDgyIDIuMDA3YTEuNDU1IDEuNDU1IDAgMCAxLS4wOTguNDI3Yy0uMDUuMTI0LS4xMTQuMjMyLS4xOTIuMzI0YTEuMTMgMS4xMyAwIDAgMS0uMjU0LjIyNyAxLjM1MyAxLjM1MyAwIDAgMS0uNTk1LjIxNGMtLjEuMDEyLS4xOTMuMDE0LS4yOC4wMDZsLTEuNTYtLjEwOC4wMzQtLjQwNi4wMy0uMzQ4IDEuNTU5LjE1NGMuMDkgMCAuMTczLS4wMS4yNDgtLjAzM2EuNjAzLjYwMyAwIDAgMCAuMi0uMTA2LjUzMi41MzIgMCAwIDAgLjEzOS0uMTcyLjY2LjY2IDAgMCAwIC4wNjQtLjI0MWwuMDI5LS4zMjFhLjk0Ljk0IDAgMCAwLS4wMzYtLjI1LjU3LjU3IDAgMCAwLS4xMDMtLjIwMi41MDIuNTAyIDAgMCAwLS4xNjgtLjEzOC42MDUuNjA1IDAgMCAwLS4yNC0uMDY3TDEuMjczLjgyN2MtLjA5NC0uMDA4LS4xNjguMDEtLjIyMS4wNTUtLjA1My4wNDUtLjA4NC4xMTQtLjA5Mi4yMDZMLjcwNSA0IDAgMy45MzhsLjI1NS0yLjkxMUExLjAxIDEuMDEgMCAwIDEgLjM5My41NzIuOTYyLjk2MiAwIDAgMSAuNjY2LjI4NmEuOTcuOTcgMCAwIDEgLjMzOC0uMTRDMS4xMjIuMTIgMS4yMy4xMSAxLjMyOC4xMTlsMS41OTMuMTRjLjE2LjAxNC4zLjA0Ny40MjMuMWExLjE3IDEuMTcgMCAwIDEgLjU0NS40NDhjLjA2MS4wOTUuMTA5LjE5My4xNDQuMjk1YTEuNDA2IDEuNDA2IDAgMCAxIC4wNzcuNTgzbC0uMDI4LjMyMloiIGZpbGw9IndoaXRlIi8+CiAgPHBhdGggZD0iTTQuMDgyIDIuMDA3YTEuNDU1IDEuNDU1IDAgMCAxLS4wOTguNDI3Yy0uMDUuMTI0LS4xMTQuMjMyLS4xOTIuMzI0YTEuMTMgMS4xMyAwIDAgMS0uMjU0LjIyNyAxLjM1MyAxLjM1MyAwIDAgMS0uNTk1LjIxNGMtLjEuMDEyLS4xOTMuMDE0LS4yOC4wMDZsLTEuNTYtLjEwOC4wMzQtLjQwNi4wMy0uMzQ4IDEuNTU5LjE1NGMuMDkgMCAuMTczLS4wMS4yNDgtLjAzM2EuNjAzLjYwMyAwIDAgMCAuMi0uMTA2LjUzMi41MzIgMCAwIDAgLjEzOS0uMTcyLjY2LjY2IDAgMCAwIC4wNjQtLjI0MWwuMDI5LS4zMjFhLjk0Ljk0IDAgMCAwLS4wMzYtLjI1LjU3LjU3IDAgMCAwLS4xMDMtLjIwMi41MDIuNTAyIDAgMCAwLS4xNjgtLjEzOC42MDUuNjA1IDAgMCAwLS4yNC0uMDY3TDEuMjczLjgyN2MtLjA5NC0uMDA4LS4xNjguMDEtLjIyMS4wNTUtLjA1My4wNDUtLjA4NC4xMTQtLjA5Mi4yMDZMLjcwNSA0IDAgMy45MzhsLjI1NS0yLjkxMUExLjAxIDEuMDEgMCAwIDEgLjM5My41NzIuOTYyLjk2MiAwIDAgMSAuNjY2LjI4NmEuOTcuOTcgMCAwIDEgLjMzOC0uMTRDMS4xMjIuMTIgMS4yMy4xMSAxLjMyOC4xMTlsMS41OTMuMTRjLjE2LjAxNC4zLjA0Ny40MjMuMWExLjE3IDEuMTcgMCAwIDEgLjU0NS40NDhjLjA2MS4wOTUuMTA5LjE5My4xNDQuMjk1YTEuNDA2IDEuNDA2IDAgMCAxIC4wNzcuNTgzbC0uMDI4LjMyMloiIGZpbGw9IndoaXRlIi8+Cjwvc3ZnPgo=)](https://www.phorm.ai/query?projectId=c5863b56-6703-4a5d-87b6-7e6031bf16b6)

LlamaIndex (GPT Index) is a data framework for your LLM application. Building with LlamaIndex typically involves working with LlamaIndex core and a chosen set of integrations (or plugins). There are two ways to start building with LlamaIndex in
Python:

1. **Starter**: [`llama-index`](https://pypi.org/project/llama-index/). A starter Python package that includes core LlamaIndex as well as a selection of integrations.

2. **Customized**: [`llama-index-core`](https://pypi.org/project/llama-index-core/). Install core LlamaIndex and add your chosen LlamaIndex integration packages on [LlamaHub](https://llamahub.ai/)
   that are required for your application. There are over 300 LlamaIndex integration
   packages that work seamlessly with core, allowing you to build with your preferred
   LLM, embedding, and vector store providers.

The LlamaIndex Python library is namespaced such that import statements which
include `core` imply that the core package is being used. In contrast, those
statements without `core` imply that an integration package is being used.

```python
# typical pattern
from llama_index.core.xxx import ClassABC  # core submodule xxx
from llama_index.xxx.yyy import (
    SubclassABC,
)  # integration yyy for submodule xxx

# concrete example
from llama_index.core.llms import LLM
from llama_index.llms.openai import OpenAI
```

### Important Links

LlamaIndex.TS [(Typescript/Javascript)](https://github.com/run-llama/LlamaIndexTS)

[Documentation](https://docs.llamaindex.ai/en/stable/)

[X (formerly Twitter)](https://x.com/llama_index)

[LinkedIn](https://www.linkedin.com/company/llamaindex/)

[Reddit](https://www.reddit.com/r/LlamaIndex/)

[Discord](https://discord.gg/dGcwcsnxhU)

### Ecosystem

- LlamaHub [(community library of data loaders)](https://llamahub.ai)
- LlamaLab [(cutting-edge AGI projects using LlamaIndex)](https://github.com/run-llama/llama-lab)

## 🚀 Overview

**NOTE**: This README is not updated as frequently as the documentation. Please check out the documentation above for the latest updates!

### Context

- LLMs are a phenomenal piece of technology for knowledge generation and reasoning. They are pre-trained on large amounts of publicly available data.
- How do we best augment LLMs with our own private data?

We need a comprehensive toolkit to help perform this data augmentation for LLMs.

### Proposed Solution

That's where **LlamaIndex** comes in. LlamaIndex is a "data framework" to help you build LLM apps. It provides the following tools:

- Offers **data connectors** to ingest your existing data sources and data formats (APIs, PDFs, docs, SQL, etc.).
- Provides ways to **structure your data** (indices, graphs) so that this data can be easily used with LLMs.
- Provides an **advanced retrieval/query interface over your data**: Feed in any LLM input prompt, get back retrieved context and knowledge-augmented output.
- Allows easy integrations with your outer application framework (e.g. with LangChain, Flask, Docker, ChatGPT, or anything else).

LlamaIndex provides tools for both beginner users and advanced users. Our high-level API allows beginner users to use LlamaIndex to ingest and query their data in
5 lines of code. Our lower-level APIs allow advanced users to customize and extend any module (data connectors, indices, retrievers, query engines, reranking modules),
to fit their needs.

## 💡 Contributing

Interested in contributing? Contributions to LlamaIndex core as well as contributing
integrations that build on the core are both accepted and highly encouraged! See our [Contribution Guide](CONTRIBUTING.md) for more details.

New integrations should meaningfully integrate with existing LlamaIndex framework components. At the discretion of LlamaIndex maintainers, some integrations may be declined.

## 📄 Documentation

Full documentation can be found [here](https://docs.llamaindex.ai/en/latest/)

Please check it out for the most up-to-date tutorials, how-to guides, references, and other resources!

## 💻 Example Usage

```sh
# custom selection of integrations to work with core
pip install llama-index-core
pip install llama-index-llms-openai
pip install llama-index-llms-replicate
pip install llama-index-embeddings-huggingface
```

Examples are in the `docs/examples` folder. Indices are in the `indices` folder (see list of indices below).

To build a simple vector store index using OpenAI:

```python
import os

os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"

from llama_index.core import VectorStoreIndex, SimpleDirectoryReader

documents = SimpleDirectoryReader("YOUR_DATA_DIRECTORY").load_data()
index = VectorStoreIndex.from_documents(documents)
```

To build a simple vector store index using non-OpenAI LLMs, e.g. Llama 2 hosted on [Replicate](https://replicate.com/), where you can easily create a free trial API token:

```python
import os

os.environ["REPLICATE_API_TOKEN"] = "YOUR_REPLICATE_API_TOKEN"

from llama_index.core import Settings, VectorStoreIndex, SimpleDirectoryReader
from llama_index.embeddings.huggingface import HuggingFaceEmbedding
from llama_index.llms.replicate import Replicate
from transformers import AutoTokenizer

# set the LLM
llama2_7b_chat = "meta/llama-2-7b-chat:8e6975e5ed6174911a6ff3d60540dfd4844201974602551e10e9e87ab143d81e"
Settings.llm = Replicate(
    model=llama2_7b_chat,
    temperature=0.01,
    additional_kwargs={"top_p": 1, "max_new_tokens": 300},
)

# set tokenizer to match LLM
Settings.tokenizer = AutoTokenizer.from_pretrained(
    "NousResearch/Llama-2-7b-chat-hf"
)

# set the embed model
Settings.embed_model = HuggingFaceEmbedding(
    model_name="BAAI/bge-small-en-v1.5"
)

documents = SimpleDirectoryReader("YOUR_DATA_DIRECTORY").load_data()
index = VectorStoreIndex.from_documents(
    documents,
)
```

To query:

```python
query_engine = index.as_query_engine()
query_engine.query("YOUR_QUESTION")
```

By default, data is stored in-memory.
To persist to disk (under `./storage`):

```python
index.storage_context.persist()
```

To reload from disk:

```python
from llama_index.core import StorageContext, load_index_from_storage

# rebuild storage context
storage_context = StorageContext.from_defaults(persist_dir="./storage")
# load index
index = load_index_from_storage(storage_context)
```

## 🔧 Dependencies

We use poetry as the package manager for all Python packages. As a result, the
dependencies of each Python package can be found by referencing the `pyproject.toml`
file in each of the package's folders.

```bash
cd <desired-package-folder>
pip install poetry
poetry install --with dev
```

## 📖 Citation

Reference to cite if you use LlamaIndex in a paper:

```
@software{Liu_LlamaIndex_2022,
author = {Liu, Jerry},
doi = {10.5281/zenodo.1234},
month = {11},
title = {{LlamaIndex}},
url = {https://github.com/jerryjliu/llama_index},
year = {2022}
}
```


LlamaIndex là gì?
LlamaIndex (trước đây gọi là GPT Index) là một framework (khung công cụ) giúp bạn dễ dàng xây dựng các ứng dụng sử dụng trí tuệ nhân tạo (AI) kiểu LLM (Large Language Model, ví dụ như ChatGPT) với dữ liệu riêng của bạn.

Vấn đề mà LlamaIndex giải quyết
Các mô hình AI lớn như ChatGPT thường chỉ biết những gì được huấn luyện (thường là dữ liệu công khai, đến một thời điểm nhất định). Nếu bạn muốn AI “hiểu” hoặc trả lời các câu hỏi dựa trên dữ liệu nội bộ, tài liệu cá nhân, file PDF, database, hay website riêng,... thì cần một cách kết nối dữ liệu của bạn vào AI.
Đó chính là lý do ra đời của LlamaIndex.

Tính năng nổi bật
LlamaIndex cung cấp cho bạn:

Kết nối dữ liệu (data connectors): Kết nối với nhiều nguồn dữ liệu khác nhau như file PDF, doc, dữ liệu SQL, API, Google Drive,...

Tổ chức dữ liệu thông minh: Chuyển dữ liệu thành dạng mà AI dễ sử dụng (chẳng hạn lưu thành chỉ mục/vector để tìm kiếm nhanh).

Tìm kiếm, truy xuất thông minh: Hỏi gì cũng được, AI sẽ tự động lấy thông tin liên quan nhất từ dữ liệu của bạn để trả lời.

Dễ dàng tích hợp vào các ứng dụng: Bạn có thể dùng LlamaIndex cùng với LangChain, Flask, Docker, ChatGPT, hoặc tự xây dựng ứng dụng riêng.

Ai nên dùng?
Người mới (beginner):
Bạn chỉ cần vài dòng code là có thể “nạp” dữ liệu và bắt đầu hỏi AI rồi.

Người có kinh nghiệm (advanced):
LlamaIndex cho phép bạn tuỳ chỉnh sâu từng phần, mở rộng thêm các module riêng.

Cách hoạt động tổng quát
Nạp dữ liệu: Đưa dữ liệu của bạn (file, database, v.v.) vào LlamaIndex qua các data connectors.

Tạo chỉ mục (index): LlamaIndex chuyển dữ liệu sang dạng mà AI dễ sử dụng (ví dụ, lưu thành các vector để sau này tìm kiếm nhanh).

Truy vấn (query): Khi bạn nhập câu hỏi, LlamaIndex sẽ tìm kiếm phần dữ liệu phù hợp nhất, gửi cho AI để trả lời chính xác theo “kiến thức riêng” của bạn.

Ví dụ cơ bản (Python)
1. Cài đặt
sh
Sao chép
Chỉnh sửa
pip install llama-index
2. Sử dụng với OpenAI (ChatGPT)
python
Sao chép
Chỉnh sửa
import os
from llama_index.core import VectorStoreIndex, SimpleDirectoryReader

os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"  # Thay bằng API key của bạn

documents = SimpleDirectoryReader("THU_MUC_DU_LIEU_CUA_BAN").load_data()
index = VectorStoreIndex.from_documents(documents)

query_engine = index.as_query_engine()
result = query_engine.query("Nội dung câu hỏi của bạn")
print(result)
3. Lưu lại chỉ mục để dùng về sau
python
Sao chép
Chỉnh sửa
index.storage_context.persist()  # Lưu index xuống ổ cứng
4. Tải lại chỉ mục
python
Sao chép
Chỉnh sửa
from llama_index.core import StorageContext, load_index_from_storage

storage_context = StorageContext.from_defaults(persist_dir="./storage")
index = load_index_from_storage(storage_context)
Tóm tắt ý nghĩa
LlamaIndex giống như một “bộ não phụ trợ” giúp AI hiểu được dữ liệu riêng của bạn.

Dễ tích hợp, nhiều plugin, tài liệu hướng dẫn rõ ràng.

Hỗ trợ cả người mới và chuyên gia xây dựng sản phẩm AI dựa trên dữ liệu riêng.

Tài liệu, cộng đồng
Tài liệu chính thức

LlamaHub (kho plugin tải dữ liệu)

Discord cộng đồng

Nếu bạn mới fork repo này, có thể bắt đầu đọc các ví dụ trong mục docs/examples, tham khảo tài liệu hướng dẫn chi tiết, và thử “nạp” dữ liệu của mình vào để hỏi AI nhé!


1. Tổng quan: LlamaIndex so với các hệ thống RAG khác
LlamaIndex thực chất là một bộ framework chuyên sâu dành riêng cho việc xây dựng ứng dụng RAG, trong khi nhiều hệ thống RAG khác chỉ cung cấp một số thành phần cơ bản, hoặc là các giải pháp “all-in-one” ít tùy biến hơn.

Các hệ thống RAG phổ biến bạn có thể đã tìm hiểu như:

LangChain

Haystack (deepset.ai)

Chroma / Weaviate / Milvus / Qdrant (chủ yếu là vector DB, nhưng đều có thể làm RAG với plugin)

OpenAI Cookbook/ RAG sample / Llama-Index

Điểm giống nhau
Đều xây dựng pipeline với các bước cơ bản: nạp dữ liệu → tạo vector → tìm kiếm → trả về kết quả cho LLM trả lời.

Đều hỗ trợ nhiều nguồn dữ liệu, vector DB, các LLM khác nhau.

2. Điểm khác biệt nổi bật của LlamaIndex
A. Khác biệt về mục tiêu và kiến trúc
Tiêu chí	LlamaIndex	LangChain/Haystack	VectorDB (Chroma, Qdrant,...)
Mục tiêu	Framework tập trung RAG, linh hoạt	General orchestration (workflow, agent, RAG, tool-use,...)	Lưu trữ & tìm kiếm vector
Khả năng custom pipeline	Mạnh, nhiều level tuỳ biến	Rất mạnh (nhưng nhiều thành phần, dễ “loãng”)	Chỉ làm phần truy xuất
Dễ dùng cho người mới	Cao, nhiều API high-level, ít code	Nhiều bước, dễ “overwhelm”	Không đủ cho người mới tự làm RAG

B. LlamaIndex nổi bật ở chỗ nào?
Modular & Plug & Play:

LlamaIndex chia rõ “core” và “plugin/integration”.

Bạn chỉ cần cài những module cần thiết (ví dụ: LLM, embedding, retriever, loader cho từng nguồn dữ liệu), tiết kiệm dung lượng và phù hợp nhu cầu.

Cộng đồng mạnh & kho plugin lớn nhất:

LlamaHub có hơn 300 plugin để nạp dữ liệu từ nhiều nguồn độc-lạ nhất (PDF, notion, SQL, các tool SaaS,...).

Luôn cập nhật plugin mới, dễ góp code.

API nhiều cấp độ:

API “5 dòng code”: Dành cho người mới, chỉ cần nạp data → hỏi → xong.

API low-level: Dễ custom từng thành phần (retriever, reranker, post-processor,...), phù hợp nghiên cứu, production.

Tích hợp sẵn nhiều tính năng nâng cao:

Retrieval nâng cao: Hybrid search, Semantic rerank, Query Transform, Multi-modal (text + image), Conversational memory, ...

Index đa dạng: Không chỉ vector mà còn List, Tree, Graph index.

Streaming, “chunk” động, context window,...: Dễ tuning, ít phải “hack” code.

Khả năng tích hợp với các hệ thống khác:

LlamaIndex tích hợp mượt với LangChain, ChatGPT plugin, Flask, Docker, Streamlit, FastAPI,...

Đặc biệt, có thể xuất index ra format cho các vector DB phổ biến.

Documentation, Example, Cộng đồng:

Tài liệu cực dễ hiểu, nhiều example đa dạng thực chiến.

Cộng đồng active, nhiều tutorial, event, workshop.

So với LangChain
LangChain mạnh về workflow orchestration (làm agent, tool-use, chaining nhiều pipeline phức tạp), nhưng code RAG thuần trong LangChain thường phải viết nhiều hơn, cấu hình phức tạp.

LlamaIndex tối ưu hóa pipeline RAG, tập trung sâu cho bài toán kết nối dữ liệu riêng với AI.

So với Haystack
Haystack thiên về enterprise (Python/Java), tài liệu tốt nhưng thiên về mô hình chuẩn/truyền thống. Cộng đồng Việt ít hơn, plugin ít hơn LlamaIndex.

So với Vector DB thuần
Vector DB chỉ là phần “kho” lưu dữ liệu đã embed, bạn vẫn phải tự xây các tầng còn lại (data ingestion, query, rerank, context,...). LlamaIndex lo luôn những thứ này.

3. Khi nào nên chọn LlamaIndex?
Muốn xây ứng dụng hỏi đáp trên dữ liệu riêng nhanh, code ít, dễ mở rộng.

Muốn tối ưu từng bước pipeline RAG (custom retriever, chunking, index, rerank,...).

Muốn tích hợp AI vào ứng dụng của bạn mà không bị “cứng nhắc” như các dịch vụ all-in-one (VD: Zapier, Google Vertex AI Search,...).

Thích cộng đồng mở, dễ góp ý, đóng góp plugin mới.

4. Tóm tắt bảng so sánh
Tiêu chí	LlamaIndex	LangChain	Haystack	VectorDB
Chuyên sâu RAG	✅	❌ (đa năng)	✅	❌
Dễ dùng cho người mới	✅	❌	✅	❌
API high-level	✅	❌	✅	❌
Khả năng mở rộng	✅	✅	⚠️	⚠️
Plugin Data Loader	✅ (300+)	~100	<50	❌
Doc, cộng đồng	✅	✅	⚠️	⚠️

5. Kết luận: LlamaIndex phù hợp với ai?
Rất hợp cho cả dân kỹ thuật, PM, startup lẫn doanh nghiệp muốn POC nhanh ứng dụng RAG với dữ liệu nội bộ, sau này vẫn có thể scale/tuỳ biến sâu.

Nếu bạn chỉ làm RAG cho một project nhỏ, muốn code ngắn, cấu hình dễ, thì LlamaIndex là lựa chọn rất mạnh.

Nếu cần orchestration nhiều workflow (vd: Agent, Tool-Use, Multi-Chain...) thì nên cân nhắc LangChain hoặc kết hợp cả hai.
