git add .# Simulacao-2D-Equipe-OuroBots
Projeto da Equipe OuroBots no RoboCup Soccer Simulator 2D (RCSS) para desenvolvimento de agentes em C++.

##⚽ Simulação 2D – Equipe OuroBots

Projeto da Equipe OuroBots para desenvolvimento de agentes de futebol no RoboCup Soccer Simulator 2D (RCSS), utilizando C++.

Este repositório foi estruturado para permitir que várias pessoas programem juntas, cada uma responsável por uma parte do robô, com organização, clareza e sem conflitos de código.

---

##🧠 Ideia geral do projeto (em linguagem simples)

Pense no robô como um jogador de futebol:

Ele possui uma base comum
(ver o jogo, se mover, chutar, etc.)

Ele pode assumir papéis diferentes:

- Atacante

- Defensor

- Goleiro

Cada papel é programado separadamente, e depois tudo é conectado no arquivo principal.

---

## 📁 Estrutura do Projeto (explicada)

```text
Simulacao-2D-Equipe-OuroBots/
├── src/
│   ├── core/
│   │   ├── agent_base.h
│   │   └── agent_base.cpp
│   │
│   ├── attack/
│   │   ├── attack.h
│   │   └── attack.cpp
│   │
│   ├── defense/
│   │   ├── defense.h
│   │   └── defense.cpp
│   │
│   ├── goalie/
│   │   ├── goalie.h
│   │   └── goalie.cpp
│   │
│   └── main.cpp
│
├── include/        # Headers compartilhados (uso futuro)
├── scripts/        # Scripts auxiliares (uso futuro)
├── docs/           # Documentação
├── README.md       # Este arquivo
└── .gitignore
```

---

##📂 O que cada parte do código faz

###🔹 src/core/ — Base do agente

Contém o código base do robô, utilizado por todos os papéis.

Aqui ficam funcionalidades comuns, como:

- Leitura das informações do jogo

- Posição da bola e do robô

- Funções básicas: andar, girar, chutar

👉 Pense nisso como:
“Tudo que QUALQUER jogador precisa saber fazer”

Este código é infraestrutura comum e fica sob responsabilidade do(a) líder do projeto.

###🔹 src/attack/ — Ataque

Responsável pelo comportamento ofensivo do robô.

Exemplos:

- Ir atrás da bola

- Chutar para o gol

- Se posicionar para receber passe

###🔹 src/defense/ — Defesa

Responsável pelo comportamento defensivo.

Exemplos:

- Marcar adversários

- Proteger o gol

- Afastar a bola da área

###🔹 src/goalie/ — Goleiro

Responsável pelo comportamento do goleiro.

Exemplos:

- Posicionar-se corretamente no gol

- Defender chutes

- Sair do gol em situações específicas

###🔹 src/main.cpp — Arquivo principal

Arquivo central do projeto.

Responsável por:

- Inicializar o programa

- Criar o agente

- Definir se ele será atacante, defensor ou goleiro

- Chamar o comportamento correspondente

👉 O main.cpp orquestra, mas não contém lógica complexa.

---

##📄 Arquivos .h e .cpp (explicação simples)

.h (header)
Define o que a classe ou módulo faz
(declarações, interfaces)

.cpp (source)
Define como isso é feito
(implementação da lógica)

👉 Regra geral:

.h → contrato

.cpp → implementação

---

##👥 Organização da Equipe (branches)

As branches do projeto já foram criadas para manter padrão e evitar erros.

Branches existentes:

- main → versão oficial do projeto
(base do agente + integração)

- attack → desenvolvimento do ataque

- defense → desenvolvimento da defesa

- goalie → desenvolvimento do goleiro

Cada integrante** não** cria uma branch nova.
Ele apenas trabalha na branch correspondente à sua função.

❌ Não trabalhar na main
❌ Não criar branches extras sem combinar

---

##🔄 Passo a passo para cada integrante

###1️⃣ Clonar o repositório
```
git clone <link-do-repositorio>
cd Simulacao-2D-Equipe-OuroBots
```
###2️⃣ Entrar na branch da sua função
```
git checkout attack
```
ou
```
git checkout defense
```
ou
```
git checkout goalie
```
###3️⃣ Programar apenas no seu módulo

- Ataque → src/attack/

- Defesa → src/defense/

- Goleiro → src/goalie/

###4️⃣ Salvar o trabalho
```
git add .
git commit -m "Implementa comportamento inicial do módulo"
```
###5️⃣ Enviar para o GitHub
```
git push origin nome-da-branch
```
Depois disso, o código será revisado e integrado à branch principal.

---

##🎯 Objetivo inicial do projeto

Neste primeiro momento, o objetivo é:

- Aprender a trabalhar em equipe

- Manter o projeto organizado

- Criar uma base sólida

- Evoluir o robô aos poucos

---

##🔜 Próximos passos

- Integrar os módulos no main.cpp

- Criar comportamentos simples

- Conectar com o simulador RoboCup 2D

###✨ Fim do README


