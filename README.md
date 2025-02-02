Aqui está o `README` atualizado para o código modificado:

---

# Projeto Controle de LEDs com Temporizador

Este código utiliza um microcontrolador Raspberry Pi Pico para controlar dois LEDs (vermelho e verde), alternando entre eles a cada 3 segundos.

## Funcionalidades
- **Alternância de LEDs**: O LED verde e o LED vermelho alternam a cada 3 segundos.
- **Contagem de tempo**: O código imprime no terminal a contagem de tempo a cada segundo.

## Hardware Necessário
- Raspberry Pi Pico
- 1 LED vermelho
- 1 LED verde

## Pinos Utilizados
- **LED Vermelho**: GPIO 13
- **LED Verde**: GPIO 11

## Como Funciona

1. **LEDs**: O código utiliza um temporizador repetido a cada 3 segundos para alternar entre os LEDs. O LED vermelho e o LED verde alternam da seguinte forma:
   - Quando o LED vermelho está apagado, o LED verde acende.
   - Quando o LED verde está apagado, o LED vermelho acende.
   
2. **Contagem de Tempo**: A cada segundo, o programa imprime a quantidade de segundos passados no terminal.

## Dependências
- Biblioteca `pico/stdlib.h` (padrão da Raspberry Pi Pico)
- Biblioteca `hardware/timer.h` (para temporizadores)

## Como Usar

1. **Carregar o código**: Compile e carregue o código no Raspberry Pi Pico utilizando o ambiente de desenvolvimento adequado (como o Visual Studio Code com a extensão do Raspberry Pi Pico).
   
2. **Conectar os componentes**: Conecte os LEDs aos pinos GPIO conforme mencionado.

3. **Monitorar a saída**: Abra o terminal serial para observar a contagem de tempo ("Passou X segundo(s)") e acompanhar o comportamento dos LEDs.

## Observações

- O código utiliza um temporizador repetitivo a cada 3 segundos para alternar os LEDs.
- A cada segundo, o programa imprime a contagem de tempo no terminal.
