# Semaforo
Temporizador periódico utilizando Pico SDK

## Funcionamento 📋
O programa utiliza a função add_repeating_timer_ms(), presente no pacote Pico SDK para executar as seguintes operações (utilizando 3 leds e 3 resistores de 300 ohms ou a placa BitDogLab):

### Utilizando 3 leds e 3 resistores de 300 ohms:
- O LED vermelho acende durante 3 segundos e os LEDs amarelo e verde permanecem apagados.
- O LED amarelo acende durante 3 segundos e os LEDs vermelho e verde permanecem apagados.
- O LED verde acende durante 3 segundos e os LEDs vermelho e amarelo permanecem apagados.

### Utilizando a placa BitDogLab:
- O LED vermelho acende durante 3 segundos e os LEDs azul e verde permanecem apagados.
- O LED azul acende durante 3 segundos e os LEDs vermelho e verde permanecem apagados.
- O LED verde acende durante 3 segundos e os LEDs vermelho e azul permanecem apagados.

## Requisitos cumpridos pelo projeto
1. Uso de temporizador: aplicação da função add_repeating_timer_ms().
2. Acionamento dos LEDs (sinais do semáforo) iniciando pela cor vermelha, alterando para amarela e, em seguida, verde.
3. Temporizador ajustado para um atraso de 3 segundos(3000 ms).
4. Mudança de estado dos LEDs implementa na função de call-back do temporizador (repeating_timer_callback()).
5. A rotina principal imprime algum tipo de informação a cada segundo (1000 ms).
6. Na placa BitDogLab é utilizado o LED RGB.