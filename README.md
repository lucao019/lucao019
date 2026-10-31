<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:080b16,45:111827,100:4f46e5&height=210&section=header&text=lucao019&fontSize=56&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=SOFTWARE%20%7C%20IA%20LOCAL%20%7C%20HARDWARE%20%7C%20AUTOMA%C3%87%C3%83O&descAlignY=62&descSize=15&descColor=67e8f9" alt="Banner animado de lucao019"/>

### Construindo soluções práticas — do software à bancada.

Desenvolvedor independente interessado em transformar problemas reais em ferramentas úteis, testáveis e em constante evolução.

<a href="https://github.com/lucao019">
  <img src="https://img.shields.io/badge/GitHub-lucao019-111827?style=for-the-badge&logo=github&logoColor=white" alt="GitHub lucao019"/>
</a>
<img src="https://img.shields.io/badge/FOCO-ENGENHARIA%20PR%C3%81TICA-06b6d4?style=for-the-badge&labelColor=111827" alt="Foco em engenharia prática"/>
<img src="https://img.shields.io/badge/PROJETOS-EM%20EVOLU%C3%87%C3%83O-8b5cf6?style=for-the-badge&labelColor=111827" alt="Projetos em evolução"/>

</div>

---

## Sobre

Crio aplicações desktop, automações e ferramentas que conectam software ao uso cotidiano. Meu foco passa por **Windows, streaming, hardware e IA local**, com atenção à validação no ambiente real e à clareza sobre o que cada recurso faz.

```text
IDEIA  →  PROTÓTIPO  →  TESTES  →  MELHORIA CONTÍNUA
```

## Projeto em destaque

<div align="center">

<a href="https://github.com/lucao019/webcam-mic">
  <img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=0:080b16,100:111827&height=130&section=header&text=LUCAO%20LINK%20%E2%80%94%20webcam-mic&fontSize=38&fontColor=ffffff&fontAlignY=42&desc=ANDROID%20COMO%20WEBCAM%20DO%20PC%20%E2%80%A2%20USB%20%2B%20WI-FI%20%E2%80%A2%20LOW-LATENCY&descSize=14&descColor=67e8f9&descAlignY=68" alt="LUCAO LINK — Android como webcam do PC via USB e Wi-Fi"/>
</a>

### [LUCAO LINK (webcam-mic)](https://github.com/lucao019/webcam-mic)

Transforma a câmera e o microfone do celular Android em fonte de vídeo e áudio do PC, por USB (túnel `adb reverse`) ou Wi-Fi. O vídeo H.264 é remuxado para fMP4 e reproduzido por um player desktop customizado com Media Source Extensions, mantendo a latência próxima do tempo real.

<a href="https://github.com/lucao019/webcam-mic"><img src="https://img.shields.io/badge/Electron-45-47848F?style=flat-square&logo=electron&logoColor=white" alt="Electron 45"/></a>
<a href="https://github.com/lucao019/webcam-mic"><img src="https://img.shields.io/badge/Node.js-20%2B-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js 20 ou superior"/></a>
<a href="https://github.com/lucao019/webcam-mic"><img src="https://img.shields.io/badge/Android-CameraX-3DDC84?style=flat-square&logo=android&logoColor=white" alt="Android CameraX"/></a>
<a href="https://github.com/lucao019/webcam-mic"><img src="https://img.shields.io/badge/Release-v1.2.0-16a34a?style=flat-square" alt="Release v1.2.0"/></a>

<br/>

<a href="https://github.com/lucao019/webcam-mic">Explorar o projeto →</a>

</div>

**Destaques de engenharia:** player de baixa latência com MSE, descoberta automática do PC na LAN, controle remoto de zoom/lente/flash, suporte multi-dispositivo e watchdogs de autorrecuperação. Versão 1.2.0, com changelog técnico de 31 checkpoints documentando evolução real (latência, keyframes, fila TCP, seleção de lente).

## Unknowns Lab — em desenvolvimento (repositório privado)

Um centro de controle desktop para reunir overlays, visualização de inputs e diagnóstico local de desempenho em uma experiência integrada.

### O que estou construindo

