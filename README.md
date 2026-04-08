# 🎙️ Assistente de Voz com GenAI (Whisper + ChatGPT + gTTS)

## 📌 Descrição do Projeto

Este projeto apresenta a implementação de um **assistente de voz utilizando Inteligência Artificial Generativa**, desenvolvido no **Google Colab**, capaz de realizar uma interação completa por voz.

O sistema permite que o usuário **grave uma pergunta em áudio**, que é convertida em texto por um modelo de reconhecimento de fala, processada por um modelo de linguagem generativa e, por fim, convertida novamente em áudio como resposta.

Idioma utilizado no projeto: **Português (`pt`)**

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

