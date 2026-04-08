# 🎙️ Assistente de Voz com GenAI (Whisper + ChatGPT + gTTS)

## 📌 Descrição do Projeto

Este projeto apresenta a implementação de um **assistente de voz utilizando Inteligência Artificial Generativa**, desenvolvido no **Google Colab**, capaz de realizar uma interação completa por voz.

O sistema permite que o usuário **grave uma pergunta em áudio**, que é convertida em texto por um modelo de reconhecimento de fala, processada por um modelo de linguagem generativa e, por fim, convertida novamente em áudio como resposta.

Idioma utilizado no projeto: **Português (`pt`)**

---

## ▶️ Acesse o Notebook no Google Colab

🔗 **Link direto para execução do projeto:**  
https://colab.research.google.com/drive/1Q2jYRopcjjhSV9jxl0bUMqtIrcLk7vlm?usp=sharing

> Recomenda-se abrir o link logado em uma conta Google e executar as células na ordem indicada.

---

## 🧠 Funcionalidades

- Gravação de áudio diretamente pelo navegador
- Reconhecimento de fala usando **Whisper (OpenAI)**
- Geração de respostas com **ChatGPT**
- Síntese de voz da resposta com **gTTS**
- Execução completa no Google Colab

---

## 🧩 Arquitetura do Fluxo

1. 🎤 Gravação do áudio via JavaScript + Python  
2. 🧠 Transcrição do áudio em texto com Whisper  
3. 💬 Envio da transcrição para o ChatGPT  
4. 🔊 Conversão da resposta textual em áudio com gTTS  

---

## ⚙️ Requisitos

- Conta Google para utilizar o Google Colab
- Conta OpenAI com **API Key válida**
- Navegador com permissão para uso do microfone
- Conexão com a internet

---

## 🚀 Passo a Passo para Execução

### 1️⃣ Abrir o Projeto no Google Colab

- Acesse o link do notebook disponibilizado acima
- Execute as células **na ordem apresentada**

---

### 2️⃣ Gravação de Áudio 🎤

- Execute a célula responsável pela gravação
- Autorize o acesso ao microfone quando solicitado
- Fale sua pergunta dentro do tempo configurado (padrão: 10 segundos)
- O áudio será salvo como `request_audio.wav`

---

### 3️⃣ Reconhecimento de Fala com Whisper 🧠

- O modelo Whisper transcreve o áudio gravado
- O texto transcrito será exibido no output

**Exemplo de pergunta:**

> Como a inteligência artificial generativa pode ajudar bancos a melhorar o atendimento ao cliente?

---

### 4️⃣ Configuração da API OpenAI 🔑

Antes de executar a integração com o ChatGPT:

1. Acesse: https://platform.openai.com/account/api-keys  
2. Gere sua **API Key**
3. No código, substitua:

```python
os.environ['OPENAI_API_KEY'] = 'coloque sua API Key'
