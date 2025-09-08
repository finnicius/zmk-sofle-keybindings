# Sofle - Teclado Mecânico para Português Brasileiro

- [Português](README.md)
- [English](README_EN.md)

## 📋 Índice

- [Visão Geral](#visão-geral)
- [Características Principais](#características-principais)
- [Layout das Camadas](#layout-das-camadas)
- [Instalação Rápida](#instalação-rápida)
- [Flashing do Firmware](#flashing-do-firmware)
- [Personalização](#personalização)
- [Solução de Problemas](#solução-de-problemas)

## Visão Geral

Este é um firmware personalizado para o teclado Sofle, otimizado especificamente para **digitação em português brasileiro**. O layout foi projetado para permitir digitação completa em PT-BR com acesso fácil a acentos, cedilhas e caracteres especiais.

## Características Principais

### ✨ Digitação Completa em PT-BR
- **Layer 0**: Layout QWERTY padrão com cedilha (Ç) integrada
- **Layer 3**: Acentos completos (á, é, í, ó, ú, à, ã, â, ê, ô)
- **Tap-dance**: C/ç/Ç com um único botão
- **Macros**: Acentos automáticos para digitação rápida

### 🎯 Layout Otimizado
- **Navegação**: Setas direcionais no centro do teclado
- **Mídia**: Controles de volume no slider
- **Mouse**: Emulação de mouse integrada
- **Backlight**: Controle de brilho da iluminação

## Estrutura das Camadas

### Layer 0 - Base (Digitação Principal)
**Layout QWERTY com modificações para PT-BR:**

```
ESC  1  2  3  4  5    ↑    6  7  8  9  0  BACKSPACE
TAB  Q  W  E  R  T    ↓    Y  U  I  O  P  DEL
SHIFT A  S  D  F  G    ←    H  J  K  L  ;  '
CTRL Z  X  C  V  B    →    N  M  ,  .  /  RCTRL
WIN ALT TAB L1 SPACE/ESC   SPACE ENTER L2 BSPC PRTSC/DESKTOP
```

**Características especiais:**
- **Acentos completos**: Vogais com tap-dance múltiplo:
  - **A**: 1 toque=A, 2 toques=á, 3 toques=à, 4 toques=ã
  - **E**: 1 toque=E, 2 toques=é, 3 toques=ê
  - **I**: 1 toque=I, 2 toques=í
  - **O**: 1 toque=O, 2 toques=ó, 3 toques=ô
  - **U**: 1 toque=U, 2 toques=ú
- **Cedilha integrada**: Tecla C com tap-dance (C/ç/Ç)
- **Shift inteligente**: Hold-tap para Shift (tap=Shift, hold=Caps Lock)
- **Space/Escape**: Hold-tap para Space (tap=Space, hold=Escape)
- **Print Screen/Desktop**: Hold-tap para captura (tap=Print Screen, hold=Mostrar Desktop)
- **Setas no centro**: Navegação sem sair da posição de digitação
- **Controles de mídia**: Mute no canto inferior esquerdo
- **Volume**: Controle via slider (encoder)
- **Ergonomia otimizada**: Space e Enter lado a lado no polegar direito

### Layer 1 - Símbolos e Mouse
**Acesso rápido a símbolos e emulação de mouse:**

```
ESC `  '  @  $  |    ↑    |  $  @  '  `  ESC
TAB  ~  ^  *  (  )    ↓    (  )  *  ^  ~  TAB
SHIFT +  -  %  [  ]    ←    [  ]  %  -  +  SHIFT
CTRL /  =  _  {  }    →    {  }  _  =  \  CTRL
MUTE GUI ALT TAB L1   SPACE/ESC SPACE ENTER SHIFT BSPC PRTSC/DESKTOP
```

**Funcionalidades:**
- **Símbolos**: Parênteses, colchetes, chaves, operadores
- **Mouse**: Movimento e clique esquerdo
- **Scroll**: Encoder para rolagem

### Layer 2 - Numpad Dedicado
**Teclado numérico completo:**

```
`  trans trans trans trans trans    ↑    7  8  9  /  *  BACKSPACE
   trans trans trans trans trans    ↓    4  5  6  +  -  DEL
   trans trans trans trans trans    ←    1  2  3  ENTER =  '
   trans trans trans trans trans    →    0  .  ENTER SPACE ENTER trans
   trans trans trans trans trans    LCLK trans trans trans trans trans
```

**Funcionalidades:**
- **Numpad completo**: Todos os números e operadores
- **Mouse**: Movimento e clique esquerdo
- **Scroll**: Encoder para rolagem
- **Layout ergonômico**: Numpad na mão direita, mouse no centro

## Comportamentos Especiais

### Tap-Dance Completo para Acentos
As vogais no Layer 0 possuem comportamentos especiais:

**Cedilha:**
- **1 toque**: C
- **2 toques**: ç (cedilha minúscula)
- **3 toques**: Ç (cedilha maiúscula)

**Vogais com acentos completos:**
- **A**: 1 toque=A, 2 toques=á, 3 toques=à, 4 toques=ã
- **E**: 1 toque=E, 2 toques=é, 3 toques=ê
- **I**: 1 toque=I, 2 toques=í
- **O**: 1 toque=O, 2 toques=ó, 3 toques=ô
- **U**: 1 toque=U, 2 toques=ú

### Macros de Acentos
Cada acento é uma macro que combina dead-key + letra:
- **Acentos agudos**: ' + letra (á, é, í, ó, ú)
- **Acentos graves**: ` + letra (à)
- **Tils**: ~ + letra (ã)
- **Circunflexos**: ^ + letra (â, ê, ô)

### Hold-Tap Behaviors

**Shift/Caps Lock:**
- **Tap**: Shift (modificador)
- **Hold**: Caps Lock (toggle)

**Space/Escape:**
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

## Configuração e Uso

### Acesso às Camadas
- **Layer 1**: Segurar tecla inferior esquerda (L1)
- **Layer 2**: Segurar tecla inferior direita (L2)
- **Layer 3**: L1 + L2 (momentaneamente)

### Controles de Mídia
- **Mute**: Tecla inferior esquerda (Layer 0)
- **Volume**: Slider (encoder) no lado direito
- **Scroll**: Encoder no Layer 1 e 2

### Mouse
- **Movimento**: Setas direcionais no centro (Layer 1 e 2)
- **Clique**: Pressionar o joystick/controle direcional
- **Scroll**: Encoder (Layer 1 e 2)

## Vantagens para PT-BR

### ✅ Digitação Eficiente
- **Cedilha integrada**: Sem necessidade de combinações complexas
- **Acentos rápidos**: Layer dedicado com macros otimizadas
- **Layout familiar**: QWERTY com melhorias

### ✅ Produtividade
- **Navegação central**: Setas sem mover as mãos
- **Sticky keys**: Modificadores que ficam ativos
- **Mouse integrado**: Sem necessidade de mouse externo

### ✅ Ergonomia
- **Teclado dividido**: Reduz tensão nos ombros
- **Thumb clusters otimizados**: Space e Enter lado a lado no polegar direito
- **Escape acessível**: Hold no Space esquerdo (sem esticar mindinho)
- **Page Up/Down no polegar**: Navegação sem mover as mãos
- **Backspace no polegar**: Edição confortável
- **Camadas lógicas**: Organização intuitiva

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
2. **Segure** o botão reset (geralmente na parte inferior)
3. **Conecte** o USB mantendo o botão pressionado
4. **Solte** o botão reset
5. **Aguarde** 2-3 segundos

**Alternativas:**
- **Duplo reset**: Pressione o botão reset duas vezes rapidamente
- **Combinação de teclas**: Layer 2 + tecla BT (Bluetooth)

#### **Passo 2: Fazer Flash**

1. **Verifique** que apareceu um novo drive USB (ex: "SOFLEBOOT")
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

**Use uma das camadas existentes como template:**

```c
// Template baseado na layer_1 (símbolos)
layer_3 {
    bindings = <
        /* ========== LINHA 1 ========== */
        &kp ESC            // Posição 1: ESC
        &kp N1             // Posição 2: 1
        &kp N2             // Posição 3: 2
        &kp N3             // Posição 4: 3
        &kp N4             // Posição 5: 4
        &kp N5             // Posição 6: 5
        
        &kp UP_ARROW       // Posição 7: Seta para cima
        
        &kp N6             // Posição 8: 6
        &kp N7             // Posição 9: 7
        &kp N8             // Posição 10: 8
        &kp N9             // Posição 11: 9
        &kp N0             // Posição 12: 0
        &kp BACKSPACE      // Posição 13: Backspace
        
        /* Continue mapeando todas as 64 posições... */
        /* Use &trans para posições que herdam da camada base */
    >;
    display-name = "layer_3";
    sensor-bindings = <&inc_dec_kp C_VOLUME_UP C_VOL_DN>;
};
```

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

## 🎨 Layout Atual

![Layout atual da configuração](keymap-drawer/eyelash_sofle.svg)