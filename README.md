# Eyelash Sofle - Teclado para Português Brasileiro (pt-br)

Este é um firmware personalizado para o teclado Eyelash Sofle, otimizado especificamente para **digitação em português brasileiro**. O layout foi projetado para permitir digitação completa em PT-BR com acesso fácil a acentos, cedilhas e caracteres especiais.

## ✨ Características Principais

- **Digitação completa em PT-BR**: Acentos, cedilhas e caracteres especiais integrados
- **Tap-dance inteligente**: C/ç/Ç e vogais acentuadas com um único botão
- **Layout ergonômico**: Teclado dividido com navegação central
- **Mouse integrado**: Emulação de mouse e scroll
- **Controles de mídia**: Volume e mute integrados
- **Numpad dedicado**: Teclado numérico completo

## 🎨 Layout Atual

![Layout atual da configuração](keymap-drawer/eyelash_sofle.svg)

## 📋 Índice

- [Primeiros Passos](#primeiros-passos)
- [Estrutura das Camadas](#estrutura-das-camadas)
- [Comportamentos Especiais](#comportamentos-especiais)
- [Instalação Rápida](#instalação-rápida)
- [Flashing do Firmware](#flashing-do-firmware)
- [Personalização](#personalização)
- [Solução de Problemas](#solução-de-problemas)
- [Contato](#contato)

## 🚀 Primeiros Passos

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/finnicius/zmk-sofle-keybindings
   cd zmk-sofle-keybindings
   ```

2. **Baixe o firmware:**
   - Vá para a aba **Actions** no GitHub
   - Aguarde o build completar (5-15 minutos)
   - Baixe os arquivos `.uf2` na seção "Artifacts"

3. **Faça flash no teclado:**
   - Pressione duas vezes o botão RESET
   - Copie o arquivo `.uf2` para o drive que apareceu
   - Aguarde o teclado reiniciar

4. **Teste os acentos PT-BR:**
   - **A**: 1 toque=A, 2 toques=á, 3 toques=à, 4 toques=ã
   - **C**: 1 toque=C, 2 toques=ç, 3 toques=Ç

## 📚 Estrutura das Camadas

### Layer 0 - Digitação Principal (QWERTY + Acentos PT-BR)

- **Acentos completos**: Vogais com tap-dance múltiplo
- **Cedilha integrada**: Tecla C com tap-dance (C/ç/Ç)
- **Navegação central**: Setas direcionais no centro
- **Controles de mídia**: Volume via knob, mute ao pressionar
- **Ergonomia otimizada**: Space e Enter lado a lado no polegar direito

### Layer 1 - Símbolos e Emulação de Mouse

- **Símbolos**: Parênteses, colchetes, chaves, operadores
- **Mouse**: Movimento e clique esquerdo
- **Scroll**: Encoder para rolagem

### Layer 2 - Numpad Dedicado

- **Numpad completo**: Todos os números e operadores
- **Mouse**: Movimento e clique esquerdo
- **Scroll**: Encoder para rolagem
- **Layout ergonômico**: Numpad na mão direita, mouse no centro

## 🎯 Comportamentos Especiais

### Tap-Dance para Acentos PT-BR

- **A**: 1 toque=A, 2 toques=á, 3 toques=à, 4 toques=ã
- **E**: 1 toque=E, 2 toques=é, 3 toques=ê
- **I**: 1 toque=I, 2 toques=í
- **O**: 1 toque=O, 2 toques=ó, 3 toques=ô
- **U**: 1 toque=U, 2 toques=ú
- **C**: 1 toque=c, 2 toques=ç, 3 toques=Ç

### Hold-Tap Behaviors

**Shift/Caps Lock:**
- **Tap**: Shift (modificador)
- **Tap duplo**: Caps Lock (toggle)

**Space/Escape Esquerdo:**
- **Tap**: Space
- **Hold**: Escape

**Print Screen/Desktop:**
- **Tap**: Print Screen (captura de tela)
- **Hold**: Mostrar Desktop (Windows+D)

### Combo de Soft Off
**Z + X + C** (segurados por 2 segundos):
- Coloca o teclado em modo de sono profundo
- Útil para transporte
- Acordar: pressionar botão reset

### Acesso às Camadas
- **Layer 1**: Segurar tecla inferior esquerda (L1)
- **Layer 2**: Segurar tecla inferior direita (L2)
- **Layer 3**: L1 + L2 (momentaneamente)

### Controles de Mídia
- **Mute**: Pressionar o knob de volume (Layer 0)
- **Volume**: Girar o knob no lado direito
- **Scroll**: Girar o knob (Layer 1 e 2)

### Mouse
- **Movimento**: Setas direcionais no centro (Layer 1 e 2)
- **Clique**: Pressionar o joystick/controle direcional
- **Scroll**: Girar o knob (Layer 1 e 2)

## Instalação Rápida

### 🚀 Método Recomendado: GitHub Actions

**Para a maioria dos usuários, este é o método mais simples e confiável:**

1. **Clone e configure o repositório:**
   ```bash
   git clone https://github.com/finnicius/zmk-sofle-keybindings
   cd zmk-sofle-keybindings
   ```

2. **Faça suas personalizações:**
   - Edite `config/eyelash_sofle.keymap` conforme necessário
   - Faça commit das mudanças:
   ```bash
   git add config/eyelash_sofle.keymap
   git commit -m "feat: atualizar configuração do keymap"
   git push origin main
   ```

3. **Baixe o firmware:**
   - Vá para a aba **Actions** no seu repositório GitHub
   - Aguarde o build completar (5-15 minutos)
   - Baixe os arquivos `.uf2` na seção "Artifacts"

### 🔧 Build Local (Avançado)

**Apenas se você quiser compilar localmente ou fazer modificações no código:**

<details>
<summary>Clique para expandir instruções de build local</summary>

#### Pré-requisitos
- **Python 3.8+**
- **Git**
- **West** (meta-ferramenta do Zephyr)
- **CMake** (3.20.0 ou superior)
- **Ninja**
- **DTC** (Device Tree Compiler)

#### Instalação das Dependências

**Windows (usando Chocolatey):**
```bash
choco install python git cmake ninja dtc
pip install west
```

**Linux/Ubuntu:**
```bash
sudo apt update
sudo apt install python3 python3-pip git cmake ninja-build device-tree-compiler
pip3 install west
```

**macOS:**
```bash
brew install python git cmake ninja dtc
pip3 install west
```

#### Configuração e Build

1. **Configure o workspace:**
   ```bash
   west init -l config
   west update
   pip install -r zephyr/scripts/requirements.txt
   ```

2. **Configure o ambiente Zephyr:**
   ```bash
   # Windows
   west zephyr-export
   
   # Linux/macOS
   source zephyr/zephyr-env.sh
   ```

3. **Compile o firmware:**
   ```bash
   # Lado direito
   west build -b eyelash_sofle_right -- -DSHIELD=nice_view
   
   # Lado esquerdo com suporte ZMK Studio
   west build -b eyelash_sofle_left -- -DSHIELD=nice_view -DCONFIG_ZMK_STUDIO=y
   
   # Lado esquerdo para reset de configurações
   west build -b eyelash_sofle_left -- -DSHIELD=settings_reset
   ```

4. **Localize os arquivos:**
   - Os arquivos estarão em `build/zephyr/zmk.uf2`

</details>

## Flashing do Firmware

### 🎯 Método UF2 (Recomendado)

O UF2 é o método mais confiável para fazer flash do firmware em ambos os lados do teclado.

#### **Passo 1: Entrar no Modo Bootloader**

**Método mais simples:**
1. **Desconecte** o teclado do USB
2. **Pressione duas vezes o botão RESET** (na lateral do teclado)
3. **Confirme** que a luz azul começou a piscar
4. **Conecte** o USB

#### **Passo 2: Fazer Flash**

1. **Verifique** que apareceu um novo drive USB (ex: "NICENANO")
2. **Copie** o arquivo `.uf2` correto para o drive:
   - **Lado esquerdo**: `eyelash_sofle_left-nice_view-zmk.uf2`
   - **Lado direito**: `eyelash_sofle_right-nice_view-zmk.uf2`
3. **Aguarde** a cópia completar
4. **O teclado reiniciará automaticamente**

#### **Troubleshooting Rápido**

| Problema | Solução |
|----------|----------|
| Drive não aparece | Tente botão reset + conectar USB |
| Arquivo não copia | Verifique se o arquivo não está corrompido |
| Teclado não reinicia | Aguarde até 30 segundos |

### 🔧 ZMK Studio (apenas lado esquerdo)

1. **Instale** o ZMK Studio: https://zmk.studio
2. **Conecte** seu teclado
3. **Faça upload** do arquivo de firmware

## Personalização

### ✏️ Editando o Keymap

1. **Edite o arquivo:**
   - Abra `config/eyelash_sofle.keymap`
   - Cada camada é definida como um array `bindings`
   - As teclas são mapeadas em ordem específica (esquerda para direita, cima para baixo)

2. **Códigos ZMK principais:**
   - **Teclas padrão:** `&kp NOME_DA_TECLA` (ex: `&kp A`, `&kp ENTER`)
   - **Modificadores:** `&kp LCTRL`, `&kp LALT`, `&kp LSHFT`, `&kp LGUI`
   - **Mudança de camada:** `&mo NUMERO_DA_CAMADA` (momentâneo), `&to NUMERO_DA_CAMADA` (toggle)
   - **Funções especiais:** `&bt BT_SEL 0` (Bluetooth), `&sys_reset` (reset)
   - **Mouse:** `&mkp LCLK` (clique esquerdo), `&mmv MOVE_UP` (movimento)

3. **Estrutura das camadas:**
   - **Layer 0:** Camada principal de digitação (QWERTY com acentos)
   - **Layer 1:** Camada de símbolos e mouse
   - **Layer 2:** Camada de numpad dedicado
   - **Layer 3:** Camada vazia (disponível para personalização)

### 🆕 Criando uma Nova Camada

**Use uma das camadas existentes no config/eyelash_sofle.keymap** como ponto de partida, e edite as teclas

**Dicas importantes:**
- **Use `&trans`** para posições que devem herdar da camada base
- **Mapeie todas as 64 posições** (mesmo que algumas sejam `&trans`)
- **Adicione a camada ao keymap** após as camadas existentes
- **Configure o acesso** usando `&mo 3` ou `&to 3` em alguma tecla

### 🎯 Behaviors Essenciais do ZMK

**Behaviors** são funções especiais que definem como as teclas se comportam. Os principais tipos são:

#### **Hold-Tap**
- **Função:** Uma tecla que faz uma coisa quando pressionada rapidamente e outra quando segurada
- **Exemplo:** `&space_escape ESC SPACE` (tap=Space, hold=Escape)
- **Uso comum:** Modificadores, navegação, funções especiais

#### **Tap-Dance**
- **Função:** Uma tecla que faz coisas diferentes baseado no número de toques
- **Exemplo:** `&a_complete` (1 toque=A, 2 toques=á, 3 toques=à, 4 toques=ã)
- **Uso comum:** Acentos, símbolos múltiplos, funções relacionadas

#### **Macros**
- **Função:** Sequência de teclas executadas automaticamente
- **Exemplo:** `&macro_show_desktop` (Windows+D)
- **Uso comum:** Atalhos complexos, combinações de teclas

#### **Combos**
- **Função:** Ação ativada quando múltiplas teclas são pressionadas simultaneamente
- **Exemplo:** Z+X+C = Soft Off (desligar teclado)
- **Uso comum:** Funções especiais, atalhos de emergência

### 📚 Recursos de Documentação ZMK

**Links essenciais:**
- **[Lista Completa de Keycodes](https://zmk.dev/docs/keymaps/list-of-keycodes)** - Todos os códigos de tecla disponíveis
- **[Behaviors](https://zmk.dev/docs/behaviors)** - Documentação completa dos comportamentos
- **[Documentação de Keymaps](https://zmk.dev/docs/keymaps)** - Guia geral de keymaps
- **[Tap-Dance](https://zmk.dev/docs/behaviors/tap-dance)** - Comportamento de múltiplos toques
- **[Hold-Tap](https://zmk.dev/docs/behaviors/hold-tap)** - Comportamento de pressionar/seguar
- **[Macros](https://zmk.dev/docs/behaviors/macros)** - Sequências de teclas automáticas

4. **Salve e teste:**
   - Salve o arquivo
   - Faça commit e push para acionar GitHub Actions
   - Baixe os arquivos de firmware gerados

### 🎨 Visualização do Keymap

Para gerar uma representação visual do seu keymap:

1. Faça push das mudanças para o GitHub
2. A GitHub Action gerará automaticamente um SVG em `keymap-drawer/eyelash_sofle.svg`


## Solução de Problemas

### 🔧 Problemas Comuns

| Problema | Solução |
|----------|----------|
| **Teclado não reconhecido** | Tente cabo USB diferente ou porta diferente |
| **Build falha** | Verifique sintaxe do keymap e ponto e vírgula |
| **Tecla não funciona** | Verifique se o código existe na documentação ZMK |
| **Camada não muda** | Verifique números das camadas (0,1,2,3) e use `&mo` vs `&to` |
| **Mouse não funciona** | Verifique comportamentos de mouse no keymap |

### 🔄 Metades não se comunicam (ZMK split BLE)

**Sintoma:** Lado direito liga mas não envia teclas, tecla de layer no lado direito não altera display do lado esquerdo.

**Solução:**
1. **Reset em ambos os lados:**
   - Flash `settings_reset_right` → desconectar e reiniciar
   - Flash `settings_reset_left` → desconectar e reiniciar

2. **Flash firmware normal (ordem importante):**
   - **Primeiro** lado direito: `eyelash_sofle_right` (peripheral)
   - **Depois** lado esquerdo: `eyelash_sofle_left` (central)

3. **Pareamento:**
   - Ligar ambas as metades
   - Parear **apenas o lado esquerdo** com o computador
   - Testar se tecla de layer no lado direito altera display do esquerdo

### 📚 Obtendo Ajuda

- **Documentação ZMK:** [zmk.dev/docs](https://zmk.dev/docs)
- **Comunidade Discord:** [discord.zmk.dev](https://zmk.dev/community/discord)
- **Exemplos:** [zmk.dev/docs/keymaps/examples](https://zmk.dev/docs/keymaps/examples)

## 📞 Contato

Para arquivos de modelo 3D impresso ou problemas com o teclado: [380465425@qq.com](mailto:380465425@qq.com)

