# 🌍 Engenharia de Contexto e Lógica Física (Python)

[![Python Version](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/)
[![Status](https://img.shields.io/badge/status-concluído-brightgreen.svg)]()

## 📖 Sobre o Projeto
Este repositório reúne um conjunto de algoritmos desenvolvidos em Python focados em **Engenharia de Contexto e Lógica Física**. O objetivo central é traduzir variáveis, restrições e cenários do mundo real em dados estruturados que o computador consiga interpretar de forma exata. 

O projeto é composto por duas soluções principais:
1. **Algoritmo de Microclima Local:** Analisa dados meteorológicos e de qualidade do ar de pontos urbanos específicos, calculando um índice composto de conforto.
2. **Simulador de Saída Eficiente (Evacuação):** Modela um agente inteligente tentando escapar de um ambiente complexo com restrição de energia, lidando com obstáculos como portas trancadas e fechaduras de múltiplas voltas.

> 🧠 **Filosofia do Projeto:** "Problemas grandes ficam menos complexos se os dividimos em pequenas partes. A vida deixa de ser um evento caótico e passa a parecer um projeto que se pode organizar, testar e melhorar a cada dia, um comando por vez.

---

## 🚀 Funcionalidades

### 1. Sistema de Monitoramento de Microclima Urbano
- **Ingestão de Dados Multicontexto:** Processamento de dados climáticos reais extraídos de canais meteorológicos (*Weather Channel*) estruturados por turnos (Manhã e Noite).
- **Mapeamento de Métricas Físicas:** Classificação de Temperatura (Frio, Quente, Muito Quente) e Umidade (Sol, Nublado, Chuvoso, Muito Chuvoso).
- **Análise Avançada da Qualidade do Ar (IQAr):** Uso de estruturas condicionais modernas (`match/case`) para categorizar a qualidade do ar em Boa, Moderada ou Ruim, disparando alertas de saúde críticos para cenários de insalubridade.
- **Métrica de Conforto Urbano:** Algoritmo ponderado que normaliza as pontuações de temperatura, umidade e IQAr para gerar uma nota final de 0 a 10 para a localidade.

### 2. Simulador de Evacuação e Fuga Eficiente
- **Mapeamento de Ambientes Dinâmicos:** Representação espacial de salas, corredores e saídas através de vetores de estado, simulando obstáculos físicos de forma puramente lógica.
- **Gerenciamento de Inventário e Recursos:** O agente coleta itens (como chaves) e consome energia a cada movimento, precisando escapar antes do esgotamento de suas forças.
- **Lógica de Bloqueio Físico por Voltas:** Simulação de fechaduras mecânicas complexas que exigem iterações repetidas (ex: dar 3 ou 4 voltas na chave) para a liberação da rota.

---

## 🛠️ Tecnologias e Conceitos Aplicados
O projeto foi construído utilizando os recursos nativos do Python 3.10+, explorando os seguintes conceitos:
* **Estruturas de Repetição e Condicionais Avançadas:** Uso de laços `while` estruturados para estados de fuga e controle de fluxo com estruturas `match/case` (Pattern Matching).
* **Matrizes e Listas Dinâmicas:** Armazenamento indexado para cruzamento de dados geoespaciais e condições ambientais.
* **Modularização e Abstração:** Funções auxiliares específicas com responsabilidade única para cálculos de scores e conversões de dados.

---

## ⚙️ Como Executar

### Pré-requisitos
* Python 3.10 ou superior instalado (necessário para suporte ao `match/case`).

### Passo a Passo
1. Clone este repositório:
   ```bash
   git clone [https://github.com/WillV-Code/portfolio-williams-vargas-neves-paoli-dos-santos.git](https://github.com/WillV-Code/portfolio-williams-vargas-neves-paoli-dos-santos.git)

 2. Acesse a pasta do projeto:
   ```bash
   cd portfolio-williams-vargas-neves-paoli-dos-santos
   
   ```
 3. Execute o script de análise de Microclima:
   ```bash
   python engenharia-de-contexto-e-logica-fisica-1.py
   
   ```
 4. Execute o script do Simulador de Fuga:
   ```bash
   python engenharia-de-contexto-e-logica-fisica-2.py
   
   ```
> 💡 **Nota de Execução:** Ambos os scripts foram originalmente gerados e validados no ambiente **Google Colab**, sendo 100% compatíveis com Jupyter Notebooks.
> 
## 🧠 Lógica e Visão de Engenharia
Diferente de sistemas puramente abstratos, estes scripts aplicam a lógica computacional rigorosa para resolver a falta de definição de passos do cotidiano.
 * No **Script 1**, o contexto urbano é destrinchado em métricas de bem-estar, onde o computador calcula friamente o que seria um ambiente confortável através de thresholds bem definidos.
 * No **Script 2**, o problema de uma rota de evacuação física é traduzido em dados puros (distância, estados de portas e travas), provando que cenários imprevisíveis podem ser antecipados e mitigados com uma estrutura robusta de *if/else* ("Se o corredor A estiver bloqueado, vá pelo corredor B").
## 👤 Autor
 * **Williams Vargas Neves Paoli dos Santos**
 * GitHub: WillV-Code

*Projeto focado na aplicação prática de lógica física, modelagem de contexto ambiental e estruturação algorítmica de problemas complexos.*
---
[Voltar ao perfil](https://github.com/WillV-Code)
