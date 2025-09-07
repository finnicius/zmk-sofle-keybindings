# Sofle - Teclado Mecânico para Português Brasileiro

- [Português](README.md)
- [English](README_EN.md)

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

## Instalação

### Pré-requisitos
- **Python 3.8+**
- **Git**
- **West** (meta-ferramenta do Zephyr)
- **CMake** (3.20.0 ou superior)
- **Ninja**
- **DTC** (Device Tree Compiler)

### Instalação das Dependências

#### Windows (usando Chocolatey)
```bash
choco install python git cmake ninja dtc
pip install west
```

#### Linux/Ubuntu
```bash
sudo apt update
sudo apt install python3 python3-pip git cmake ninja-build device-tree-compiler
pip3 install west
```

#### macOS
```bash
brew install python git cmake ninja dtc
pip3 install west
```

### Configuração do Workspace

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/finnicius/zmk-sofle-keybindings
   cd zmk-sofle-keybindings
   ```

2. **Inicialize o workspace West:**
   ```bash
   west init -l config
   west update
   ```

3. **Instale dependências do Zephyr:**
   ```bash
   pip install -r zephyr/scripts/requirements.txt
   ```

## Compilação do Firmware

### Opção 1: GitHub Actions (Recomendado)

1. **Faça commit e push das mudanças:**
   ```bash
   git add config/eyelash_sofle.keymap
   git commit -m "feat: atualizar configuração do keymap"
   git push origin main
   ```

2. **Monitore o processo de build:**
   - Vá para a aba **Actions** no seu repositório GitHub
   - Clique na execução mais recente do workflow "Build ZMK firmware"
   - Aguarde todos os jobs completarem (5-15 minutos)

3. **Baixe o firmware:**
   - Na página do workflow, role até "Artifacts"
   - Baixe os arquivos de firmware (`.uf2` para ambos os lados)
   - Os artefatos serão nomeados conforme sua configuração `build.yaml`

### Opção 2: Build Local

1. **Configure o ambiente Zephyr:**
   ```bash
   # No Windows
   west zephyr-export

   # No Linux/macOS
   source zephyr/zephyr-env.sh
   ```

2. **Compile o firmware:**
   ```bash
   # Lado direito
   west build -b eyelash_sofle_right -- -DSHIELD=nice_view

   # Lado esquerdo com suporte ZMK Studio
   west build -b eyelash_sofle_left -- -DSHIELD=nice_view -DCONFIG_ZMK_STUDIO=y

   # Lado esquerdo para reset de configurações
   west build -b eyelash_sofle_left -- -DSHIELD=settings_reset
   ```

3. **Localize os arquivos:**
   - Os arquivos estarão em `build/zephyr/zmk.uf2`

## Flashing do Firmware

### Usando UF2 Bootloader

O UF2 (USB Flashing Format) é o método mais confiável para fazer flash do firmware em ambos os lados do teclado.

#### **Passo 1: Entrar no Modo Bootloader**

**Método 1 - Botão Reset (Recomendado):**
1. **Desconecte** o teclado do USB
2. **Segure** o botão reset (geralmente na parte inferior)
3. **Conecte** o USB mantendo o botão pressionado
4. **Solte** o botão reset
5. **Aguarde** 2-3 segundos

**Método 2 - Duplo Reset:**
1. **Pressione** o botão reset duas vezes rapidamente
2. **Aguarde** o LED piscar (se houver)

**Método 3 - Combinação de Teclas:**
1. **Acesse** o Layer 2 (segure a tecla L2)
2. **Pressione** a tecla BT (Bluetooth)
3. **Aguarde** o LED piscar

#### **Passo 2: Verificar o Modo Bootloader**

Quando estiver no modo bootloader:
- **Windows**: Aparecerá um novo drive USB (ex: "SOFLEBOOT")
- **Linux/macOS**: Aparecerá um drive montado (ex: "/media/SOFLEBOOT")
- **LED**: Pode piscar de forma diferente (se houver LED)

#### **Passo 3: Fazer Flash do Firmware**

1. **Localize** o arquivo `.uf2` correto:
   - **Lado esquerdo**: `eyelash_sofle_left-nice_view-zmk.uf2`
   - **Lado direito**: `eyelash_sofle_right-nice_view-zmk.uf2`

2. **Copie** o arquivo `.uf2` para o drive USB que apareceu
   - **Windows**: Arraste e solte ou Ctrl+C/Ctrl+V
   - **Linux/macOS**: `cp arquivo.uf2 /caminho/do/drive/`

3. **Aguarde** a cópia completar (alguns segundos)

4. **O teclado reiniciará automaticamente** com o novo firmware

#### **Passo 4: Verificar se Funcionou**

- **LED**: Deve parar de piscar e voltar ao normal
- **Drive USB**: Deve desaparecer
- **Teclado**: Deve funcionar normalmente

#### **Troubleshooting**

**Problema: Drive não aparece**
- Tente o método 1 (botão reset + conectar USB)
- Verifique se o cabo USB está funcionando
- Tente uma porta USB diferente

**Problema: Arquivo não copia**
- Verifique se o arquivo `.uf2` não está corrompido
- Tente renomear o arquivo para algo mais simples
- Verifique se há espaço suficiente no drive

**Problema: Teclado não reinicia**
- Aguarde mais tempo (até 30 segundos)
- Desconecte e reconecte o USB
- Tente entrar no modo bootloader novamente

#### **Vantagens do UF2:**
- ✅ **Funciona em ambos os lados**
- ✅ **Não precisa de software especial**
- ✅ **Mais confiável** que outros métodos
- ✅ **Funciona em qualquer sistema operacional**

### Usando ZMK Studio (apenas lado esquerdo)

1. **Instale o ZMK Studio:**
   - Baixe de https://zmk.studio
   - Conecte seu teclado

2. **Atualize o firmware:**
   - Selecione seu dispositivo no ZMK Studio
   - Faça upload do arquivo de firmware

## Personalização

### Editando o Keymap

1. **Edite o arquivo:**
   - Abra `config/eyelash_sofle.keymap`
   - Cada camada é definida como um array `bindings`
   - As teclas são mapeadas em ordem específica (esquerda para direita, cima para baixo)

2. **Template de Camada (Recomendado):**
   
   Para facilitar a criação e manutenção dos layouts, use este template com uma tecla por linha:

```c
layer_exemplo {
    bindings = <
        /* ========== LINHA 1 ========== */
        /* Mão esquerda - Fileira 1 */
        &kp ESC,           // Posição 1: ESC
        &kp N1,            // Posição 2: 1
        &kp N2,            // Posição 3: 2
        &kp N3,            // Posição 4: 3
        &kp N4,            // Posição 5: 4
        &kp N5,            // Posição 6: 5
        
        /* Controle direcional - Movimento para cima */
        &kp UP_ARROW,      // Posição 7: Seta para cima
        
        /* Mão direita - Fileira 1 */
        &kp N6,            // Posição 8: 6
        &kp N7,            // Posição 9: 7
        &kp N8,            // Posição 10: 8
        &kp N9,            // Posição 11: 9
        &kp N0,            // Posição 12: 0
        &kp BACKSPACE,     // Posição 13: Backspace
        
        /* ========== LINHA 2 ========== */
        /* Mão esquerda - Fileira 2 */
        &kp TAB,           // Posição 14: Tab
        &kp Q,             // Posição 15: Q
        &kp W,             // Posição 16: W
        &kp E,             // Posição 17: E
        &kp R,             // Posição 18: R
        &kp T,             // Posição 19: T
        
        /* Controle direcional - Movimento para baixo */
        &kp DOWN_ARROW,    // Posição 20: Seta para baixo
        
        /* Mão direita - Fileira 2 */
        &kp Y,             // Posição 21: Y
        &kp U,             // Posição 22: U
        &kp I,             // Posição 23: I
        &kp O,             // Posição 24: O
        &kp P,             // Posição 25: P
        &kp DEL,           // Posição 26: Delete
        
        /* ========== LINHA 3 ========== */
        /* Mão esquerda - Fileira 3 */
        &kp LSHFT,         // Posição 27: Shift esquerdo
        &kp A,             // Posição 28: A
        &kp S,             // Posição 29: S
        &kp D,             // Posição 30: D
        &kp F,             // Posição 31: F
        &kp G,             // Posição 32: G
        
        /* Controle direcional - Movimento para esquerda */
        &kp LEFT_ARROW,    // Posição 33: Seta para esquerda
        
        /* Mão direita - Fileira 3 */
        &kp H,             // Posição 34: H
        &kp J,             // Posição 35: J
        &kp K,             // Posição 36: K
        &kp L,             // Posição 37: L
        &kp SEMI,          // Posição 38: Ponto e vírgula
        &kp APOS,          // Posição 39: Aspas simples
        
        /* ========== LINHA 4 ========== */
        /* Mão esquerda - Fileira 4 */
        &kp LCTRL,         // Posição 40: Ctrl esquerdo
        &kp Z,             // Posição 41: Z
        &kp X,             // Posição 42: X
        &kp C,             // Posição 43: C
        &kp V,             // Posição 44: V
        &kp B,             // Posição 45: B
        
        /* Controle direcional - Movimento para direita */
        &kp RIGHT_ARROW,   // Posição 46: Seta para direita
        
        /* Mão direita - Fileira 4 */
        &kp N,             // Posição 47: N
        &kp M,             // Posição 48: M
        &kp COMMA,         // Posição 49: Vírgula
        &kp DOT,           // Posição 50: Ponto
        &kp FSLH,          // Posição 51: Barra
        &kp RSHFT,         // Posição 52: Shift direito
        
        /* ========== LINHA 5 ========== */
        /* Encoder - Pressionamento do volume knob */
        &kp C_MUTE,        // Posição 53: Pressionar encoder/volume knob
        
        /* Mão esquerda - Thumb cluster */
        &kp LGUI,          // Posição 54: GUI esquerdo
        &kp LALT,          // Posição 55: Alt esquerdo
        &kp TAB,           // Posição 56: Tab
        &mo 1,             // Posição 57: Momentâneo Layer 1
        &space_escape ESC SPACE,  // Posição 58: Space/Escape (hold-tap)
        
        /* Controle direcional - Pressionamento do joystick */
        &mkp LCLK,         // Posição 59: Pressionar controle direcional/joystick
        
        /* Mão direita - Thumb cluster */
        &kp ENTER,         // Posição 60: Enter
        &kp SPACE,         // Posição 61: Space
        &mo 2,             // Posição 62: Momentâneo Layer 2
        &kp BSPC,          // Posição 63: Backspace
        &prtscr_desktop 0 0  // Posição 64: Print Screen/Desktop (hold-tap)
    >;
    display-name = "LAYER_EXEMPLO";
    /* Encoder = volume */
    sensor-bindings = <&inc_dec_kp C_VOLUME_UP C_VOL_DN>;
};
```

3. **Entendendo os códigos ZMK:**
   - **Teclas padrão:** Use `&kp NOME_DA_TECLA` (ex: `&kp A`, `&kp ENTER`)
   - **Modificadores:** `&kp LCTRL`, `&kp LALT`, `&kp LSHFT`, `&kp LGUI`
   - **Mudança de camada:** `&mo NUMERO_DA_CAMADA` (momentâneo), `&to NUMERO_DA_CAMADA` (toggle)
   - **Funções especiais:** `&bt BT_SEL 0` (dispositivo Bluetooth), `&sys_reset` (reset)
   - **Mouse:** `&mkp LCLK` (clique esquerdo), `&mmv MOVE_UP` (movimento do mouse)

4. **Recursos de documentação ZMK:**
   - [Documentação de Keymaps ZMK](https://zmk.dev/docs/keymaps)
   - [Referência de Códigos de Tecla ZMK](https://zmk.dev/docs/keymaps/keycodes)
   - [Comportamentos ZMK](https://zmk.dev/docs/behaviors)
   - [Lista Completa de Códigos de Tecla](https://zmk.dev/docs/keymaps/list-of-keycodes)
   - [Modificadores ZMK](https://zmk.dev/docs/keymaps/modifiers)
   - [Tap-Dance ZMK](https://zmk.dev/docs/behaviors/tap-dance)
   - [Hold-Tap ZMK](https://zmk.dev/docs/behaviors/hold-tap)
   - [Macros ZMK](https://zmk.dev/docs/behaviors/macros)

5. **Estrutura das camadas:**
   - **Layer 0:** Camada principal de digitação (QWERTY com acentos)
   - **Layer 1:** Camada de símbolos e mouse (símbolos, mouse, scroll)
   - **Layer 2:** Camada de numpad dedicado (números, operadores, mouse)
   - **Layer 3:** Camada vazia (disponível para personalização)

6. **Salve e teste:**
   - Salve o arquivo
   - Faça commit e push para acionar GitHub Actions
   - Baixe os arquivos de firmware gerados

### Visualização do Keymap

Para gerar uma representação visual do seu keymap:

1. Faça push das mudanças para o GitHub
2. A GitHub Action gerará automaticamente um SVG em `keymap-drawer/eyelash_sofle.svg`

## Solução de Problemas

### Problemas Comuns

**West update falha:**
```bash
# Limpe o cache do west e tente novamente
west update --narrow
```

**Build falha com dependências ausentes:**
```bash
# Reinstale os requisitos
pip install -r zephyr/scripts/requirements.txt
```

**Teclado não reconhecido:**
- Tente um cabo USB diferente
- Tente uma porta USB diferente
- Verifique se o teclado está no modo bootloader

**Problemas de conexão ZMK Studio:**
- Certifique-se de usar o firmware do lado esquerdo com suporte Studio
- Verifique a conexão USB
- Tente atualizar a interface do Studio

### Solução de Problemas de Edição de Keymap

**Problemas comuns de keymap:**
- **Build falha com erro de sintaxe:** Verifique ponto e vírgula ausentes ou formato incorreto de código de tecla
- **Tecla não funciona:** Verifique se o código de tecla existe na documentação ZMK
- **Camada não muda:** Certifique-se de que os números das camadas coincidem (0, 1, 2, 3) e use o comportamento correto (`&mo` vs `&to`)
- **Mouse não funciona:** Verifique se os comportamentos de mouse estão configurados corretamente no keymap

**Testando suas mudanças:**
- Sempre teste mudanças de keymap em um lado primeiro antes de fazer flash em ambos
- Use o lado esquerdo com suporte ZMK Studio para testes mais fáceis
- Mantenha backups de configurações de keymap funcionais

### Metades não se comunicam após update (ZMK split BLE)

**Descrição curta do problema:**  
Após atualizar o firmware, o lado direito liga, mas não envia teclas e **pressionar a tecla de layer no lado direito não altera o layer exibido no display do lado esquerdo**. Isso indica falta de comunicação entre as metades do split (BLE/internal link).

**Causa provável:**  
Inconsistência de *roles* (central/peripheral) e/ou *settings/bonds* BLE entre as metades — comum quando a mesma UF2 é gravada nos dois lados ou quando o reset só foi feito em um lado.

#### Procedimento de recuperação
1. **Reset (apagar settings/bonds) em ambos**
   - `settings_reset_right` → desconectar e reiniciar
   - `settings_reset_left`  → desconectar e reiniciar

2. **Flash do firmware "normal" (binários distintos)**
   - **Primeiro** o lado direito: `eyelash_sofle_right` (peripheral)
   - **Depois** o lado esquerdo: `eyelash_sofle_left` (central)  
     *(use a variante `..._studio_left` se quiser ZMK Studio)*

3. **Boot e pareamento**
   - Ligar **as duas metades** (o **right** deve conectar ao **left** automaticamente)
   - Apagar pareamentos BLE antigos do **PC** com o teclado (se houver)
   - Parear **apenas o lado esquerdo** com o computador

4. **Teste funcional**
   - Pressionar **layer key** no **lado direito** e confirmar que o **display do lado esquerdo** muda de layer
   - Testar digitação no **lado direito** no host
   - Se falhar, **repetir**: reset dos dois lados → flash *right* → flash *left* → pareamento

### Obtendo Ajuda

- **Documentação ZMK:** [zmk.dev/docs](https://zmk.dev/docs)
- **Comunidade Discord ZMK:** [discord.zmk.dev](https://zmk.dev/community/discord)
- **Exemplos de Keymap:** [zmk.dev/docs/keymaps/examples](https://zmk.dev/docs/keymaps/examples)
- **Contato:** [380465425@qq.com](mailto:380465425@qq.com)

## Contato

Para arquivos de modelo 3D impresso ou quaisquer problemas e mau funcionamento com o teclado, entre em contato [380465425@qq.com](mailto:380465425@qq.com)

## Meu Layout Atual

![Layout atual da configuração](keymap-drawer/eyelash_sofle.svg)