# rosa-channel-service

Serviço centralizado de comunicação para o ecossistema PROJETO ITABERAI (e-mail, WhatsApp e notificações).

## Setup inicial de desenvolvimento

O passo a passo completo está em [`docs/get_start.md`](docs/get_start.md).

### 1) Pré-requisitos
- Python 3.11+
- [uv](https://docs.astral.sh/uv/)

### 2) Instalação de dependências
```bash
uv sync --all-groups
```

### 3) Ativar pre-commit
```bash
uv run pre-commit install
```

> O projeto bloqueia commit direto na branch `main` via hook `no-commit-to-branch`.

### 4) Executar aplicação localmente
```bash
uv run uvicorn rosa_channel_service.main:app --reload
```

### 5) Qualidade e testes
```bash
uv run ruff check .
uv run ruff format --check .
uv run pytest
```

### 6) Documentação com MkDocs
```bash
uv run mkdocs serve
```

## Endpoints base
- `GET /health` — healthcheck da aplicação.
