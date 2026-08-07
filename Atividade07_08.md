# Análise do TCC

## Identificação do trabalho

| Item | Informação |
|---|---|
| **Título do trabalho** | **LembraMed – Desenvolvimento de um Sistema para Lembretes e Gerenciamento de Medicações** |
| **Curso** | **Ciência da Computação – Universidade Franciscana (UFN), Santa Maria – RS** |
| **Aluno** | **Guilherme S. Kuhn** |
| **Orientadora** | **Ana P. Canal** |
| **Link do trabalho** | https://www.tcconline.lapinf.ufn.edu.br/media/midias/TCC_II_5bxh4rt.pdf |

---

## Descrição básica do trabalho

O trabalho apresenta o desenvolvimento do **LembraMed**, uma aplicação web voltada ao **gerenciamento de medicamentos e ao envio de lembretes aos usuários**.

O sistema permite:

- cadastrar e gerenciar medicamentos;
- visualizar os medicamentos que devem ser utilizados no dia;
- registrar a utilização dos medicamentos;
- consultar o histórico de uso;
- acompanhar a data de validade dos medicamentos;
- receber lembretes por **SMS** no horário previsto para utilização do medicamento.

Para o desenvolvimento, foram utilizadas as seguintes tecnologias:

- **React** e **TypeScript** no frontend;
- **Node.js** e **Express** no backend;
- **MongoDB** para armazenamento dos dados;
- **Twilio** para envio das notificações por SMS.

O objetivo principal do sistema é auxiliar o usuário na organização de sua rotina de medicamentos, contribuindo para reduzir esquecimentos, erros de horário e uso de medicamentos vencidos.

---

# Rotinas da Saúde trabalhadas

## Quadro-resumo

| Rotina da Saúde | Trabalhada? | Classificação | Justificativa |
|---|:---:|---|---|
| **Diagnóstico** | ❌ **Não** | Não se aplica | O sistema não identifica doenças, condições clínicas ou problemas de saúde. O trabalho menciona diagnóstico apenas no referencial teórico, como uma possibilidade geral da Saúde Digital, mas essa funcionalidade não foi implementada no LembraMed. |
| **Monitoramento** | ✅ **Sim** | **Rotina principal** | O sistema acompanha medicamentos cadastrados, histórico de utilização, medicamentos previstos para o dia, horários de uso e datas de validade. Também registra data e hora da utilização dos medicamentos. |
| **Recomendação** | ✅ **Sim, com ressalva** | **Baseada em regras** | O sistema orienta e alerta o usuário sobre qual medicamento cadastrado deve ser utilizado e em qual horário, além de avisar sobre a validade. Não realiza recomendação médica, prescrição ou escolha automática de medicamentos. |
| **Predição / Previsão** | ❌ **Não** | Não se aplica | O sistema não utiliza modelos estatísticos, aprendizado de máquina ou algoritmos preditivos para estimar acontecimentos futuros. Os alertas são gerados a partir de datas, horários e recorrências previamente cadastrados. |

---

## 1. Diagnóstico

**Classificação: Não trabalhado.**

O LembraMed não executa diagnóstico médico ou clínico. Ele não analisa sintomas, exames ou dados do paciente com o objetivo de identificar doenças ou condições de saúde.

Embora o referencial teórico mencione que tecnologias de Saúde Digital podem contribuir para o diagnóstico precoce de doenças, essa possibilidade é apresentada apenas de forma conceitual e **não faz parte das funcionalidades desenvolvidas no sistema**.

**Conclusão:**

> **Diagnóstico: NÃO.**

---

## 2. Monitoramento

**Classificação: Trabalhado.**

O monitoramento é uma das principais funções do LembraMed.

O sistema permite acompanhar:

- os medicamentos cadastrados;
- quais medicamentos devem ser utilizados no dia atual;
- o horário programado para utilização;
- a data de validade;
- o histórico de uso;
- a data e a hora em que o medicamento foi registrado como utilizado.

Dessa forma, o sistema mantém um acompanhamento contínuo da rotina de medicamentos cadastrada pelo usuário.

**Conclusão:**

> **Monitoramento: SIM.**

---

## 3. Recomendação

**Classificação: Trabalhada de forma simples e baseada em regras.**

O sistema envia alertas e lembretes informando ao usuário que chegou o horário de utilizar determinado medicamento previamente cadastrado.

As mensagens podem conter informações como:

- nome do medicamento;
- horário de utilização;
- dosagem cadastrada;
- pessoa para quem o medicamento é destinado;
- informação sobre a validade do medicamento.

Entretanto, o sistema **não escolhe medicamentos**, **não prescreve tratamentos** e **não realiza recomendação clínica**.

Portanto, a recomendação existente no trabalho deve ser entendida como uma **orientação operacional baseada em dados previamente cadastrados**, e não como recomendação médica automatizada.

**Conclusão:**

> **Recomendação: SIM, baseada em regras.**

---

## 4. Predição ou previsão

**Classificação: Não trabalhada.**

O LembraMed não utiliza:

- Inteligência Artificial;
- Machine Learning;
- modelos estatísticos;
- algoritmos preditivos;
- séries temporais;
- técnicas de previsão.

Os avisos futuros do sistema são produzidos com base em **horários, datas e recorrências cadastrados previamente pelo próprio usuário**.

Assim, o sistema sabe que determinado medicamento deverá ser usado em determinado horário porque essa informação já foi cadastrada, e não porque realizou uma previsão.

**Conclusão:**

> **Predição / Previsão: NÃO.**

---

# Classificação final das rotinas

| Rotina | Resultado final |
|---|---|
| **Diagnóstico** | ❌ Não |
| **Monitoramento** | ✅ Sim |
| **Recomendação** | ✅ Sim, baseada em regras |
| **Predição / Previsão** | ❌ Não |

---

## Observação importante sobre a classificação

A rotina de **recomendação** deve ser interpretada com cuidado.

O sistema não realiza recomendação médica propriamente dita. Ele apenas **lembra e orienta o usuário a executar uma ação previamente cadastrada**, como utilizar determinado medicamento em determinado horário.

Por isso, em trabalhos comparativos, a classificação mais precisa é:

**Recomendação: Sim, baseada em regras e sem decisão clínica automatizada.**

---
