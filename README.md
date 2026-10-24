<h1 align="center">Adnan Waasi</h1>

<p align="center">
  <b>Backend + applied AI.</b> I build systems that check their own output.<br/>
  <i>If it doesn't run, it doesn't ship.</i>
</p>

<p align="center">
  <a href="https://adnanwaasi.vercel.app"><img src="https://img.shields.io/badge/portfolio-adnanwaasi.vercel.app-000?style=flat-square&logo=vercel&logoColor=white" alt="Portfolio"/></a>
  <a href="https://github.com/adnanwaasi"><img src="https://img.shields.io/github/followers/adnanwaasi?label=followers&style=flat-square&logo=github" 
</p>

---

### 🔭 Right now

- 🌐 [adnanwaasi.vercel.app](https://adnanwaasi.vercel.app)

---

### 🧭 What I care about

**Correctness over demos.** **Testable boundaries.** **Architecture you can still explain six months later.**

> Everything here has been run, and I know it works.
> If it doesn't work, it isn't here.

How that plays out in practice:

| Principle | What it means in my code |
| --- | --- |
| Verify, don't trust | Generated output gets executed and tested before anything accepts it |
| Idempotent by default | Content hashing and dedupe, so a retry never double-processes |
| Explicit state | Work moves through a state machine, not through loose flags |
| Safe concurrency | Workers claim jobs through the database, not through hope |
| Roll back | If a change doesn't meet the bar, the last good version stays |

---

### 🛠️ Selected work

| Project | What it does | Stack |
| --- | --- | --- |
| [**code synthesizer and validator**](https://github.com/adnanwaasi/fyproject) | Self-repairing code synthesis: spec extraction → generation → test generation → execution → error analysis → repair. Rolls back anything under an 85% acceptance bar. | Python · FastAPI · LangChain · Pydantic |
| [**f1 lap_time_simulation**](https://github.com/adnanwaasi/lap_time_simulation) | originally i wanted to make my quali simulations and check who has better chances at winning and what could be quali laps then later made it into race simulations | C++ · Python |
| [**faster one**](https://github.com/adnanwaasi/mini_laps) | a game built to improve your observability and reaction time  | C++  |

<details>
<summary><b>fyproject pipeline at a glance</b></summary>

```mermaid
flowchart LR
    A[Spec extraction] --> B[Code generation]
    B --> C[Test generation]
    C --> D[Execution]
    D -->|pass ≥ 85%| E[Accept]
    D -->|fail| F[Error analysis]
    F --> G[Repair]
    G --> D
    G -.->|below bar| H[Rollback]
```

</details>

---

### 🧰 Toolbox

**Languages**

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++"/>
  <img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript"/>
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white" alt="Bash"/>
</p>

**Backend & data**

<p>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI"/>
  <img src="https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white" alt="Pydantic"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/>
  <img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white" alt="pytest"/>
</p>

**AI / LLM**

<p>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" alt="LangChain"/>
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langgraph&logoColor=white" alt="LangGraph"/>
  <img src="https://img.shields.io/badge/Langfuse-0A0A0A?style=flat-square" alt="Langfuse"/>
  <img src="https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white" alt="Qdrant"/>
  <img src="https://img.shields.io/badge/Chroma-FF6446?style=flat-square" alt="Chroma"/>
  <img src="https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white" alt="Ollama"/>
  <img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" alt="Hugging Face"/>
</p>

**ML**

<p>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch"/>
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white" alt="TensorFlow"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="scikit-learn"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" alt="NumPy"/>
  <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="pandas"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white" alt="Jupyter"/>
</p>

**Infra**

<p>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" alt="Kubernetes"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git"/>
</p>

**Frontend**

<p>
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React"/>
</p>

---

### 📊 Activity

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=adnanwaasi&show_icons=true&hide_border=true&count_private=true&theme=transparent" alt="GitHub stats"/>
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=adnanwaasi&layout=compact&hide_border=true&theme=transparent" alt="Top languages"/>
</p>

---

<p align="center"><i>Shipped only after it runs.</i></p>
