# 🎙️ AudioScribe Pro v1.0.0

[![Versão](https://img.shields.io/badge/vers%C3%A3o-1.0.0-blue.svg)](https://github.com/)
[![Licença](https://img.shields.io/badge/Licen%C3%A7a-CC%20BY--NC--SA%204.0-green.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](https://www.python.org/)
[![Whisper AI](https://img.shields.io/badge/Whisper%20IA-Faster--Whisper%20%7C%20OpenAI-purple)](https://github.com/openai/whisper)

**AudioScribe Pro** é um aplicativo desktop avançado para **Transcrição Automática e Legenderia Inteligente de Áudios e Vídeos**, desenvolvido em **Python** com **CustomTkinter** e alimentado pelos motores de Inteligência Artificial **Whisper IA** (OpenAI & Faster-Whisper/CTranslate2).

---

## 🌟 Principais Funcionalidades

- **🚀 Transcrição de Altíssima Performance**: Suporte nativo aos motores `Faster-Whisper` (aceleração CTranslate2 em GPU/CPU) e `OpenAI-Whisper`.
- **📂 Transcrição e Processamento em Lote**: Adicione arquivos individuais ou pastas inteiras de áudio e vídeo com visualização em tempo real do progresso.
- **🎵 Player de Mídia Embutido com Sincronização Bi-direcional**:
  - Clique em qualquer linha de legenda no Editor com carimbo de tempo (`[00:15 - 00:22]`) para ir direto ao momento exato da mídia.
  - O Player destaca em tempo real a fala sendo reproduzida.
  - Reprodução universal compatível com todos os formatos de mídia (`.mp3`, `.wav`, `.mp4`, `.mkv`, `.avi`, `.mov`, `.m4a`, etc.).
- **🌐 Tradutor Automático de Legendas e Transcrições**:
  - Traduza transcrições e legendas entre **6 idiomas oficiais** (*Português*, *English*, *Español*, *Français*, *Deutsch*, *Italiano*).
  - Preserva a versão original intacta e permite alternar facilmente entre a transcrição original e as versões traduzidas.
- **📄 Alternador de Horários (Texto Limpo vs Timestamps)**:
  - Botão alternador instantâneo **"⏱️ Exibir Horários" / "📄 Ocultar Horários (Texto Limpo)"** para remover todos os marcadores de tempo e gerar textos corridos e limpos para leitura e cópia.
- **📤 Exportação Multiformato Automática**:
  - Exporte automaticamente para **TXT**, **Word (.docx)**, **PDF**, **Legenda SRT (.srt)**, **Legenda WebVTT (.vtt)** e **Dados JSON (.json)**.
- **📁 Acesso Rápido aos Arquivos Exportados**:
  - Botão **"📁 Abrir Pasta dos Arquivos"** integrado para abrir a pasta de saída direto no gerenciador de arquivos do sistema operacional.
- **🎨 Interface Moderna com Suporte a 6 Idiomas**:
  - Alternância rápida entre **Modo Claro (Light Mode)** e **Modo Escuro (Dark Mode)** nas Configurações.
  - Suporte completo a **6 idiomas de interface** (*Português, Inglês, Espanhol, Francês, Alemão e Italiano*).

---

## 🛠️ Requisitos de Instalação

### 1. Pré-requisitos do Sistema

- **Python**: Versão 3.10 ou superior
- **FFmpeg**: Necessário para extração e pré-visualização de áudios/vídeos.
  - **Linux (Ubuntu/Debian)**: `sudo apt install ffmpeg`
  - **macOS**: `brew install ffmpeg`
  - **Windows**: Baixe via winget ou insira o `ffmpeg.exe` no PATH.

### 2. Instalação das Dependências Python

Clone o repositório e instale os pacotes listados no `requirements.txt`:

```bash
git clone https://github.com/usuario/audioscribe-pro.git
cd audioscribe-pro

# Criação do ambiente virtual (opcional, porém recomendado)
python3 -m venv venv
source venv/bin/activate  # No Windows: venv\Scripts\activate

# Instalação das dependências
pip install -r requirements.txt
```

---

## 🚀 Como Executar o Aplicativo

Para iniciar o **AudioScribe Pro v1.0.0**, execute o comando principal:

```bash
python main.py
```

---

## 👨‍💻 Autor & Licença

- **Desenvolvedor**: **Prof. Dr. Alides Baptista Chimin Junior**
- **Licença de Uso**: **Creative Commons Atribuição-NãoComercial-CompartilhaIgual 4.0 Internacional (CC BY-NC-SA 4.0)**

> **Sobre a Licença CC BY-NC-SA 4.0**:
> Esta licença permite que outros remixem, adaptem e criem a partir deste trabalho para fins **não comerciais**, desde que atribuam o devido crédito ao autor original e licenciem suas novas criações sob termos idênticos.

---

## 📚 Agradecimentos & Tecnologias Utilizadas

1. **[OpenAI Whisper](https://github.com/openai/whisper)**: Modelo de Reconhecimento Automático de Fala (ASR).
2. **[Faster-Whisper / CTranslate2](https://github.com/SYSTRAN/faster-whisper)**: Motor otimizado de inferência para modelos Whisper.
3. **[CustomTkinter](https://github.com/TomSchimansky/CustomTkinter)**: Extensão de interface gráfica contemporânea para Tkinter.
4. **Comunidade Python**: Pelas bibliotecas `python-docx`, `reportlab`, `deep-translator`, `pygame` e `av`.