| Módulo | Destaques |
| --- | --- |
| **Control Center** | Aplicativo desktop modular, navegação integrada e preferências locais. |
| **Streaming & overlays** | Overlay para OBS, visualizadores de teclado e mouse e crosshair configurável. |
| **Movement Lab** | Visualização de curvas e perfis locais, com ativação explícita dos controles. |
| **PUBG Performance Lab** | Diagnóstico do sistema, sensores disponíveis e comparação local de perfis NVIDIA em modo somente leitura. |

> **Estado do projeto:** desenvolvimento ativo, com releases versionadas e instaladores próprios; o código segue em repositório privado. Dados sem fonte validada são apresentados como indisponíveis; diagnósticos de desempenho não prometem ganhos nem alteram configurações do sistema.

## Outros projetos

| Projeto | Descrição | Tecnologias |
| --- | --- | --- |
| [EasyRomsToOPL](https://github.com/lucao019/easyromstooplps2) | Instala jogos de PS2 em pendrive OPL arrastando o arquivo (.iso/.zip/.rar/.7z), sem corromper o `ul.cfg`; GUI WPF nativa e CLI sobre o mesmo motor. 323 testes passando, licença MIT. | PowerShell · WPF |
| [Nexa Transcrição](https://github.com/lucao019/typewriter) | Aplicativo desktop para transcrever áudio e vídeo 100% localmente (whisper.cpp + FFmpeg), focado em PT-BR; distribuído como instalador Windows. | Electron · React · TypeScript · whisper.cpp |
| [CheckIn — Discord Bot](https://github.com/lucao019/discordbotbylucao99999999999) | Check-in de membros com cards de perfil gerados em sharp (banners GIF), OCR de imagens em PT/EN e transcrição de áudio com whisper.cpp local; CI no GitHub Actions e Dockerfile. | TypeScript · Node.js · discord.js |
| [NVIDIA NIM + VS Code](https://github.com/lucao019/NVIDIA-NIM-VS-Code) | Guia e scripts para usar modelos NVIDIA NIM como provider no VS Code no Windows, com a chave de API protegida no Gerenciador de Credenciais. | Node.js · PowerShell |
| [ComfyUI Stack — até 8 GB de VRAM](https://github.com/lucao019/ComfyUI-Stack-8GB-Vram-ou-menos) | Guia e scripts para configurar geração de vídeo com MiniMax H3 em hardware limitado; workflow testado em uma RTX 2060 de 6 GB. | Python · ComfyUI |
| [Assistente de Bancada](https://github.com/lucao019/assistente-bancada) | Assistente de IA local para reparo eletrônico, com análise de imagens, consulta a esquemáticos em PDF e histórico de atendimentos. | Electron · Node.js · SQLite · llama.cpp |

<div align="center">

<a href="https://github.com/lucao019?tab=repositories">Ver todos os repositórios →</a>

</div>

---

## Ferramentas e tecnologias

<div align="center">

**Linguagens**

<a href="https://developer.mozilla.org/docs/Web/JavaScript" title="JavaScript"><img src="https://skillicons.dev/icons?i=js" alt="JavaScript"/></a>
<a href="https://www.typescriptlang.org/docs/" title="TypeScript"><img src="https://skillicons.dev/icons?i=ts" alt="TypeScript"/></a>
<a href="https://docs.python.org/3/" title="Python"><img src="https://skillicons.dev/icons?i=python" alt="Python"/></a>
<a href="https://learn.microsoft.com/dotnet/csharp/" title="C#"><img src="https://skillicons.dev/icons?i=cs" alt="C sharp"/></a>
<a href="https://docs.oracle.com/en/java/" title="Java"><img src="https://skillicons.dev/icons?i=java" alt="Java"/></a>
<a href="https://learn.microsoft.com/powershell/" title="PowerShell"><img src="https://skillicons.dev/icons?i=powershell" alt="PowerShell"/></a>

**Frontend e apps desktop**

<a href="https://www.electronjs.org/docs/latest" title="Electron"><img src="https://skillicons.dev/icons?i=electron" alt="Electron"/></a>
<a href="https://react.dev/" title="React"><img src="https://skillicons.dev/icons?i=react" alt="React"/></a>
<a href="https://vite.dev/" title="Vite"><img src="https://skillicons.dev/icons?i=vite" alt="Vite"/></a>
<a href="https://learn.microsoft.com/dotnet/" title=".NET / WPF"><img src="https://skillicons.dev/icons?i=dotnet" alt=".NET"/></a>
<a href="https://developer.android.com/media/camera/camerax" title="Android / CameraX"><img src="https://skillicons.dev/icons?i=androidstudio" alt="Android"/></a>

**Backend e dados**

<a href="https://nodejs.org/docs/latest/api/" title="Node.js"><img src="https://skillicons.dev/icons?i=nodejs" alt="Node.js"/></a>
<a href="https://expressjs.com/" title="Express"><img src="https://skillicons.dev/icons?i=express" alt="Express"/></a>
<a href="https://www.sqlite.org/docs.html" title="SQLite"><img src="https://skillicons.dev/icons?i=sqlite" alt="SQLite"/></a>

**IA e mídia local**

<a href="https://github.com/ggml-org/whisper.cpp" title="whisper.cpp">whisper.cpp</a>
· <a href="https://github.com/ggml-org/llama.cpp" title="llama.cpp">llama.cpp</a>
· <a href="https://ffmpeg.org/documentation.html" title="FFmpeg">FFmpeg</a>
· <a href="https://docs.comfy.org/" title="ComfyUI">ComfyUI</a>

**Automação e integrações**

<a href="https://discord.js.org/" title="discord.js">discord.js</a>
· <a href="https://tesseract-ocr.github.io/" title="Tesseract OCR">Tesseract OCR</a>
· <a href="https://sharp.pixelplumbing.com/" title="sharp">sharp</a>
· <a href="https://obsproject.com/wiki/" title="OBS Studio">OBS Studio</a>
· <a href="https://developer.android.com/" title="Android">Android</a>

**Qualidade e entrega**

<a href="https://www.docker.com/" title="Docker"><img src="https://skillicons.dev/icons?i=docker" alt="Docker"/></a>
<a href="https://docs.github.com/actions" title="GitHub Actions"><img src="https://skillicons.dev/icons?i=github" alt="GitHub Actions"/></a>
<a href="https://learn.microsoft.com/windows/" title="Windows"><img src="https://skillicons.dev/icons?i=windows" alt="Windows"/></a>
<a href="https://git-scm.com/doc" title="Git"><img src="https://skillicons.dev/icons?i=git" alt="Git"/></a>
<a href="https://code.visualstudio.com/docs" title="Visual Studio Code"><img src="https://skillicons.dev/icons?i=vscode" alt="Visual Studio Code"/></a>
<br/>
<a href="https://vitest.dev/" title="Vitest">Vitest</a>
· <a href="https://xunit.net/" title="xUnit">xUnit</a>
· <a href="https://docs.github.com/actions" title="GitHub Actions">GitHub Actions (CI)</a>
· <a href="https://www.electron.build/" title="electron-builder">electron-builder</a>

</div>

## Princípios de desenvolvimento

- **Utilidade primeiro:** construir para resolver uma necessidade concreta.
- **Validar antes de afirmar:** distinguir recursos testados, em desenvolvimento e indisponíveis.
- **Transparência técnica:** explicar fontes de dados, limites e comportamento dos módulos.
- **Evoluir com feedback:** prototipar, testar no uso real e aprimorar.

## Atividade no GitHub

<div align="center">

<img width="49%" height="195" src="https://github-readme-stats.vercel.app/api?username=lucao019&show_icons=true&hide_border=true&bg_color=080b16&title_color=67e8f9&icon_color=f59e0b&text_color=cbd5e1&rank_icon=github" alt="Estatísticas do GitHub"/>
<img width="49%" height="195" src="https://github-readme-stats.vercel.app/api/top-langs/?username=lucao019&layout=compact&hide_border=true&bg_color=080b16&title_color=67e8f9&text_color=cbd5e1&langs_count=8" alt="Linguagens mais usadas"/>

<img width="98%" src="https://streak-stats.demolab.com/?user=lucao019&hide_border=true&background=080b16&ring=22d3ee&fire=f59e0b&currStreakLabel=67e8f9&sideLabels=cbd5e1&currStreakNum=ffffff&sideNums=ffffff&dates=94a3b8" alt="Sequência de contribuições"/>

<br/><br/>

<sub>Projetos em evolução contínua: construir, validar no uso real e compartilhar o que funciona.</sub>

</div>
