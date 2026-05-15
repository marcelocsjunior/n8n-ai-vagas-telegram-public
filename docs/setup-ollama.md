# Setup Ollama

## Objetivo

Usar IA local gratuita no workflow n8n.

## Modelo inicial

```text
llama3.2:3b
```

## Endpoint esperado

```text
http://localhost:11434
```

Em ambiente de rede local, ajustar o host conforme o IP da VM.

## Validação

```bash
curl http://localhost:11434/api/tags
```

A resposta deve listar o modelo instalado.

## n8n

No node Ollama Chat Model:

```text
Base URL: endpoint do Ollama
Model: llama3.2:3b
```

Conectar o node ao AI Agent pelo conector Chat Model.

## Evolução futura

Avaliar uso do `qwen2.5:7b` se a VM tiver memória e CPU suficientes.
