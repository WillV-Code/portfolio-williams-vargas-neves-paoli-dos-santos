# 🏢 Auditoria de Orçamentos Corporativos (Python)
 
[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/)
[![Status](https://img.shields.io/badge/status-concluído-brightgreen.svg)]()
 
## 📖 Sobre o Projeto
Este projeto consiste em um **Sistema de Auditoria de Recursos Corporativos** desenvolvido em Python. O objetivo principal é simular o ambiente financeiro de uma empresa multinacional, processando e calculando o orçamento total consolidado a partir de uma estrutura organizacional complexa e altamente aninhada (Matriz e Filiais).

A solução foi projetada utilizando conceitos avançados do ecossistema Python para garantir **modularidade**, **rastreabilidade** e **separação de responsabilidades**, simulando boas práticas amplamente adotadas em sistemas backend de auditoria e governança corporativa.
 
## 🚀 Funcionalidades
- **Cálculo Hierárquico Recursivo:** Varredura profunda na árvore de dados da empresa para consolidação dos orçamentos, independentemente do nível de aninhamento dos subdepartamentos.
- **Filtros Dinâmicos de Escopo (`*args`):** Permite ignorar departamentos inteiros (e todas as suas ramificações) de forma dinâmica durante o cálculo.
- **Conversão de Câmbio em Tempo de Execução (`**kwargs`):** Suporte nativo para aplicação de taxas de câmbio e definição de moedas de destino (`BRL`, `EUR`, etc.).
- **Log de Auditoria Automatizado (Decorator):** Interceptação da função de cálculo para gerar logs detalhados contendo os parâmetros de entrada, o tempo de execução exato e a assinatura da função.
 
## 🛠️ Tecnologias e Conceitos Aplicados
Este projeto foi construído utilizando exclusivamente a **Biblioteca Padrão do Python (Standard Library)**, explorando os seguintes recursos:

- **Decorators (`@auditor`):** Implementação de um decorador customizado acoplado à função principal. Utiliza `functools.wraps` para preservar os metadados da função original enquanto injeta a lógica de monitoramento e medição de tempo (`time.time()`).

- **Recursão Interna (`dicionario_percorrer`):** Uma função utilitária aninhada que navega pelas estruturas de dicionários (`isinstance(valor, dict)`), acumulando os valores numéricos (`int`, `float`) e aplicando as cláusulas de escape para setores ignorados.

- **Argumentos Variádicos (`*args` e `**kwargs`):** Flexibilidade total na assinatura de `calcular_orcamento`, permitindo passar uma lista indefinida de exclusões e dicionários de configuração econômica de forma limpa.
 
## ⚙️ Como Executar
 
### ✅ Pré-requisitos
- Python **3.8 ou superior** instalado.
 
### ▶️ Passo a Passo
1. Clone este repositório:
   ```bash
   git clone [https://github.com/WillV-Code/portfolio-williams-vargas-neves-paoli-dos-santos.git](https://github.com/WillV-Code/portfolio-williams-vargas-neves-paoli-dos-santos.git)

   ```
2. Acesse a pasta do projeto:
   ```bash
   cd projeto-sistema-de-auditoria-de-recursos-corporativos
   ```
3. Execute o script principal:
   ```bash
   python sistema_auditoria.py
   ```

## 📊 Exemplo de Saída no Terminal
Ao executar o script com a configuração padrão do arquivo (ignorando "RH" e "Jurídico" com taxa de 5.20), a saída gerada será:
--- Ínicio da Auditoria ---
Função chamada: calcular_orcamento
Args (posicionais): ({...}, 'RH', 'Jurídico')
Kwargs (nomeados): {'taxa_cambio': 5.2, 'moeda_destino': 'BRL'}
Moeda de destino: BRL
Taxa de câmbio: 5.2
Tempo de execução: 0.000032 segundos
--- Fim da auditoria ---
ORÇAMENTO TOTAL FINAL: 2,756,000.00

 
## 🧠 Estrutura de Dados do Projeto
​Os dados simulados do ecossistema corporativo possuem a seguinte distribuição geográfica e departamental dentro do script:
​Matriz: Divisões de TI (Infraestrutura, Desenvolvimento, Suporte), RH (Recrutamento, Treinamento, Cultura, Folha), Financeiro e Jurídico.
​Filial_Brasil: Divisões de Comercial, Marketing e Operações.
​Filial_Europa: Divisões de TI e Comercial.

## 👤 Autor
* **Williams Vargas Neves Paoli dos Santos** • **LinkedIn: <https://www.linkedin.com/in/williams-paoli-98315b407>**
* E-mail: williamspaoli1@gmail.com
 
---
*Projeto acadêmico com foco na aplicação prática de conceitos avançados da linguagem Python.*
