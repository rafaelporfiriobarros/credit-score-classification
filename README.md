<img src="images/dataset-cover.jpg">

# Credit Score Classification
## Sobre o conjunto de dados

- ID: um identificador para cada registro no conjunto de dados.
- Customer_ID: Identificador para clientes individuais.
- Month: O mês associado à entrada de dados.
- Name: Nome do cliente.
- Age: Idade do cliente.
- SSN: Número de Segurança Social ou alguma outra forma de identificação.
- Occupation: Ocupação ou cargo do cliente.
- Annual_Income: Renda anual do cliente.
- Monthly_Inhand_Salary: A quantia em dinheiro que o cliente recebe como salário mensalmente.
- Num_Bank_Accounts: Número de contas bancárias que o cliente possui.
- Num_Credit_Card: Número de cartões de crédito que o cliente possui.
- Interest_Rate: A taxa de juros associada a algum aspecto financeiro (por exemplo, empréstimos ou cartões de crédito).
- Num_of_Loan: Número de empréstimos que o cliente possui.
- Type_of_Loan: O tipo de empréstimo(s) que o cliente possui (por exemplo, hipoteca, empréstimo pessoal, etc.).
- Delay_from_due_date: Atraso nos pagamentos a partir da data de vencimento.
- Num_of_Delayed_Payment: Número de pagamentos atrasados.
- Changed_Credit_Limit: Indica se o cliente alterou seu limite de crédito.
- Num_Credit_Inquiries: Quantidade de consultas de crédito realizadas pelo cliente.
- Credit_Mix: A combinação de diferentes tipos de contas de crédito (por exemplo, cartões de crédito, empréstimos).
- Outstanding_Debt: O valor da dívida pendente.
- Credit_Utilization_Ratio: A relação entre o crédito utilizado e o limite de crédito total.
- Credit_History_Age: A idade do histórico de crédito do cliente.
- Payment_of_Min_Amount: Comportamento de pagamento em relação aos pagamentos mínimos exigidos.
- Total_EMI_per_month: Total de pagamentos da Parcela Mensal Equacionada (EMI) feitos pelo cliente.
- Amount_invested_monthly: O valor que o cliente investe mensalmente.
- Payment_Behaviour: Comportamento relacionado a pagamentos, possivelmente indicando padrões ou tendências.
- Monthly_Balance: Saldo mensal do cliente em suas contas financeiras.
- Credit_Score: A pontuação de crédito associada à qualidade de crédito do cliente.

### Declaração do problema
Você está trabalhando como cientista de dados em uma empresa financeira global. Ao longo dos anos, a empresa coletou dados bancários básicos e muitas informações relacionadas ao crédito. A gestão quer construir um sistema inteligente para segregar as pessoas em faixas de pontuação de crédito para reduzir os esforços manuais.
### Tarefa
Dadas as informações relacionadas ao crédito de uma pessoa, construir um modelo de aprendizado de máquina que possa classificar a pontuação de crédito.

### Relatório EDA Inicial

#### Relatório Análise Univariada Variáveis Categóricas

- Mês de Abril foi o Mês com mais frequência.
- Lawyer, Architect, Engineer e Scientist são as Profissões com mais frequência.
- Standard é o nível com mais frequência em Mix de Crédito.
- (Pagamentos baixos com gastos de valor pequeno), 
  (Pagamentos baixos com gastos de valor médio) e 
  (Pagamentos altos com gastos de valor médio) 
  foram os níveis mais frequentes em Comportamento do Pagamento.
- Em Pontuação de Crédito o nível Standard é o mais frequente, seguido do nível Poor.
  
#### Relatório Análise Univariada Variáveis Numéricas

- 37760.22 é a renda anual mais frequente.
- 3102.840000 é o salário mensal mais frequente.
- 6 é o número de contas bancárias mais frequente.
- 5 é o número de cartões de crédito mais frequente.
- 5 é a taxa de juro mais frequente.
- 3 é o número de empréstimos mais frequente.
- 15 é o número de atraso na data de vencimento mais frequente.
- 14 é o número de atrasos de pagamento mais frequente.
- 9.41 é o número de limite de crédito mais frequente.
- 4 é o número de consultas de crédito mais frequente.
- 11517 é o número de dívidaa a pagar mais frequente.
- 31.944960 é o número da taxa de utilização de crédito mais frequente.
- 18 é o número de tempo do histórico de crédito mais frequente.
- 1 é o número de pagamento do valor mínimo mais frequente.
- 0 é o número do total por mês de parcelas mensais fáceis - emi mais frequente.
- 129.479346 é o número do valor investido mensalmente mais frequente.
- 336.792169 é o número do valor do saldo mensal mais frequente.

#### Relatório Análise Bivariada

De um modo geral, a análise bivariada ficou mais significativa com a variáveis quantitativas, assim sendo, essa é a ordem decrescente das relações:

- 1 - salario mensal x saldo mensal - 0.63
- 2 - valor investido mensalmente x salário mensal - 0.54
- 3 - taxa de utilização de crédito x saldo mensal - 0.25
- 4 - taxa de utilização de crédito x salário mensal - 0.16

E na análise bivariada com a relação da variável pontuação de crédito e as demais variáveis, temos que o pagamento do valor mínimo tem a relação mais forte com a pontuação de crédito:

- pontuação de crédito - 1
- pagamento do valor mínimo - 0.13
  
## REFERÊNCIAS DE ESTUDO
> Livro: [Manual de Análise de Dados](https://www.amazon.com.br/Manual-An%C3%A1lise-Dados-Luiz-F%C3%A1vero/dp/8535270876/ref=sr_1_9?__mk_pt_BR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=13X6DL3LVB2F0&keywords=estatistica&qid=1700422688&sprefix=estatistica%2Caps%2C177&sr=8-9&ufe=app_do%3Aamzn1.fos.fcd6d665-32ba-4479-9f21-b774e276a678)

> Livro: [Mãos à obra aprendizado de máquina com Scikit-Learn, Keras & TensorFlow: conceitos, ferramentas e técnicas para a construção de sistemas inteligentes](https://www.amazon.com.br/M%C3%A3os-obra-aprendizado-Scikit-Learn-inteligentes/dp/8550815489/ref=sr_1_1?__mk_pt_BR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=3T4UBQGEP8ZTA&keywords=machine+learning&qid=1706301509&sprefix=machine+learnin%2Caps%2C188&sr=8-1)

> Livro: [Credit Scoring: Desenvolvimento, Implantação, Acompanhamento](https://www.amazon.com.br/Credit-Scoring-Desenvolvimento-Implanta%C3%A7%C3%A3o-Acompanhamento/dp/8521205333/ref=sr_1_1_mod_primary_new?__mk_pt_BR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=2LKPI3TW7M7T6&keywords=credit+score&qid=1706301455&sbo=RZvfv%2F%2FHxDF%2BO5021pAnSA%3D%3D&sprefix=credit+scor%2Caps%2C193&sr=8-1)

> Curso: [Asimov](https://asimov.academy/)

> Curso: [Universidade dos Dados](https://hotmart.com/pt-br/marketplace/produtos/clube-de-assinaturas-da-universidade-dos-dados/Y79687647W)
