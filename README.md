# llmops-agent-lab

Proyecto base del laboratorio de LLMOps: un agente de retención con LangChain, desplegado con CRISP-ML(Q).

La estructura ya está creada y los archivos están vacíos. La guía indica qué va en cada uno:
[2. llmops-agente-langchain-crisp-mlq.md](https://github.com/utec-devops-2026/laboratorios/blob/main/laboratorio_llmops/2.%20llmops-agente-langchain-crisp-mlq.md)

## Cómo empezar

No trabajes sobre este repositorio: haz **fork** a tu cuenta (botón **Fork**) y clona tu fork.

```bash
git clone https://github.com/<tu-usuario>/llmops-agent-lab.git
cd llmops-agent-lab
```

## Qué archivo se llena en qué fase

| Fase | Archivo | Estado |
|---|---|---|
| Paso 0 | `requirements.txt`, `.gitignore`, `src/__init__.py` | Listos |
| 1. Negocio y datos | `gate/thresholds.json`, `gate/baseline.json`, `data/clientes.csv`, `data/golden.jsonl` | Vacíos |
| 2. Preparación | `src/tools.py` | Vacío |
| 3. Modelado | `config.json`, `src/agent.py`, `prompts/agente/v1.md` | Vacíos |
| 4. Evaluación | `src/evaluate.py`, `src/gate.py`, `prompts/agente/v2.md`, `tests/test_agent.py` | Vacíos |
| 5.1 API | `src/api.py` | Vacío |
| 5.2 Imagen | `Dockerfile`, `.dockerignore` | Vacíos |
| 5.3 Pipeline | `.github/workflows/agent.yml` | Lo creas tú |
| 5.3 Pipeline | `.github/CODEOWNERS` | Vacío |
| 6. Monitoreo | `data/prod/semana_base.jsonl`, `data/prod/semana_price_hike.jsonl`, `src/replay.py`, `src/monitor.py` | Vacíos |

El workflow no viene creado a propósito: un archivo de workflow vacío hace que GitHub Actions marque un error en cada push.
