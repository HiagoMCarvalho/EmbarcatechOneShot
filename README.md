# Embarcatech OneShot

## Descrição
Este projeto implementa um software que em conjunto com a ferramenta de desenvolvimento BitDogLab faz com que 3 leds sejam acionados 
e desligados individualmente através de um sistema de alarme

## Funcionalidades
- Controle automatizado do tempo de sinalização.
- Indicação visual através de LEDs.
- Ajuste dinâmico de tempos de espera.
- Implementação de rotinas de alarme 

## Estrutura do Projeto
```
OneShot/
├── .gitignore
├── CMakeLists.txt          # Configuração do build
├── diagram.json            # Esquema de conexões
├── OneShot.c              # Lógica principal do sistema
├── wokwi.toml              # Configuração da simulação no Wokwi
```

## Requisitos
- **Hardware**: Microcontrolador compatível (Raspberry Pi Pico), LEDs
- **Software**:
  - Ambiente de desenvolvimento C/C++
  - Simulador Wokwi (opcional)
  - CMake

## Como Compilar e Executar
1. Clone o repositório e acesse a pasta do projeto:
   ```sh
   git clone https://github.com/HiagoMCarvalho/EmbarcatechOneShot.git
   cd OneShot
   ```
2. Configure e compile o projeto:
   ```sh
   mkdir build && cd build
   cmake ..
   make
   ```
3. Carregue o firmware no Raspberry Pi Pico copiando o arquivo `.uf2` para a unidade correspondente.

## Simulação no Wokwi
1. Acesse [Wokwi](https://wokwi.com/) e importe os arquivos `diagram.json` e `wokwi.toml`.
2. Inicie a simulação para visualizar o funcionamento do projeto sem precisar de hardware físico.

## Licença
Este projeto é distribuído sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

## Autor
Desenvolvido por <https://github.com/HiagoMCarvalho>.

