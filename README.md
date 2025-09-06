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
TAB  Q  W  É  R  T    ↓    Y  Ú  Í  Ó  P  DEL
SHIFT Á  S  D  F  G    ←    H  J  K  L  ;  '
CTRL Z  X  Ç  V  B    →    N  M  ,  .  /  RCTRL
MUTE GUI ALT APP L1   SPACE/ESC SPACE ENTER L2 PG_UP/DN BACKSPACE
```

**Características especiais:**
- **Acentos completos**: Vogais com tap-dance múltiplo:
  - **A**: 1 toque=A, 2 toques=á, 3 toques=à, 4 toques=ã
  - **E**: 1 toque=E, 2 toques=é, 3 toques=ê
  - **I**: 1 toque=I, 2 toques=í
  - **O**: 1 toque=O, 2 toques=ó, 3 toques=ô
  - **U**: 1 toque=U, 2 toques=ú
- **Cedilha integrada**: Tecla C com tap-dance (C/ç/Ç)
- **Shift inteligente**: Tap-dance para Shift (tap=Shift, double-tap=Caps Lock)
- **Space/Escape**: Hold-tap para Space (tap=Space, hold=Escape)
- **Page Up/Down**: Hold-tap para navegação (tap=Page Up, hold=Page Down)
- **Setas no centro**: Navegação sem sair da posição de digitação
- **Controles de mídia**: Mute no canto inferior esquerdo
- **Volume**: Controle via slider (encoder)
- **Ergonomia otimizada**: Space e Enter lado a lado no polegar direito

### Layer 1 - Símbolos e Números
**Acesso rápido a símbolos e emulação de mouse:**

```
`  1  2  3  4  5    ↑    6  7  8  9  0  trans
    |  \  -  *  /    ↓    (  )  [  ]  +  _
    trans trans trans trans trans  ←    {  }  :  ;  ?  "
    trans trans trans trans trans  →    <  >  /  \  trans trans
MUTE trans trans trans trans trans  LCLK trans trans trans trans trans
```

**Funcionalidades:**
- **Símbolos**: Parênteses, colchetes, chaves, operadores
- **Mouse**: Movimento e clique esquerdo
- **Scroll**: Encoder para rolagem

### Layer 2 - Navegação e Edição
**Ferramentas de produtividade:**

```
`  trans trans trans trans trans    ↑    HOME UP END PG_UP PSCRN trans
   STICKY_CTRL STICKY_ALT STICKY_GUI STICKY_SHIFT trans  ↓    LEFT DOWN RIGHT trans PG_DN trans
   CTRL ALT GUI SHIFT trans        ←    DEL BSPC CUT COPY PASTE UNDO
   trans trans trans trans trans    →    BL_DEC BL_INC BL_TOG trans trans trans
   trans trans trans trans trans    LCLK trans trans trans trans trans
```

**Funcionalidades:**
- **Navegação**: Home, End, Page Up/Down, Print Screen
- **Edição**: Cut, Copy, Paste, Undo
- **Sticky Keys**: Modificadores que ficam ativos
- **Backlight**: Controle de brilho
- **Mouse**: Movimento e clique

### Layer 3 - Acentos PT-BR
**Acentos completos para português brasileiro:**

```
trans trans trans trans trans trans    trans trans trans trans trans trans trans
     '     `     ~     ^     "         á     é     í     ó     ú    trans
     à     ã     â     ê     ô         trans trans trans trans trans trans trans
     trans trans  Ç   trans trans      trans trans trans trans trans trans trans
     trans trans trans trans trans      trans trans trans trans trans
