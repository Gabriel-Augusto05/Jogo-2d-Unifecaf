# Jogo-2d-Unifecaf

🎮 2D Tilemap Platformer — Unity

Um jogo de plataforma 2D desenvolvido na Unity como projeto final da disciplina de Game Development (UniFECAF). O jogo foi criado para demonstrar habilidades técnicas e criativas no uso da engine Unity, incluindo mecânicas de movimento fluido, design de níveis progressivos, sistema de coletáveis, animações e áudio.


📸 Screenshots

<img width="1677" height="945" alt="Captura de tela 2026-06-11 193115" src="https://github.com/user-attachments/assets/5a845de8-1654-409f-bc38-fd6ed3b48343" />


🕹️ Sobre o Jogo

O jogador controla um personagem que percorre fases com plataformas, coleta moedas e supera obstáculos em níveis de dificuldade crescente. As mecânicas foram projetadas para respeitar a curva de aprendizado clássica dos jogos de plataforma side-scrolling.


✨ Funcionalidades


Movimentação completa: andar, correr e pulo duplo (double jump)
Animações fluidas: Idle, Run e Jump sincronizadas com as ações do personagem
Sistema de Tilemap: cenários modulares criados com o Tilemap da Unity
Moedas e Coletáveis: sistema de coleta com incremento de pontuação
HUD funcional: exibição de pontuação, vidas e itens em tempo real
Sistema de morte e respawn: o personagem reaparece ao morrer
Game Manager & UI Manager: gerenciamento centralizado do estado do jogo
Feedback visual e sonoro: efeitos em cada ação do jogador
Trilha sonora: música de fundo coerente com a atmosfera do jogo



🎯 Mecânicas de Jogo

MecânicaDescriçãoAndarMovimentação horizontal com Input.GetAxisRaw()Pulo duploDois saltos consecutivos, o segundo disponível no arGrounded checkPhysics2D.OverlapCircle() nos pés do personagemColeta de moedasOnTriggerEnter2D() + notificação ao GameManagerRespawnReposicionamento ao ponto de spawn ao morrerFlip de spriteSpriteRenderer.flipX conforme direção de movimento


🗺️ Design de Níveis

O jogo conta com 3 a 5 fases com progressão de dificuldade:


Fase 1 — Tutorial implícito: plataformas largas, poucos obstáculos, ideal para aprender os controles
Fase 2 — Gaps e pulo duplo: lacunas maiores exigem uso do double jump
Fase 3 — Obstáculos dinâmicos: plataformas móveis e inimigos em patrulha
Fases 4–5 (opcional): combinação de todos os elementos em layouts mais complexos



🎮 Controles

TeclaAçãoA / ←Mover para a esquerdaD / →Mover para a direitaEspaçoPular / Pulo duploEscPausar / Menu


🚀 Como Executar

Jogar o executável


Baixe a pasta compactada do jogo na seção Releases do repositório
Extraia o conteúdo
Execute o arquivo 2DPlatformer.exe (Windows) ou o equivalente para seu sistema operacional


Abrir no Unity (código-fonte)


Clone o repositório:


Abra o Unity Hub e clique em Add project from disk
Selecione a pasta clonada
Certifique-se de usar uma versão do Unity compatível (Unity 2020.x ou superior recomendado)
Abra a cena principal em Assets/Scenes/
Pressione Play para testar



🗂️ Estrutura do Projeto

2D-platformer/
├── Assets/
│   ├── Scenes/          # Cenas do jogo (fases + menu)
│   ├── Scripts/         # Scripts C# (PlayerController, GameManager, UIManager...)
│   ├── Sprites/         # Sprites do personagem, inimigos e cenário
│   ├── Tilemaps/        # Tilesets utilizados nos níveis
│   ├── Animations/      # Animator Controllers e Animation Clips
│   ├── Audio/           # Trilha sonora e efeitos sonoros
│   └── Prefabs/         # Prefabs reutilizáveis (moedas, inimigos, etc.)
├── ProjectSettings/
└── README.md


🛠️ Tecnologias Utilizadas


Unity Engine — desenvolvimento do jogo e ferramentas de animação
C# — programação de todas as mecânicas e sistemas
Unity Tilemap — criação modular dos cenários
Unity Animator — máquina de estados para animações do personagem
Git / GitHub — controle de versão e hospedagem do projeto



🎨 Assets Utilizados

Os sprites, tilesets e áudios utilizados são provenientes de repositórios gratuitos com licença aberta. Créditos:


Sprites e tiles: OpenGameArt.org / itch.io Free Assets
Efeitos sonoros: freesound.org
Trilha sonora: assets gratuitos com licença CC0 / CC-BY



Caso algum asset específico exija crédito adicional, ele está listado no arquivo CREDITS.txt dentro da pasta Assets/.




📋 Requisitos do Sistema

ItemRequisito mínimoSistema OperacionalWindows 10 / macOS 10.14 / Ubuntu 18.04ProcessadorIntel Core i3 ou equivalenteMemória RAM4 GBPlaca de VídeoSuporte a DirectX 11 / OpenGL 3.2Armazenamento~500 MB



🎓 Disciplina: Game Development — UniFECAF
