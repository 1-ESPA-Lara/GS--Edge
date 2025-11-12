# Projeto: Wellness Reminder – Ambiente Inteligente de Trabalho
## Descrição do Projeto

O Wellness Reminder é um sistema baseado em Arduino desenvolvido para melhorar o bem-estar e as condições de trabalho em ambientes corporativos, educacionais ou laboratoriais.
O projeto monitora temperatura e luminosidade do ambiente em tempo real e alerta, por meio de LEDs e um buzzer, quando as condições estão fora dos limites ideais.
Além disso, o sistema incentiva pausas regulares a cada hora, promovendo descanso físico e mental, contribuindo para a saúde e produtividade dos trabalhadores.

## Visão Geral do Projeto
Simulação disponivel no Wokwi:https://wokwi.com/projects/447270124587428865
<img width="442" height="361" alt="image" src="https://github.com/user-attachments/assets/18b9dae1-620a-462c-b860-880a71e9b680" />


## Funcionalidades

- Monitoramento ambiental: mede continuamente temperatura, umidade e luminosidade.
- Alertas visuais e sonoros: acende LED vermelho e ativa buzzer se as condições estiverem fora dos limites ideais.
- Feedback positivo: LED verde aceso quando o ambiente está adequado.
- Controle de tempo de descanso: a cada 1 hora, o sistema exibe no LCD a contagem regressiva para a próxima pausa e emite um alarme de descanso.
- Armazenamento de dados: grava os valores de temperatura e luminosidade na EEPROM, mantendo histórico entre reinicializações.
- Interface intuitiva: LCD 16x2 exibe ícones de temperatura, luz e o tempo restante até a próxima pausa.
- Interação com joystick: pausa o alarme e confirma o retorno do colaborador ao trabalho.

## Conceitos Envolvidos
- Automação e Internet das Coisas (IoT): uso de sensores e atuadores para criar ambientes inteligentes.
- Ergonomia digital: equilíbrio entre conforto e produtividade.
- Sustentabilidade e eficiência energética: controle de luminosidade ideal reduz consumo e fadiga visual.
- Saúde ocupacional: incentivo a pausas periódicas para prevenir estresse e fadiga.
- Armazenamento não volátil (EEPROM): preservação dos últimos dados coletados.
- Programação embarcada: aplicação prática de lógica condicional, temporização (millis()), sensores analógicos e digitais.

## Como Reproduzir o Projeto
### 1 Montagem dos componentes
Monte o circuito conforme os pinos definidos no código:
| Componente              | Pino do Arduino     |
| ----------------------- | ------------------- |
| DHT11 (data)            | 2                   |
| Buzzer                  | 3                   |
| LED Verde               | 4                   |
| LED Vermelho            | 5                   |
| LCD 16x2 (RS, E, D4-D7) | 12, 11, 10, 9, 8, 7 |
| RTC DS1307 (SDA, SCL)   | A4, A5              |
| LDR                     | A0                  |
| Botão Joystick          | 13                  |
### 2 Carregamento do código
- Abra o Arduino IDE.
- Copie e cole o código completo comentado.
- Selecione a placa (Arduino Uno) e a porta correta.
- Faça o upload para o Arduino.
### 3 Execução
- Ao ligar, o display mostra uma animação de inicialização.
- O sistema começa a medir temperatura e luminosidade.
- Se estiver tudo certo → LED verde acende.
- Caso contrário → LED vermelho acende e buzzer toca.
- A cada hora → aparece aviso “Hora da pausa!” e buzzer soa até o joystick ser pressionado.

## Componentes Utilizados
| Componente                   | Função                                     |
| ---------------------------- | ------------------------------------------ |
| **Arduino UNO**              | Microcontrolador principal                 |
| **Sensor DHT11**             | Mede temperatura e umidade                 |
| **Sensor LDR**               | Detecta luminosidade ambiente              |
| **RTC DS1307**               | Mantém controle do tempo e data            |
| **Display LCD 16x2**         | Exibe informações do sistema               |
| **LED Verde e LED Vermelho** | Indicadores de status                      |
| **Buzzer Piezoelétrico**     | Alerta sonoro                              |
| **Joystick (botão)**         | Interação com o usuário                    |
| **EEPROM interna**           | Armazenamento permanente de dados          |
| **Resistores e jumpers**     | Conexões elétricas e segurança do circuito |

## Licença
Este projeto é de uso educacional e livre, podendo ser reproduzido, modificado e compartilhado para fins acadêmicos, desde que mantida a referência ao projeto original e ao contexto do desafio Global Solution – FIAP 2025.

## Equipe de Desenvolvimento 
- Lara Mofid Essa Alssabak — RM567947
- Maria Luisa Boucinhos Franco — RM567355
- Roberta Moreira dos Santos — RM567825

## Conclusão
O Wellness Reminder propõe uma solução tecnológica simples e acessível para promover ambientes de trabalho mais saudáveis e humanos.
Ao unir automação, sustentabilidade e bem-estar, o projeto contribui para o debate sobre o Futuro do Trabalho, mostrando como pequenas inovações podem gerar grandes impactos na qualidade de vida e produtividade das pessoas.
