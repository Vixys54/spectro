[README.md](https://github.com/user-attachments/files/33868106/README.md)
<p align="center">
  <img src="https://raw.githubusercontent.com/Vixys54/Spectro/main/readme-github/assets/logo.png" alt="Spectro Logo" width="120"/>
</p>

<h1 align="center">🌀 Spectro</h1>

<p align="center">
  <b>Aplicativo mobile para uso de Agentes de IA "Agent/Coding" sem necessidade de um PC/Desktop.</b>
</p>

<p align="center">
  <img alt="GitHub license" src="https://img.shields.io/github/license/Vixys54/Spectro?color=00f0ff&style=for-the-badge"/>
  <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Vixys54/Spectro?color=00f0ff&style=for-the-badge"/>
  <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/Vixys54/Spectro?color=00f0ff&style=for-the-badge"/>
</p>

---

## 📱 Sobre o Spectro

O **Spectro** é um laboratório móvel de Inteligência Artificial que roda diretamente no seu Android. Ele permite que você crie, edite, gerencie e automatize arquivos, pastas e scripts no seu celular sem precisar de um computador — tudo através de uma interface de chat com IA.

Seja para criar projetos de código, organizar experimentos de IA, compactar arquivos ou executar terminais móveis, o Spectro coloca o controle real do sistema de arquivos do Android nas suas mãos.

## ✨ Funcionalidades

| Área | O que você pode fazer |
|------|----------------------|
| 💬 **Chat IA** | Converse com modelos de IA (Gemini, Claude, OpenAI, Grok, Qwen, Ollama e mais) |
| 📁 **Arquivos** | Crie, leia, edite, exclua e liste arquivos e pastas reais do Android |
| 🖥️ **Termux** | Terminal móvel compatível com comandos estilo Unix |
| 📦 **Pacotes** | Marketplace de runtimes e ferramentas (Python, Node.js, MCP, SQLite, Git, etc.) |
| 🗜️ **Compactação** | Crie e extraia arquivos ZIP, RAR e 7Z diretamente no dispositivo |
| 🧠 **Contexto** | Memória compactada estilo Traycer para sessões longas |

## 🚀 Começando

### Pré-requisitos
- Dispositivo Android (recomendado Android 11+)
- Permissão de "Acesso a todos os arquivos" (All Files Access) — necessária em dispositivos Xiaomi/MIUI

### Instalação
1. Faça o download do APK mais recente na seção [**Releases**](https://github.com/Vixys54/Spectro/releases)
2. Instale o APK no seu Android (ativa "Fontes desconhecidas" se necessário)
3. Conceda as permissões de armazenamento quando solicitado
4. Configure sua chave de API na aba **Ajustes**

## 🧠 Como funciona a IA

O Spectro usa um agente autônomo em processo contínuo (estilo Traycer). Quando você pede uma ação — como criar um arquivo ou compactar uma pasta — a IA:

1. **Raciocina** sobre o que precisa ser feito (`<thinking>`)
2. **Emite uma chamada de ferramenta** (`TOOL_CALL`) com nome e argumentos
3. **Executa** a ação no armazenamento real do Android
4. **Apresenta o resultado** e continua se houver mais passos

### Exemplo de interação
> **Usuário:** "Crie um arquivo texto chamado receita.txt com o conteúdo 'arroz frito' dentro da pasta Spectro"

> **IA:** Detecta a intenção → emite `write_file` → grava o arquivo → confirma sucesso

## 📦 Pacotes e Marketplace

Na aba **Pacotes** você encontra runtimes e ferramentas instaláveis:

- **Python 3.12 (Pyodide WASM)** — Interpretador Python real no Android sem root
- **Node.js JS Engine** — Execução de JavaScript/TypeScript
- **Model Context Protocol (MCP) Core** — Conecte a IA a ferramentas móveis e servidores SSE
- **SQLite 3 Embedded** — Banco de dados relacional local
- **Git Mobile Lite** — Controle de versão para seus experimentos
- **Termux CLI Compatibility Kit** — Comandos Unix utilitários (curl, grep, sed, awk...)
- **Compactador ZIP (Python zipfile)** — Compactação e extração de .zip
- **Suporte RAR (unrar-free)** — Extração de arquivos .rar
- **Compactador 7Z (p7zip)** — Alta compressão em .7z

## 🗜️ Compactação de Arquivos

O Spectro permite compactar e extrair arquivos diretamente no dispositivo:

- **ZIP:** Crie arquivos `.zip` com múltiplos arquivos e pastas
- **RAR:** Extraia conteúdo de arquivos `.rar`
- **7Z:** Compacte com alta taxa de compressão

A IA gera os scripts de compactação usando bibliotecas padrão do Python (`zipfile`) e você executa no terminal móvel integrado.

## 🧩 Compactação de Contexto

Para sessões longas, o Spectro usa **context compaction** (estilo Traycer/Claude Code):
- Mantém as mensagens recentes intactas
- Resume a história antiga em um bloco de memória compactado
- Preserva arquivos tocados, decisões e estado das tarefas
- Libera tokens no contexto do modelo para continuar trabalhando

## 🛠️ Tecnologias

- [React](https://reactjs.org/) + [TypeScript](https://www.typescriptlang.org/)
- [Vite](https://vitejs.dev/) + [Tailwind CSS](https://tailwindcss.com/)
- [Capacitor](https://capacitorjs.com/) (bridge para Android nativo)
- [Lucide React](https://lucide.dev/) (ícones)

/*## 🤝 Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/minha-feature`)
3. Commit suas mudanças (`git commit -m 'feat: adiciona minha feature'`)
4. Push para a branch (`git push origin feature/minha-feature`)
5. Abra um Pull Request*/

## 📄 Licença

Este projeto está sob a licença **MIT**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

<p align="center">
  Desenvolvido com ❤️ por <a href="https://github.com/Vixys54" target="_blank">Vixys54</a>
</p>
