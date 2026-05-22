# 💰 Sistema de Auditoria e Segurança de Vendas

## 📝 Descrição do Projeto
Este projeto é um script interativo em Python desenvolvido para auditoria, monitoramento e validação de dados de vendas. O sistema atua na garantia da integridade financeira, calculando médias de transações, disparando alertas de quarentena automatizados e identificando *outliers* (discrepâncias estatísticas) que demandam revisão manual. 

Além disso, o script oferece uma interface via terminal para que o auditor possa gerenciar e redefinir dinamicamente os parâmetros de segurança do sistema durante a execução.

---

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.x
* **Ambientes de Execução:** Google Colab, PyCharm ou qualquer terminal compatível com Python 3.
* **Paradigma:** Programação Estruturada e Modular.

---

## 📊 Funcionalidades
* **Entrada de Dados Validada:** Coleta interativa de valores para um lote de 3 vendas.
* **Cálculo de Média Global:** Processamento e exibição instantânea da média aritmética das vendas informadas.
* **Mecanismo de Quarentena:** Alerta visual crítico (`SISTEMA EM QUARENTENA`) acionado caso a média das vendas ultrapasse o teto de segurança predefinido.
* **Detecção de Outliers:** Identificação automática de desvios padrão (vendas individuais com valor 5 vezes maior que a média do lote), sugerindo revisão manual.
* **Ajuste de Parâmetros em Tempo Real:** Permite ao operador alterar dinamicamente a variável global de limite de segurança (`limite_seguranca`) caso alguma venda individual atinja o teto estipulado.
* **Inspeção de Tipagem:** Exibição final detalhada dos valores armazenados e seus respectivos tipos de dados na memória.

---

## 🔧 Como Executar

### Pré-requisitos
* Ter o Python 3.x instalado em sua máquina.

### Passo a Passo

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/nome-do-repositorio.git](https://github.com/seu-usuario/nome-do-repositorio.git)

 2. **Navegue até o diretório do projeto:**
   ```bash
   cd projeto-algoritmo-de-auditoria-de-dados
   
   ```
 3. **Execute o script:**
   ```bash
   python auditoria-de-dados.py
   
   ```
> 💡 **Nota de Compatibilidade:** O script também pode ser importado e executado perfeitamente em ambientes de notebook como o **Google Colab** ou **Jupyter Notebook**, bastando colar o código em uma célula de execução.
> 
## 🛠️ Estrutura do Código
 * limite_seguranca: Variável de controle global inicializada em 10000.
 * analisar_vendas(): Função principal responsável pela lógica de negócio, cálculo de métricas e interface de decisão de alteração de limites.
 * vendas: Lista dinâmica utilizada para o armazenamento e persistência dos dados coletados..

---
[Voltar ao perfil](https://github.com/WillV-Code)
