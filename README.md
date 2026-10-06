📱 Stateful Motion - Generative UI Error State (E-Commerce)
Animação interativa de Stateful Motion simulando o estado de erro e contingência em uma interface de Generative UI para E-Commerce de Eletrônicos (Smartphones), desenvolvida com React, Shadcn/UI, Framer Motion e Tailwind CSS.

Stateful Motion Banner

🌟 Principais Recursos
🤖 Robô Vetorial 2D Animado (SVG Native): Robô em vetor 2D flutuante (@keyframes robotFloat), com piscada de olhos e brilho de antena em 60fps.
📱 Layout Mobile iPhone (iOS Realista):
Barra Superior iOS: Relógio (09:41), Sinal de Rede 5G, Wi-Fi e ícone de bateria preenchido com indicador, acompanhado da Dynamic Island / Notch.
Barra Inferior iOS: Home Indicator (Barra de gestos iOS na base).
💬 Barra de Conversa & Entrada de Áudio: Barra inferior de chat com campo de texto, botão de microfone/áudio e ação de envio.
📦 Contingência com 3 Celulares (Degradação Graciosa): Exibição de 3 opções topo de linha (iPhone 15 Pro Max, Galaxy S24 Ultra, Xiaomi 14 Ultra) com fotos em alta definição.
🎨 Design System Clean Shadcn/UI:
Touch targets ergonomicamente dimensionados em ≥48px para facilitar o toque em telas mobile.
Grade de espaçamento estrita em múltiplos de 8px.
⚡ Zero Dependências de Servidor (demo.html): Arquivo nativo em HTML5/CSS3/JS que abre diretamente em qualquer navegador com um duplo-clique.
📐 Cobertura das 5 Regras de Heurística de UX
Linguagem Humana & Transparente: Frase clara sem jargões técnicos ("A nossa ligação ao sistema de estoque de eletrônicos oscilou momentaneamente.").
Caminhos de Recuperação Imediatos: Botões de 1-toque [Tentar novamente agora] e [Ver alternativas disponíveis].
Degradação Graciosa: Transição fluida para um card contendo 3 smartphones em estoque preservando o contexto da busca.
Tom Empático & Voice/Tone: Mensagem acolhedora com botão de reprodução em síntese de voz (Speech Synthesis API).
Transição Visual & Loading Skeleton: Skeleton Loader animado de pulsação suave ao tentar novamente.
🚀 Como Executar
Opção 1: Abrir o Protótipo Standalone (Sem instalar nada)
Basta dar um duplo-clique no arquivo 
demo.html
 para abrir a aplicação completa e funcional direto no seu navegador!

Opção 2: Projeto React (Vite + Tailwind CSS)
Clone o repositório:
bash

git clone https://github.com/SEU_USUARIO/stateful-motion-error-ui.git
cd stateful-motion-error-ui
Instale as dependências:
bash

npm install
Execute o servidor de desenvolvimento:
bash

npm run dev
🎨 Especificações para o Figma (Smart Animate)
Crie um Component Set no Figma com o nome Generative UI Mobile Electronics:


Component Set: "Generative UI Mobile Electronics"
├── [Variant=Streaming_Generative]   -> Stream com animação de digitação
├── [Variant=Error_Stateful]          -> Robô 2D Animado + Mensagem Empática
├── [Variant=Skeleton_Loading]        -> Pulsador de Carregamento Shimmer
└── [Variant=Graceful_Contingency]    -> Lista de 3 Celulares em Estoque
Configuração de Prototipagem no Figma:
No botão [Tentar Novamente]:
Trigger: On Click
Action: Change to [Variant: Skeleton_Loading]
Animation: Smart Animate
Easing: Custom Cubic Bezier (0.16, 1, 0.3, 1)
Duration: 400ms
📁 Estrutura de Arquivos do Projeto

stateful-motion-error-ui/
├── index.html                   # HTML base do Vite
├── demo.html                    # Demonstrador standalone 100% nativo (GitHub Pages)
├── package.json                 # Dependências e scripts do projeto
├── README.md                    # Documentação do projeto
├── .gitignore                   # Arquivos ignorados pelo Git
├── src/
│   ├── main.jsx                 # Entrada principal React
│   ├── App.jsx                  # Container da aplicação
│   ├── index.css                # Estilos globais Tailwind e animações CSS
│   ├── lib/
│   │   └── utils.js             # Helper cn() do Shadcn UI
│   ├── components/
│   │   ├── AnimatedRobotVector.jsx  # Vetor SVG animado do robô 2D
│   │   ├── MobileDeviceFrame.jsx   # Moldura iPhone iOS (Bateria, Status Bar, Notch)
│   │   ├── MobileChatInputBar.jsx  # Barra de conversa e botão de áudio
│   │   ├── StatefulErrorCard.jsx   # Card de erro com robô 2D
│   │   ├── ContingencyCard.jsx    # Card de degradação graciosa (3 celulares)
│   │   ├── SkeletonLoader.jsx      # Skeleton loader de pulsação
│   │   ├── GenerativeStreamingCard.jsx # Stream animado pre-erro
│   │   └── ui/                     # Componentes Shadcn UI (Button, Card, Badge, Input, Skeleton)
│   └── data/
│       └── mockData.js          # Catálogo de smartphones e mensagens
📤 Como Enviar para o GitHub
No terminal da pasta do projeto, execute os comandos:

bash

git init
git add .
git commit -m "feat: Stateful Motion Generative UI Error State com Robô 2D e 3 Smartphones"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git
git push -u origin main
Para publicar no GitHub Pages:

Vá em Settings > Pages no repositório do GitHub.
Em Source, selecione a branch main e a pasta / (root).
O seu arquivo demo.html ficará acessível publicamente na web!
📄 Licença
Este projeto está sob a licença MIT. Sinta-se à vontade para utilizar e personalizar!
