# Getting Started

Guia rápido para preparar o ambiente local de desenvolvimento do `rosa-channel-service`.

## Pré-requisitos

- Python 3.11+
- [uv](https://docs.astral.sh/uv/)

## Instalação de dependências

```bash
uv sync --all-groups
```

## Ativar hooks de pre-commit

```bash
uv run pre-commit install
```

> O projeto bloqueia commit direto na branch `main` com o hook `no-commit-to-branch`.

## Rodar a aplicação

```bash
uv run uvicorn rosa_channel_service.main:app --reload
```

## Qualidade de código e testes

```bash
uv run ruff check .
uv run ruff format --check .
uv run pytest
```

## Documentação local (MkDocs)

```bash
uv run mkdocs serve
```

A documentação ficará disponível em `http://127.0.0.1:8000`.
