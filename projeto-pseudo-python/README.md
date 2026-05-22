# 🐍 PseudoPython: Laboratório de Lógica e Estruturas de Controle

## 📝 Descrição do Projeto
Este projeto reúne um conjunto de quatro scripts utilitários desenvolvidos em Python, com o objetivo de demonstrar a aplicação prática de estruturas condicionais, laços de repetição, manipulação de fluxos e tipagem de dados. Os códigos simulam cenários cotidianos e corporativos, servindo como uma ponte prática entre o pseudocódigo tradicional e a sintaxe Python.

O projeto aborda conceitos fundamentais da linguagem, como o comportamento exclusivo da função `range()` e a necessidade de conversão estática de tipos (`type casting`) ao manipular dados recebidos via terminal (`input()`).

---

## 🛠️ Funcionalidades do Sistema

O repositório está estruturado em quatro módulos principais:

### 1. 🛒 Processador de Vendas (`processar_vendas`)
* **Objetivo:** Simular o fechamento de um carrinho de compras.
* **Regras de Negócio:** Aplica descontos progressivos baseados no valor total:
    * Compras acima de **R$ 500,00**: 10% de desconto.
    * Compras acima de **R$ 200,00**: 5% de desconto.
* **Validação:** Implementa consistência de dados, impedindo o processamento de preços ou quantidades menores ou iguais a zero.

### 2. 🌤️ Analisador de Clima (`analisar_clima`)
* **Objetivo:** Monitorar e consolidar dados de temperatura ao longo de uma semana (7 dias).
* **Métricas:** Calcula a média térmica semanal e contabiliza dias de calor extremo (acima de 35°C).
* **Alertas:** Ativa um sinalizador de segurança caso condições críticas sejam detectadas.

### 3. 🎓 Sistema de Notas de Turma (`sistema_notas_turmas`)
* **Objetivo:** Automatizar o cálculo de médias escolares de uma turma de alunos.
* **Critérios de Aprovação:** * Média $\ge 7.0$: Aprovado.
    * Média entre $5.0$ e $6.9$: Recuperação.
    * Média $< 5.0$: Reprovado.

### 4. 💰 Simulador de Poupança (`simulador_poupanca`)
* **Objetivo:** Projetar a evolução de um investimento com aportes mensais e juros compostos.
* **Destaque:** Monitoramento de metas em tempo real (ex.: alerta ao atingir o montante de R$ 10.000,00).

---

## 🚀 Conceitos e Aprendizados Práticos

A implementação destes scripts permitiu consolidar boas práticas essenciais de desenvolvimento em Python:

* **Tipagem Dinâmica e Casting:** No Python, a tipagem é dinâmica, dispensando a declaração formal de tipos de variáveis. Contudo, como a função `input()` captura dados estritamente como *String*, foi aplicada a conversão explícita utilizando `int()` e `float()` para viabilizar as operações matemáticas.
* **Comportamento do `range()`:** Diferente do pseudocódigo tradicional onde o limite final do laço `PARA` costuma ser inclusivo, no Python o ponto de parada do `range(inicio, fim)` é exclusivo. Para percorrer um intervalo exato (como os meses de uma simulação de 1 a $N$), a sintaxe exige o ajuste fino dos limites (`range(1, meses + 1)`).

---

## 🔧 Como Executar

### Pré-requisitos
* Python 3.8 ou superior instalado.

### Passo a Passo
1. Clone este repositório para a sua máquina local:
   ```bash
   git clone [https://github.com/seu-usuario/pseudopython.git](https://github.com/seu-usuario/pseudopython.git)

 2. Navegue até o diretório do projeto:
   ```bash
   cd pseudopython
   
   ```
 3. Execute o arquivo principal pelo terminal:
   ```bash
   python pseudopython.py
   
   ```
 4. Siga as instruções exibidas na tela para interagir com cada uma das quatro funções do sistema.

[Voltar ao perfil](https://github.com/WillV-Code)
