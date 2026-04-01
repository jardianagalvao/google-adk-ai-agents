# 🤖 Google ADK - AI Agents Study Case

Este repositório contém uma série de implementações práticas utilizando o **Google Agent Development Kit (ADK)**. O objetivo é explorar diferentes arquiteturas de agentes de IA, desde execuções simples até orquestrações complexas de múltiplos agentes.

## 🚀 Funcionalidades Implementadas

* **Single Agent:** Implementação básica de um assistente de IA.
* **Sequential Workflow:** Cadeia de agentes onde o output de um (ex: Foodie Agent) serve de input para o próximo (ex: Transportation Agent).
* **Routing Agent:** Um "diretor" que analisa a intenção do usuário e despacha a tarefa para o especialista correto.
* **Adaptive Memory:** Agentes que lembram preferências do usuário para planejar roteiros de vários dias.
* **Contexto Local:** Exemplos adaptados para a realidade de **Fortaleza, CE**, incluindo pontos turísticos e gastronomia regional.



## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3.10+
* **Modelo de IA:** Gemini 2.5 Flash (via Google GenAI API)
* **Framework:** Google ADK (Agent Development Kit)
* **Banco de Dados:** SQLite (para persistência de sessões)

## 📋 Pré-requisitos

1.  Obtenha uma API Key no [Google AI Studio](https://aistudio.google.com/).
2.  Python instalado (v3.10 ou superior).

## 🔧 Configuração e Instalação

1.  Clone o repositório:
    ```bash
    git clone [https://github.com/SEU_USUARIO/google-adk-ai-agents.git](https://github.com/SEU_USUARIO/google-adk-ai-agents.git)
    cd google-adk-ai-agents
    ```

2.  Crie e ative o ambiente virtual:
    ```bash
    python -m venv venv
    source venv/bin/activate  # No Windows: venv\Scripts\activate
    ```

3.  Instale as dependências:
    ```bash
    pip install -r requirements.txt
    ```

4.  **Configuração de Variáveis de Ambiente:**
    Crie um arquivo `.env` dentro da pasta do agente que deseja rodar (ex: `agent/.env`) com o seguinte conteúdo:
    ```env
    GOOGLE_GENAI_USE_VERTEXAI=FALSE
    GOOGLE_API_KEY=SUA_CHAVE_AQUI
    ```

## 💻 Como Executar

### Via CLI (Linha de Comando)
```bash
python main.py
