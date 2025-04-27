# ✨ Sistema de Agendamento para Salão de Beleza

Esse desafio tem como objetivo permitir aos clientes agendar serviços de beleza, escolhendo o tipo de serviço, dia e horário, além de calcular um orçamento baseado na recorrência dos atendimentos ao longo do ano.

## 🚀 Funcionalidades

- Seleção do serviço desejado: **Manicure, Barba ou Cabelo**.
- Escolha do dia e horário de atendimento.
- Validação para garantir que todos os campos estejam preenchidos corretamente.
- Verificação de disponibilidade dos serviços com base no horário de funcionamento.
- Cálculo do orçamento anual considerando recorrência e promoções do dia.
- Fidelidade: Aplicação de gratuidade em atendimentos conforme a frequência.

## 📌 Como Utilizar

1. Escolha o serviço desejado.
2. Selecione o dia e horário disponíveis.
3. Insira a quantidade de atendimentos planejados no ano.
4. Clique no botão **Realizar Orçamento**.
5. O sistema calculará os valores, aplicará descontos e exibirá um resumo com os custos totais.

## 🛠️ Regras do Agendamento

### **Horário de Atendimento**
| Serviço    | Horário de Funcionamento |
|------------|-------------------------|
| Manicure   | 08:00h - 16:00h          |
| Barba      | 13:00h - 20:00h          |
| Cabelo     | 00:00h - 23:00h          |

### **Promoções**
| Serviço    | Dias com Desconto | Valor do Desconto |
|------------|------------------|------------------|
| Manicure   | Terça e Quinta    | R$ 4,00         |
| Barba      | Segunda e Quarta  | R$ 3,00         |
| Cabelo     | Sexta a Domingo   | R$ 5,00         |

### **Fidelidade**
- **A cada X atendimentos**, um será gratuito:
  - Manicure: **A cada 3** atendimentos.
  - Barba: **A cada 4** atendimentos.
  - Cabelo: **A cada 6** atendimentos.

## 💻 Tecnologias Utilizadas

- HTML5
- JavaScript
- CSS3 (pode ser incorporado para estilização)

## 📜 Exemplo de Saída

| Atendimento | Serviço   | Dia       | Hora  | Preço Original | Desconto | Preço Final |
|------------|----------|----------|------|---------------|----------|------------|
| 1          | Cabelo   | Sábado   | 15h  | R$ 30,00      | R$ 5,00  | R$ 25,00    |
| 2          | Cabelo   | Domingo  | 14h  | R$ 30,00      | R$ 5,00  | R$ 25,00    |
| 3          | Cabelo   | Sexta    | 18h  | R$ 30,00      | R$ 5,00  | R$ 25,00    |
| 4          | Cabelo   | Segunda  | 10h  | R$ 30,00      | R$ 0,00  | R$ 30,00    |
| 6 (Fidel.) | Cabelo   | Terça    | 11h  | **Grátis**    | -        | **R$ 0,00** |
| **Total**  | -        | -        | -    | **R$ 150,00** | **R$ 20,00** | **R$ 130,00** |

