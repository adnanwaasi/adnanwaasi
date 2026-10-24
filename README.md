<h1 align="center">Adnan Waasi</h1>

<p align="center">
  <b>Backend + applied AI.</b> I build systems that check their own output.<br/>
  <i>If it doesn't run, it doesn't ship.</i>
</p>

<p align="center">
  <a href="https://adnanwaasi.vercel.app"><img src="https://img.shields.io/badge/portfolio-adnanwaasi.vercel.app-000?style=flat-square&logo=vercel&logoColor=white" alt="Portfolio"/></a>
  <a href="https://github.com/adnanwaasi"><img src="https://img.shields.io/github/followers/adnanwaasi?label=followers&style=flat-square&logo=github" alt="GitHub followers"/></a>
  <img src="https://img.shields.io/badge/SRMIST-B.Tech%20CSE-1f6feb?style=flat-square" alt="SRMIST B.Tech CSE"/>
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

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" alt="LangChain"/>
  <img src="https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white" alt="Ollama"/>
  <img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white" alt="pytest"/>
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++"/>
  <img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go"/>
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux"/>
</p>

---

### 📊 Activity

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=adnanwaasi&show_icons=true&hide_border=true&count_private=true&theme=transparent" alt="GitHub stats"/>
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=adnanwaasi&layout=compact&hide_border=true&theme=transparent" alt="Top languages"/>
</p>

---

<p align="center"><i>Shipped only after it runs.</i></p>
