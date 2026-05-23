# 💰 Sistema de Auditoria e Segurança de Vendas (Python)



[![Python Version](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/)

[![Status](https://img.shields.io/badge/status-concluído-brightgreen.svg)]()

## 📖 Sobre o Projeto

Este projeto consiste em um script interativo desenvolvido em Python voltado para a auditoria, validação e monitoramento de dados financeiros de vendas. O sistema atua na garantia da integridade financeira do negócio através do cálculo de médias transacionais, identificação estatística de *outliers* e disparos automatizados de alertas de segurança.



A solução oferece uma interface em linha de comando (CLI) que permite ao auditor inspecionar a tipagem dos dados em memória e redefinir dinamicamente os parâmetros de tolerância a riscos do sistema em tempo de execução.## 🚀 Funcionalidades- **Entrada de Dados Validada:** Coleta interativa via terminal estruturada para o processamento de lotes de vendas.- **Cálculo de Média Global:** Processamento aritmético instantâneo dos valores informados para consolidação de métricas.- **Mecanismo de Quarentena:** Alerta visual crítico (`SISTEMA EM QUARENTENA`) acionado automaticamente caso a média do lote ultrapasse o teto de segurança operacional.- **Detecção de Outliers:** Varredura algorítmica para identificar vendas individuais que superem em 5 vezes a média do lote, sinalizando a necessidade de revisão manual por discrepância.- **Ajuste Paramétrico Dinâmico:** Flexibilidade para o operador redefinir a variável global de limite de segurança (`limite_seguranca`) em tempo real caso uma transação legítima fure o bloqueio.- **Inspeção de Tipagem:** Exibição analítica final dos valores armazenados na lista e seus respectivos tipos primitivos de dados na memória.## 🛠️ Tecnologias e Conceitos Aplicados

Este projeto foi construído utilizando a biblioteca padrão do Python, com foco nos seguintes conceitos de programação:* **Estruturas de Repetição e Condicionais:** Uso de laços `for` e blocos `if/elif/else` para controle de fluxo, validações e iteração de coleções.* **Manipulação de Escopo (`global`):** Aplicação de modificadores de escopo para permitir que funções modifiquem variáveis globais de controle em tempo de execução.* **Coleções Dinâmicas (Lists):** Armazenamento, persistência temporária e agregação de dados utilizando listas dinâmicas.## ⚙️ Como Executar### Pré-requisitos* Python 3.x instalado.### Passo a Passo1. Clone este repositório:

   ```bash

   git clone [https://github.com/WillV-Code/portfolio-williams-vargas-neves-paoli-dos-santos.git](https://github.com/WillV-Code/portfolio-williams-vargas-neves-paoli-dos-santos.git)
```
Acesse a pasta do projeto:




```
cd projeto-algoritmo-de-auditoria-de-dados
```
Execute o script principal:




```
python auditoria-de-dados.py
```
>💡 Nota de Execução: O script também é 100% compatível com ambientes de notebook como Google Colab ou Jupyter Notebook, bastando copiar e colar o código de auditoria-de-dados.py em uma célula de execução.

🧠 Lógica e Estrutura do Código

O script foi desenhado seguindo o paradigma de programação estruturada e modular. A captura dos dados é isolada inicialmente através de um laço que popula a lista dinâmica vendas. Uma vez consolidado o lote, a função analisar_vendas() assume o controle do fluxo, centralizando a lógica de negócio (cálculo de média e varredura de outliers) e gerenciando a interface de tomada de decisão do auditor.

A persistência do teto de risco é mantida pela variável global limite_seguranca (inicializada em 10000), que pode ser sobrescrita de forma segura de dentro da função principal através do encapsulamento de escopo, garantindo previsibilidade ao script antes da rotina final de inspeção de tipos.

👤 Autor

**Williams Vargas Neves Paoli dos Santos**

GitHub: <https://github.com/WillV-Code>

Projeto focado na automação de processos de auditoria financeira e aplicação prática de lógica de programação.
