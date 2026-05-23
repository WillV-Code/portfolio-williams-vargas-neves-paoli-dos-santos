# 🏪 Sistema Automático de Caixa e Decomposição de Troco



[![Status](https://img.shields.io/badge/status-conclu%C3%ADdo-brightgreen.svg)]()



## 📖 Sobre o Projeto

Este projeto consiste em um **Sistema de Validação de Pagamentos e Cálculo de Troco Otimizado**. O objetivo principal é simular o funcionamento de um terminal de caixa de autoatendimento ou PDV (Ponto de Venda), processando o valor total de uma compra, validando se o valor pago é suficiente e, caso haja troco, calculando a menor quantidade possível de cédulas necessárias para o cliente.



A solução foi projetada de forma modular e estruturada através de **Pseudocódigo (Portugal/Algoritmos)** e mapeada via **Fluxogramas**, aplicando as melhores práticas de divisão de responsabilidades, reutilização de código e estruturação lógica (funções e módulos).



## 🚀 Funcionalidades

- **Validação de Pagamento:** Verifica de forma segura se o valor fornecido pelo cliente (`V_PAG`) é maior ou igual ao valor total da compra (`V_TOT`).

- **Cálculo de Diferença (Troco):** Determina com precisão o valor exato a ser devolvido ao comprador.

- **Decomposição Otimizada de Cédulas:** Algoritmo guloso que reduz o valor do troco dividindo-o pelas maiores denominações de notas disponíveis no sistema financeiro simulado (**R$ 100, R$ 50, R$ 10, R$ 5 e R$ 1**), minimizando o volume de cédulas entregues.

- **Tratamento de Exceções Lógicas:** Caso o pagamento seja insuficiente, o fluxo interrompe a operação imediatamente e exibe uma mensagem amigável de erro.



## 🛠️ Tecnologias e Conceitos Aplicados

O projeto foi modelado utilizando técnicas fundamentais de engenharia de software e lógica de programação estruturada:



- **Modularização (Funções com Retorno Multiplo):** Separação clara entre a captura de dados, validação de regras de negócio e cálculos matemáticos.

- **Estruturas de Decisão (`SE / ENTAO / SENAO`):** Controle de fluxo condicional para direcionar o comportamento do sistema com base na validade do pagamento.

- **Operadores de Divisão Inteira (`/`) e Resto (`%`):** Utilizados na função `CALC_RESTRITO_NOTA` para extrair a quantidade exata de notas de cada valor e atualizar o saldo remanescente do troco de forma iterativa.



## 📐 Estrutura Modular (Arquitetura de Funções)



O sistema é composto por 4 sub-rotinas principais que dividem o trabalho:



1. **`VALIDAR_PAGAMENTO(V_PAG, V_TOT)`**:

   - Retorna `VERDADEIRO` se `V_PAG >= V_TOT`.

   - Retorna `FALSO` caso contrário.

2. **`CALCULAR_TROCO(V_PAG, V_TOT)`**:

   - Retorna a diferença aritmética simples: `V_PAG - V_TOT`.

3. **`CALC_NOTA(TROCO, NOTA)`**:

   - Calcula a quantidade (`QNT`) da nota atual via divisão inteira (`TROCO / NOTA`).

   - Atualiza o `TROCO` restante usando a operação de módulo (`TROCO % NOTA`).

   - Retorna ambos os valores atualizados.

4. **`DECOMPOR_NOTAS(TROCO)`**:

   - Orquestra chamadas sucessivas à função `CALC_NOTA` para as denominações de 100, 50, 10, 5 e 1.

   - Retorna as quantidades de cada nota (`Q100, Q50, Q10, Q5, Q1`).



## ⚙️ Como Executar



### ✅ Pré-requisitos

- Um interpretador de pseudocódigo (como o VisuAlg) ou qualquer ambiente/linguagem de programação moderna (Python, C, JavaScript) traduzindo a lógica apresentada.



### ▶️ Algoritmo Principal (Pseudocódigo)



```pascal

INICIO

    LER V_TOT

    LER V_PAG

    

    VALIDO <- VALIDAR_PAGAMENTO(V_PAG, V_TOT)

    

    SE VALIDO = VERDADEIRO ENTAO

        TROCO <- CALCULAR_TROCO(V_PAG, V_TOT)

        (Q100, Q50, Q10, Q5, Q1) <- DECOMPOR_NOTAS(TROCO)

        

        MOSTRAR "TROCO: ", TROCO

        MOSTRAR "NOTAS: "

        MOSTRAR Q100, " NOTA(S) DE 100"

        MOSTRAR Q50, " NOTA(S) DE 50"

        MOSTRAR Q10, " NOTA(S) DE 10".

        MOSTRAR Q5, " NOTA(S) DE 5"

        MOSTRAR Q1, " NOTA(S) DE 1"

    SENAO

        MOSTRAR "VALOR PAGO INSUFICIENTE"

    FIM_SE

FIM

📊 Exemplo de Saída no Terminal

Cenário 1: Pagamento Válido com Troco Complexo

Valor Total (V_TOT): R$ 133,00

Valor Pago (V_PAG): R$ 300,00




TROCO: 167.00

NOTAS:

1 NOTA(S) DE 100

1 NOTA(S) DE 50

1 NOTA(S) DE 10

1 NOTA(S) DE 5

2 NOTA(S) DE 1

Cenário 2: Erro de Entrada

Valor Total (V_TOT): R$ 50,00

Valor Pago (V_PAG): R$ 45,00



VALOR PAGO INSUFICIENTE

```
## 👤 Autor

Williams Vargas Neves Paoli dos Santos • LinkedIn: <https://www.linkedin.com/in/williams-paoli-98315b407>

E-mail: williamspaoli1@gmail.com

Projeto acadêmico focado em lógica de programação estruturada, modularização e design de algoritmos via fluxogramas.
