# Sistema de Controle de Reservatório de Água - Simulação Tinkercad

Projeto de engenharia desenvolvido em **C++/Arduino** para monitoramento de nível de fluídos e controle automatizado de fluxo, projetado e validado no ambiente **Tinkercad**.

## Visualização da Simulação
![Circuito do Sistema de Reservatório](TinkerCAD%20Hardware.png)

## Funcionalidade
O sistema utiliza um sensor ultrassônico para medir o nível da água em um reservatório. A lógica controla dois motores/relés que operam como comportas (portões) para gerenciar a entrada e saída de água:

- **Nível Seguro (>= 50cm de distância do sensor):** Indica que o reservatório precisa ser abastecido ou está em nível operacional baixo. O sistema ativa o **portão de entrada** (relé abrir) para permitir o fluxo de água.
- **Nível Crítico (< 50cm de distância do sensor):** Indica que o reservatório está cheio. O sistema ativa o **portão de fechamento** (relé fechar) para interromper o fluxo e evitar transbordamento.

Sinalização visual via LEDs indica o status do sistema em tempo real (Verde para Seguro/Aberto, Vermelho para Crítico/Fechado).

## Hardware Simulado
- Microcontrolador Arduino Uno R3
- Sensor Ultrassônico HC-SR04 (Monitor de Nível)
- Módulo Relé (Controle das Comportas/Motores)
- Dois motores CC
- LEDs de sinalização e resistores

## Conceitos Aplicados
- **Automação Industrial:** Controle de fluxo baseado em sensores de nível.
- **C++ Embarcado:** Lógica de decisão e manipulação de I/O digital.
- **Simulação de Hardware:** Validação de comportamento e proteção contra falhas (transbordamento) via Tinkercad.

## Link para a Simulação
[Clique aqui para ver o projeto diretamente no Tinkercad](https://www.tinkercad.com/things/ksFeE0sgaf9-automacao-com-sensor-ultrassonico?sharecode=QiOTAEoDRZjMi9ixoWHbPVdneMrDHn57GZM-_4xWkz8)
