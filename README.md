# Ponderada de Programação - Semana 1

## Descrição

O projeto tem como objetivo demonstrar o uso de LEDs interno e externo no Arduino, criando um efeito de pisca-pisca que simula um giroflex policial. A seguir, estão as instruções e as imagens que ilustram o funcionamento do projeto.

### Parte 1: Pisca-Pisca com LED Interno
Nesta primeira parte, o código faz o LED interno do Arduino (embutido na placa) piscar.

<img src="./arduino_IDE.png" alt="LED Interno" width="900"/>

### Parte 2: Pisca-Pisca com LED Externo

Na segunda parte, o LED externo é conectado através de um circuito com jumpers e resistores de 330 Ohms. O LED pisca de acordo com o código implementado, simulando um giroflex.

[Link para o projeto no Tinkercad](https://www.tinkercad.com/things/09GLeNYcB4M-cool-albar?sharecode=G1Gp1OpqpWnm4ci0B3Ww3iCjPUBOY7L6I1wRaoB7TMo)

<img src="./thinkercad.png" alt="Circuito no Tinkercad" width="900"/>


##### Ambos os Leds piscam a cda 1000ms

#### Demonstração 


<img src="./demo.png" alt="Circuito no Tinkercad" width="900"/>

#### Código em C++ do LED Externo e Interno 

```cpp
void setup()
{
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop()
{
  digitalWrite(LED_BUILTIN, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
}
```




### Ir Além: Sistema Físico - Giroflex Simulado

Além do projeto no Tinkercad, foi construído um sistema físico com dois LEDs piscando de forma alternada para simular o efeito de um giroflex policial.

<img src="./giroflex.jpeg" alt="Giroflex Simulado" width="900"/>

Construi o sistema físico no protoboard como dois leds piscando de forma sequencial de maneira que simule um giroflex policial. 
## Funcionamento do Projeto

1. **Código LED Interno**: Faz o LED embutido no Arduino piscar.
2. **Circuito Externo**: Implementa um LED externo piscando com resistores e jumpers.
3. **Expansão**: O sistema físico foi construído para criar um efeito de dois LEDs piscando sequencialmente, simulando um giroflex.

---

### Clonagem do Projeto

Você pode clonar este repositório usando o comando:

```bash
git clone https://github.com/Bernardomeirelles/arduino.git
