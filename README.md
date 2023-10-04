![British_Airways](https://logosmarcas.net/wp-content/uploads/2021/02/British-Airways-Logo.png)

### Sobre o problema

A British Airways(BA) é uma companhia aérea do Reino Unido.  Todos os dias, 
milhares de voos da BA chegam e partem do Reino Unido, transportando clientes 
em todo o mundo. Seja para férias, trabalho ou qualquer outro motivo, o processo 
de agendamento, planejamento, embarque, abastecimento, transporte, pouso e 
execução contínua de voos a tempo é uma tarefa enorme, com muitas 
responsabilidades altamente importantes.

Os clientes que reservarem um voo com a British Airways experimentarão muitos 
pontos de interação com a marca BA. Compreender os sentimentos, necessidades e 
feedback de um cliente é crucial para qualquer empresa, incluindo a BA.

Além disso, os clientes estão mais habilitados do que nunca, pois têm acesso a 
uma riqueza de informações na ponta dos dedos. Essa é uma das razões pelas quais 
o ciclo de compras é muito diferente do que costumava ser. Hoje, se você espera 
que um cliente compre seus voos ou férias quando eles entram no aeroporto, você 
já perdeu! Ser reativo nessa situação não é o ideal; as companhias aéreas devem 
ser proativas para adquirir clientes antes de embarcarem em suas férias.

### Questão de Negócio

A primeira tarefa é focada em raspar e coletar feedback do cliente e revisar 
dados de uma fonte de terceiros e analisar esses dados para apresentar quaisquer
insights.

Já a segunda tarefa consiste em usar os dados fornecidos para criar um modelo
preditivo com o intuito de identificar os clientes com uma maior probabilidade 
de comprar um pacote de férias com a British Airways. Além disso, também é de 
interesse dessa área entender quais variáveis mais impactam na probabilidade de 
compra.

Por último, é necessário que os achados sejam resumidos em slides para uma
apresentação para a equipe de negócio.

### Sobre os dados

Os dados incluem:

reviews_data: dados obtidos através de scrapping em um site de
avaliações. Os dados contém informações sobre a avaliação, como título, texto de
avaliação, tipo de viagem, tipo de assento, etc.

customer_booking: dados de compras de passagens, como dia, canal de vendas, 
horário do voo, etc.

### Métricas de avaliação

Para o modelo em questão, a **Log Loss** será métrica de avaliação principal,
pois é uma métrica que penaliza mais os erros de classificação mais graves, e 
como o objetivo é identificar os clientes com maior probabilidade de compra,
erros graves podem ser prejudiciais para o negócio.

### Melhorias

[⌛] Reduzir a Log Loss do modelo.

### Instruções para execução do projeto

Siga os seguintes passos para rodar o projeto localmente:

1. Clone o repositório:
```sh
git clone https://github.com/HenriqueWF/British_Airways
```
2. Crie um ambiente virtual:
```sh
python -m venv venv
```
3. Ative o ambiente virtual de acordo com o seu sistema operacional.

4. Instale as dependências:
```sh
pip install -r requirements.txt
```

### Descrição dos arquivos


### Resultados