```

**Acentos disponíveis:**
- **Agudos**: á, é, í, ó, ú
- **Graves**: à
- **Tils**: ã
- **Circunflexos**: â, ê, ô
- **Cedilha**: Ç (tap-dance: C/ç/Ç)

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

### Combo de Soft Off
**Q + S + Z** (segurados por 2 segundos):
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
- **Movimento**: Setas no Layer 1 e 2
- **Clique**: Tecla central inferior
- **Scroll**: Encoder

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

2. **Entendendo os códigos ZMK:**
   - **Teclas padrão:** Use `&kp NOME_DA_TECLA` (ex: `&kp A`, `&kp ENTER`)
   - **Modificadores:** `&kp LCTRL`, `&kp LALT`, `&kp LSHFT`, `&kp LGUI`
   - **Mudança de camada:** `&mo NUMERO_DA_CAMADA` (momentâneo), `&to NUMERO_DA_CAMADA` (toggle)
   - **Funções especiais:** `&bt BT_SEL 0` (dispositivo Bluetooth), `&sys_reset` (reset)
   - **Mouse:** `&mkp LCLK` (clique esquerdo), `&mmv MOVE_UP` (movimento do mouse)

3. **Recursos de documentação ZMK:**
   - [Documentação de Keymaps ZMK](https://zmk.dev/docs/keymaps)
   - [Referência de Códigos de Tecla ZMK](https://zmk.dev/docs/keymaps/keycodes)
   - [Comportamentos ZMK](https://zmk.dev/docs/behaviors)
   - [Lista Completa de Códigos de Tecla](https://zmk.dev/docs/keymaps/list-of-keycodes)
   - [Modificadores ZMK](https://zmk.dev/docs/keymaps/modifiers)
   - [Tap-Dance ZMK](https://zmk.dev/docs/behaviors/tap-dance)
   - [Hold-Tap ZMK](https://zmk.dev/docs/behaviors/hold-tap)
   - [Macros ZMK](https://zmk.dev/docs/behaviors/macros)

4. **Estrutura das camadas:**
   - **Layer 0:** Camada principal de digitação (QWERTY)
   - **Layer 1:** Camada de símbolos/mouse (F1-F12, setas, mouse)
   - **Layer 2:** Camada de navegação/edição (Bluetooth, reset)
   - **Layer 3:** Camada de acentos (vazia para personalização)

5. **Salve e teste:**
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

### Obtendo Ajuda

- **Documentação ZMK:** [zmk.dev/docs](https://zmk.dev/docs)
- **Comunidade Discord ZMK:** [discord.zmk.dev](https://zmk.dev/community/discord)
- **Exemplos de Keymap:** [zmk.dev/docs/keymaps/examples](https://zmk.dev/docs/keymaps/examples)
- **Contato:** [380465425@qq.com](mailto:380465425@qq.com)

## Histórico de Atualizações

- **2024/12/21**
  1. Adicionado suporte para zmk-studio (apenas atualize o lado esquerdo para usar).
- **2024/10/24**
  1. Modificado modo de alimentação para reduzir consumo de energia.
  2. Corrigida funcionalidade de desligamento automático para alimentação RGB.
- **2025/8/22**
  1. Atualizado o soft off. Quando você pressiona as teclas Q, S e Z simultaneamente e as segura por 2 segundos, o teclado entra em estado de sono profundo e não pode ser acordado pressionando teclas. Esta função pode ser usada ao transportá-lo. O método de ativação é pressionar o botão reset uma vez.
  2. Este mês, também atualizei as versões ultra-finas dos cases corne e sofle. A moldura e a placa base foram espessadas, e a abertura do botão reset foi ajustada, para que o botão reset possa ser pressionado facilmente. Atualmente, ainda estamos conceituando como projetar a carcaça com um suporte inclinado. Se você examinar cuidadosamente uma PCB, notará que há interfaces reservadas para expansão IO. Eu me pergunto se alguém conseguiu utilizá-las, vou tentar!
  3. As animações GIF na tela do teclado do lado direito foram removidas, o que reduzirá significativamente o consumo de energia do teclado do lado direito.

> Se seu sofle foi atualizado antes de 2025/8/22, atualize para o firmware mais recente.

## Contato

Para arquivos de modelo 3D impresso ou quaisquer problemas e mau funcionamento com o teclado, entre em contato [380465425@qq.com](mailto:380465425@qq.com)

## Layout do Sofle

![Sofle键位图](keymap-drawer/eyelash_sofle.svg)