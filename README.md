# Hi, I'm Planckbaka 👋

Backend Engineer specializing in **Go/Python Cloud Services** and **AI Infrastructure**. Currently focus on high-performance model serving, distributed systems, and intelligent multi-agent architectures.

<p align="left">
  <img src="https://komarev.com/ghpvc/?username=planckbaka&label=Profile%20Views&color=24292e&style=flat-square" alt="Profile Views" />
</p>

---

## 🛠 Technical Competency Matrix

| Category | Technologies, Frameworks & Concepts |
| :--- | :--- |
| **Go Backend & Cloud Native** | Go • Gin • gRPC • Protobuf • Kafka • Redis • PostgreSQL • Docker • Kubernetes • AWS • Clean Architecture • DDD |
| **AI Infra & Model Serving** | PyTorch • vLLM • Ollama • Triton Inference Server • GPU Scheduling & Optimization • CUDA & Core Acceleration |
| **AI Agent & LLM Engineering** | LangChain / LangGraph • LlamaIndex • Vector Databases (Qdrant / Milvus / Chroma) • RAG • Multi-Agent Orchestration • Fine-Tuning |
| **Modern Fullstack (Secondary)** | React • Next.js • TypeScript • Tailwind CSS • Redux / Zustand |

---

## 🌟 Flagship Architectures & Core Showcases

### 1. High-Concurrency Go Microservice System Architecture
A robust, highly decoupled enterprise backend system engineered with Go, leveraging **Clean Architecture** and **Domain-Driven Design (DDD)** principles to ensure maintainability and high scalability.

```mermaid
graph TD
    Client[Client / Web / App] -->|HTTPS / WSS| GW[API Gateway]
    GW -->|gRPC / Service Discovery| AuthSvc[Auth Service]
    GW -->|gRPC| BizSvc[Core Business Service]
    BizSvc -->|Read / Write| DB[(PostgreSQL Cluster)]
    BizSvc -->|Cache / Session| Redis[(Redis Cluster)]
    BizSvc -->|Asynchronous Events| Kafka{Kafka Event Bus}
    Kafka -->|Consume Events| AsyncWorker[Background Worker]
    AsyncWorker -->|Persist / Aggregate| DB

    %% Style styling
    classDef default fill:#2d333b,stroke:#444c56,stroke-width:1px,color:#adbac7;
    classDef highlight fill:#1f6feb,stroke:#58a6ff,stroke-width:1px,color:#ffffff;
    classDef storage fill:#223322,stroke:#2ea043,stroke-width:1px,color:#56d364;
    class GW highlight;
    class BizSvc highlight;
    class DB storage;
    class Redis storage;
    class Kafka storage;
```

### 2. Autonomous Multi-Agent & RAG Platform Flow
An intelligent LLM orchestration framework coordinating multiple specialized agents. It integrates advanced semantic search over vector stores and dynamically maps tasks to specialized workflows.

```mermaid
graph TD
    UserQuery[User Request] -->|Query| AgentOrch[Multi-Agent Orchestrator]
    AgentOrch -->|Semantic Search| RetSvc[Retrieval Engine / RAG]
    RetSvc -->|Embeddings| VectorDB[(Vector DB: Qdrant / Milvus)]
    RetSvc -->|Relevant Context| AgentOrch
    AgentOrch -->|Delegate Task| WriterAgent[Agent: Specialized Writer]
    AgentOrch -->|Delegate Task| CodeAgent[Agent: Code Interpreter]
    WriterAgent & CodeAgent -->|Call LLM / Tool Use| LLM[Model Inference: vLLM / Triton]
    AgentOrch -->|Synthesized Output| UserQuery

    %% Style styling
    classDef default fill:#2d333b,stroke:#444c56,stroke-width:1px,color:#adbac7;
    classDef highlight fill:#d29922,stroke:#f0883e,stroke-width:1px,color:#ffffff;
    classDef model fill:#1f6feb,stroke:#58a6ff,stroke-width:1px,color:#ffffff;
    class AgentOrch highlight;
    class WriterAgent highlight;
    class CodeAgent highlight;
    class LLM model;
```

---

## 🔭 Active Research & Roadmap

* **Inference Optimization:** Benchmarking and optimizing LLM serving latency with `vLLM` and `Triton Inference Server` across heterogeneous GPU clusters.
* **Intelligent Agents:** Investigating multi-agent consensus protocols and durable state management in complex, long-running agent workflows (LangGraph).
* **System Rigor:** Implementing Domain-Driven Design (DDD) patterns in high-throughput Go microservices using clean architectural boundaries.

---

## 📈 Activity & Stats

<p align="left">
  <img src="https://github-readme-stats.vercel.app/api?username=planckbaka&show_icons=true&theme=transparent&hide_border=true&title_color=2f81f7&icon_color=2f81f7&text_color=7d8590" alt="Planckbaka's GitHub stats" width="48%" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=planckbaka&layout=compact&theme=transparent&hide_border=true&title_color=2f81f7&text_color=7d8590" alt="Planckbaka's Top Languages" width="48%" />
</p>

---

## 📫 Connect with Me

* **Email:** [akiwayne24@gmail.com](mailto:akiwayne24@gmail.com)
* **Blog:** [Planck's Space](https://blog-pearl-iota-29.vercel.app/)
* **Location:** Shanghai, China 🇨🇳
