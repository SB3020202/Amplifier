# README - Projeto Final de Eletrónica I

## Índice
1. [Visão Geral](#visão-geral)
2. [Especificações do Projeto](#especificações-do-projeto)
3. [Modalidades e Cronograma](#modalidades-e-cronograma)
4. [Planeamento do Trabalho](#planeamento-do-trabalho)
5. [Análise Teórica e Simulação](#análise-teórica-e-simulação)
6. [Montagem e Ensaio Experimental](#montagem-e-ensaio-experimental)
7. [Relatórios e Entregáveis](#relatórios-e-entregáveis)
8. [Diagramas do Circuito](#diagramas-do-circuito)
9. [Contribuidores](#contribuidores)

---

## Visão Geral
Neste Projeto Final de Eletrónica I (DEEC / FCT-UNL), dimensionámos, simulámos e testámos experimentalmente um **amplificador de áudio para smartphone** com potência de saída ≥ 0,25 W, utilizando topologia multiandar (par diferencial, emissor comum com multiplicador de V_BE e etapa push-pull).

## Especificações do Projeto
- **Potência de saída mínima:** 0,25 W
- **Ganho mínimo do AMPOP (3 andares):** ≥ 43 dB :contentReference[oaicite:0]{index=0}
- **Ganho da montagem inversora/non-inversora:** ≥ 20 dB :contentReference[oaicite:1]{index=1}
- **Alimentação:**
  - Opção A: single-supply, V_CC = +12 V
  - Opções B & C: dual-supply, V_CC = +6 V e V_EE = –6 V :contentReference[oaicite:2]{index=2}
- **Corrente de polarização (IRC2):** 15 mA – 25 mA
- **Carga (alto-falante):** 8 Ω (ou substituída por RL = 1 kΩ–3 kΩ nas leituras) :contentReference[oaicite:3]{index=3}

## Modalidades e Cronograma
Cada grupo (até 3 elementos) escolhe **Opção A (20 Valores)**, **B (17 Valores)** ou **C (15 Valores)**, podendo transitar conforme metas parciais :contentReference[oaicite:4]{index=4}.

| Aula  | Ação (Opção A)                              | Ação (Opções B & C)                   |
|:-----:|:---------------------------------------------|:--------------------------------------|
| 1     | Ensaio do par diferencial                   | Ensaio do par diferencial            |
| 2–3   | Análise teórica e simulação                 | Mesma análise                         |
| 4–5   | Montagem completa e ensaio em laboratório    | Montagem parcial (B) / ensaio (C)     |
| 6     | Ensaio final e otimização                   | Ensaio final                          | 

## Planeamento do Trabalho
1. **Análise Teórica & Dimensionamento:** deduzir equações para resistências RC1, RE1, RE2, RC2, R_Fonte, RM1/RM2 :contentReference[oaicite:5]{index=5}.  
2. **Simulação LTspice:** ponto de funcionamento DC (PFR), resposta AC (Av, ri, ro) e transiente (1 kHz) :contentReference[oaicite:6]{index=6}.  
3. **Montagem:** breadboard ou PCB (Opção A), completar parcialmente (B) ou teste em módulo (C) :contentReference[oaicite:7]{index=7}.  
4. **Ensaio Experimental:** medir tensões nodais, correntes, ganhos e potência de saída; analisar forma de onda e comparar com simulação :contentReference[oaicite:8]{index=8}.  

## Análise Teórica e Simulação
- Utilizar software (Python/Octave ou Excel) para calcular parâmetros e gerar gráficos auxiliares (não obrigatório para B/C) :contentReference[oaicite:9]{index=9}.  
- Obter PFR: medir VC1, VC2, V_x, VO1, VO2, VO, IF1 e confirmar se transístores estão em zona ativa :contentReference[oaicite:10]{index=10}.  
- Simulação dinâmica: injetar sinal 1 kHz, calcular Av1, Av2, Av_total; determinar impedâncias de entrada e saída :contentReference[oaicite:11]{index=11}.  

## Montagem e Ensaio Experimental
- **Opção A:** montagem completa em breadboard/PCB; atenção à polaridade de condensadores e ajustes de potenciómetros IF1 e V_BE :contentReference[oaicite:12]{index=12}.  
- **Opção B:** montar apenas resistores-chave e ensaiar; **Opção C:** ensaio em módulo montado.  
- Configurar fontes com limite 200–300 mA para evitar danos. Monitorar correntes e ajustar multiplicador de V_BE para obter V_ODC ≈ 0 V (dual-supply) ou V_CC/2 (single-supply) :contentReference[oaicite:13]{index=13}.  
- Registar formas de onda em vin, vo1, vo2 e vo; substituir RL por alto-falante para teste áudio e documentar observações :contentReference[oaicite:14]{index=14}.  

## Relatórios e Entregáveis
- **Parte 1 (Análise & Simulação):** equações, dimensionamento, gráficos e resultados sintéticos.  
- **Parte 2 (Experimento & Discussão):** dados experimentais, comparação com simulação e comentários.  
- Incluir turno, composição do grupo e distribuição de tarefas em ambas as partes :contentReference[oaicite:15]{index=15}.  

## Diagramas do Circuito

![Diagrama Simplificado do Amplificador](./images/diagrama_simplificado.png)

![Esquemático Completo com Fontes e Mult. VBE](./images/esquematico_multiandar.png)

## Contribuidores
- **[Nome do Estudante 1]** — Análise teórica e simulação  
- **[Nome do Estudante 2]** — Montagem e ensaio experimental  
- **[Nome do Estudante 3]** — Documentação e relatório  

*Para dúvidas, consulte o Moodle ou contacte o docente.*  
