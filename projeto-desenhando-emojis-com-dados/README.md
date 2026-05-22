# 🎨 Desenhando Emojis e Manipulação de Dados em Python

## 📝 Descrição do Projeto
Este repositório contém um conjunto de scripts em Python focados na manipulação de estruturas de dados complexas e aninhadas (dicionários, listas e tuplas). O objetivo principal é demonstrar o domínio de **estruturas de repetição em múltiplos níveis (loops aninhados)** e a aplicação de métodos nativos do Python para ler, transformar e reestruturar dados estruturados.

Desenvolvido originalmente no ambiente Google Colab, o projeto aborda três cenários práticos do mundo real:
1. **Processamento de Imagens Vetoriais (Matrizes):** Modificação de canais de cores RGB em uma grade de pixels para aplicar um efeito de sombreamento (redução de luminosidade) em um emoji.
2. **Engenharia de Dados Musicais:** Inversão de matrizes de frequências sonoras e mapeamento reverso de metadados emocionais em uma biblioteca musical.
3. **Sistemas de Informação de Receitas:** Navegação profunda e formatação de dados textuais e numéricos complexos, utilizando métodos avançados de listas (`.insert()`, `.append()`, `.pop()`).

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.10+
* **Conceitos de Core Python:** Dicionários aninhados, Matrizes (Listas bidimensionais), Tuplas imutáveis, Loops Aninhados (`for`), Condicionais (`if/elif/else`).
* **Ferramentas:** Google Colab / Jupyter Notebook

## 🗂️ Estrutura do Projeto e Resultados

O projeto é dividido em três scripts independentes, cada um cobrindo um nível de manipulação de dados:

### 1. Processamento de Matriz de Pixels (`desenhando_emojis_com_dados-1.py`)
Itera sobre uma matriz $5 \times 5$ que representa a imagem de um emoji. O algoritmo identifica os pixels amarelos `(255, 255, 0)` e reduz a sua luminosidade pela metade (`// 2`), criando um efeito de sombreamento na imagem sem alterar as cores dos olhos e da boca.

### 2. Inversão de Matriz e Sentimentos (`desenhando_emojis_com_dados-2.py`)
Acessa uma estrutura de dados de áudio, inverte a ordem das frequências musicais utilizando a função `reversed()` e realiza uma troca lógica de rótulos (o som mapeado como "Alegre" passa a ser "Triste" e vice-versa).

### 3. Gerenciador Avançado de Receitas (`desenhando_emojis_com_dados-3.py`)
Apresenta uma navegação em 3 níveis de profundidade para renderizar ingredientes e passos de preparo formatados. Demonstra o uso prático de métodos dinâmicos de listas:
* `keys()` e `items()` para desestruturação de dicionários.
* `insert()` para adicionar elementos em posições específicas da lista de ingredientes.
* `append()` e `pop()` para controle de fluxo de passos.

## 🔧 Como Executar

### Pré-requisitos
Certifique-se de ter o Python 3.10 ou superior instalado em sua máquina. Não há necessidade de instalar bibliotecas externas (como Pandas ou NumPy), pois o projeto utiliza exclusivamente a biblioteca padrão do Python.

### Passo a Passo

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/desenhando-emojis-com-dados.git](https://github.com/seu-usuario/desenhando-emojis-com-dados.git)
   cd desenhando-emojis-com-dados

 2. **Execute os scripts desejados:**
   * Para testar o processador de pixels/emoji:
     ```bash
     python desenhando_emojis_com_dados-1.py
     
     ```
   * Para testar o inversor de biblioteca musical:
     ```bash
     python desenhando_emojis_com_dados-2.py
     
     ```
   * Para visualizar o livro de receitas estruturado:
     ```bash
     python desenhando_emojis_com_dados-3.py.

---
[Voltar ao perfil](https://github.com/WillV-Code)
