# 🎮 Biblioteca Pygame – Desenvolvimento de Jogos em Python

##  Introdução

A **Pygame** é uma biblioteca **Python** usada para o **desenvolvimento de jogos 2D** e aplicações multimídia.  
Ela fornece funcionalidades para **gráficos**, **sons**, **animações** e **interações com teclado e mouse**, tornando a criação de jogos muito mais simples.

---

## Instalação

Antes de começar, é necessário instalar a biblioteca.  
No terminal (ou prompt de comando), execute:

```bash
pip install pygame
```

Após a instalação, verifique se tudo está funcionando:

```python
import pygame
print("Pygame instalado com sucesso!", pygame.ver)
```

---

## Estrutura básica de um jogo com Pygame

Um jogo em Pygame geralmente segue esta estrutura:

1. **Inicializar o Pygame**
2. **Criar a janela do jogo**
3. **Definir o loop principal (game loop)**
4. **Tratar eventos (teclado, mouse)**
5. **Atualizar a tela**

###  Exemplo básico

```python
import pygame
import sys

# Inicializa o Pygame
pygame.init()

# Define tamanho da tela
tela = pygame.display.set_mode((800, 600))
pygame.display.set_caption("Meu Primeiro Jogo")

# Define cor de fundo (RGB)
branco = (255, 255, 255)

# Loop principal do jogo
while True:
    # Verifica eventos
    for evento in pygame.event.get():
        if evento.type == pygame.QUIT:
            pygame.quit()
            sys.exit()

    # Preenche a tela
    tela.fill(branco)

    # Atualiza a tela
    pygame.display.flip()
```

---

## Desenhando na Tela

O Pygame permite desenhar **formas geométricas simples**, como retângulos, círculos e linhas.

### Exemplo:

```python
import pygame, sys
pygame.init()

tela = pygame.display.set_mode((600, 400))
pygame.display.set_caption("Desenhos no Pygame")

preto = (0, 0, 0)
vermelho = (255, 0, 0)
azul = (0, 0, 255)
verde = (0, 255, 0)

while True:
    for evento in pygame.event.get():
        if evento.type == pygame.QUIT:
            pygame.quit()
            sys.exit()

    tela.fill(preto)

    pygame.draw.rect(tela, vermelho, (50, 50, 100, 60))
    pygame.draw.circle(tela, azul, (300, 200), 50)
    pygame.draw.line(tela, verde, (0, 0), (600, 400), 5)

    pygame.display.flip()
```

---

## Controle de Movimento

Você pode mover objetos na tela utilizando **eventos do teclado**.

### Exemplo – Mover um quadrado:

```python
import pygame, sys

pygame.init()
tela = pygame.display.set_mode((600, 400))
pygame.display.set_caption("Movimento com o Teclado")

preto = (0, 0, 0)
branco = (255, 255, 255)
x, y = 300, 200
velocidade = 5

while True:
    for evento in pygame.event.get():
        if evento.type == pygame.QUIT:
            pygame.quit()
            sys.exit()

    teclas = pygame.key.get_pressed()
    if teclas[pygame.K_LEFT]:
        x -= velocidade
    if teclas[pygame.K_RIGHT]:
        x += velocidade
    if teclas[pygame.K_UP]:
        y -= velocidade
    if teclas[pygame.K_DOWN]:
        y += velocidade

    tela.fill(preto)
    pygame.draw.rect(tela, branco, (x, y, 50, 50))
    pygame.display.flip()
```

---

## Sons e Música

Pygame também pode tocar sons e trilhas de fundo.

### Exemplo de uso de som:

```python
import pygame
pygame.init()

# Carregar som
pygame.mixer.music.load('trilha.mp3')
pygame.mixer.music.play(-1)  # Toca em loop

som_efeito = pygame.mixer.Sound('pulo.wav')
som_efeito.play()
```

---

## Sprites e Imagens

Os **sprites** são imagens ou personagens usados em jogos.  
Eles podem se mover, colidir e interagir com outros objetos.

### Exemplo simples:

```python
import pygame, sys
pygame.init()

tela = pygame.display.set_mode((800, 600))
pygame.display.set_caption("Exemplo com Sprite")

personagem = pygame.image.load("personagem.png")
x, y = 300, 200

while True:
    for evento in pygame.event.get():
        if evento.type == pygame.QUIT:
            pygame.quit()
            sys.exit()

    teclas = pygame.key.get_pressed()
    if teclas[pygame.K_RIGHT]:
        x += 5
    if teclas[pygame.K_LEFT]:
        x -= 5

    tela.fill((0, 0, 0))
    tela.blit(personagem, (x, y))
    pygame.display.flip()
```

---

##  Controle de FPS (Frames por Segundo)

Para controlar a velocidade do jogo, usamos o objeto `Clock()`.

```python
relogio = pygame.time.Clock()

while True:
    relogio.tick(60)  # Limita a 60 FPS
```

---

## Mini Jogo Completo – “Quadrado Móvel”

```python
import pygame, sys

pygame.init()
tela = pygame.display.set_mode((800, 600))
pygame.display.set_caption("Quadrado Móvel")

relogio = pygame.time.Clock()
branco = (255, 255, 255)
vermelho = (255, 0, 0)

x, y = 100, 100
vel = 7

while True:
    for evento in pygame.event.get():
        if evento.type == pygame.QUIT:
            pygame.quit()
            sys.exit()

    teclas = pygame.key.get_pressed()
    if teclas[pygame.K_a]:
        x -= vel
    if teclas[pygame.K_d]:
        x += vel
    if teclas[pygame.K_w]:
        y -= vel
    if teclas[pygame.K_s]:
        y += vel

    tela.fill(branco)
    pygame.draw.rect(tela, vermelho, (x, y, 60, 60))

    pygame.display.flip()
    relogio.tick(60)
```

---

## Dicas Importantes

- Sempre **chame `pygame.init()`** antes de usar a biblioteca.  
- O **loop principal** do jogo nunca deve parar.  
- Use **`pygame.display.flip()`** para atualizar a tela.  
- Mantenha uma taxa de FPS estável com `Clock()`.  
- Organize seu jogo em **funções** e **classes** para facilitar o código.

---

## 💡 Recursos

- [Documentação oficial do Pygame](https://www.pygame.org/docs/)
- [Repositório no GitHub](https://github.com/pygame/pygame)
- [Tutoriais Pygame](https://www.pygame.org/wiki/tutorials)

---
