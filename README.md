# 🤓 Smart-Agent-WebSearch

Este projeto consiste em um agente inteligente que utiliza a ferramenta de busca DuckDuckGo para realizar pesquisas na web e retornar resultados de forma eficiente. O agente usa um modelo de inferência para gerar respostas baseadas nas informações encontradas online.

## Funcionalidades

- **Integração com DuckDuckGo**: O agente pode realizar pesquisas diretamente no DuckDuckGo.
- **Respostas baseadas em modelos de IA**: Utiliza um modelo de inferência para analisar e retornar as respostas.
- **Facilidade de uso**: Basta passar a consulta que o agente retorna a resposta.

## Tecnologias Utilizadas

- **Python**: Linguagem principal utilizada para desenvolver o agente.
- **SmolAgents**: Biblioteca para criar e configurar o agente inteligente.
- **DuckDuckGo API**: Usado para realizar as pesquisas na web.
- **Modelos de Inferência**: Utiliza modelos de IA para processar as respostas.

## Como Usar

1. Clone o repositório:

   ```bash
   git clone https://github.com/seu-usuario/Smart-Agent-WebSearch.git

2. Instale as dependências:

   ```bash
   pip install smolagents
   ```

3. Execute o código:

   ```python
   from smolagents import CodeAgent, DuckDuckGoSearchTool, InferenceClientModel

   # Inicialize o modelo
   model = InferenceClientModel()

   # Inicialize a ferramenta de busca
   search_tool = DuckDuckGoSearchTool()

   # Crie o agente com a ferramenta de busca
   agent = CodeAgent(tools=[search_tool], model=model)

   # Execute uma consulta
   response = agent.run("Qual a altura do Cristo Redentor?")
   print(response)
   ```

