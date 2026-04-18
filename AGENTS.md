# AGENTS - Configurações IA

## Objetivo
Este repositório é um projeto Python leve com um único módulo de execução (`main.py`) e uma configuração mínima no `pyproject.toml`.

## Comandos de validação e execução
- Use `ruff check .` para validar todo o código Python do projeto.
- Execute o projeto localmente com `python main.py` ou `python -m main`.

## Convenções principais
- Python
  - Sempre use `ruff` como ferramenta de validação e linting.
  - Não substitua `ruff` por `pylint`, `flake8` ou outras ferramentas para validação de Python.
  - Gere docstrings para funções, classes e módulos quando o código não for trivial.
- Arquivos SSH
  - Use `ssh-lint` para validar arquivos de configuração SSH.
- Arquivos YAML
  - Use `yamllint` para validar arquivos YAML.

## Ponto de verdade do projeto
- `pyproject.toml` é a fonte de verdade para metadados e dependências.
- A versão mínima de Python suportada é `>=3.13`.

## Observações úteis para agentes
- Este repositório não tem dependências externas listadas atualmente.
- Mantenha o escopo das alterações pequeno e adequado a um projeto de configuração e utilitários.
- Considere atualizar o `README.md` se adicionar nova documentação ou instruções de uso.

## Referências internas
- Há um arquivo complementar de regras em `.instructions.md` que define os requisitos de lint e validação do projeto.


# Instrução de projeto: validação Python com Ruff

## Regras arquivos *.py
- Use sempre `ruff` como a ferramenta de validação de código Python.
- Ao gerar, revisar ou corrigir código Python, escolha `ruff` para linting e análise de qualidade.
- Não substitua Ruff por `pylint`, `flake8` ou outras ferramentas de linting para validação de Python.
- Valide usando `ruff check .` no diretório do projeto.
- Use sempre comentários para explicar o propósito de blocos de código complexos ou não triviais.
- Evite usar comentários para explicar código simples ou autoexplicativo, a menos que seja necessário para esclarecer a intenção do código.
- Crie sempre docstrings para funções, classes e módulos para descrever seu propósito, parâmetros e valores de retorno.

## Regras arquivos *.ssh
- Use `ssh-lint` para validar arquivos de configuração SSH.
- Ao revisar ou corrigir arquivos de configuração SSH, escolha `ssh-lint` para garantir a conformidade com as melhores práticas de segurança.
- Não substitua `ssh-lint` por outras ferramentas de validação para arquivos SSH.
- Valide usando `ssh-lint <caminho-do-arquivo>` para verificar a configuração.

## Regras arquivos *.YAML
- Use `yamllint` para validar arquivos YAML.
- Ao revisar ou corrigir arquivos YAML, escolha `yamllint` para garantir a conformidade com as melhores práticas de formatação e estruturação.
- Não substitua `yamllint` por outras ferramentas de validação para arquivos YAML.
- Valide usando `yamllint <caminho-do-arquivo>` para verificar a sintaxe e a formatação do arquivo YAML