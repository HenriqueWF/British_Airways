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

### Objetivo

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
5. Selecione o notebook de interesse e execute as células.

### Descrição dos arquivos

    - data
    |- processed
    | |- customer_booking_processed.csv  # Arquivo contendo dados processados sobre as compras de passagens 
    |- raw
    | |- customer_booking.csv  # Arquivo contendo dados sobre as compras de passagens
    | |- reviews_data.csv  # Arquivo contendo dados sobre avaliações obtidas através de scrapping
    |
    - images
    |- Arquitetura_Deploy_Modelo_Propensao.png  # Imagem contendo a arquitetura pensada para o deploy do modelo
    |- Plano_Acao.png  # Plano de ação para o uso dos scores gerados pelo modelo
    |
    - models
    |- calibrador_final.pkl  # Calibrador para ser usado em conjunto com o modelo final
    |- modelo_final.pkl  # Modelo final
    |
    - notebooks
    |- booking_modelling.ipynb  # Notebook contendo a etapa de modelagem dos dados e dos experimentos
    |- EDA_British_Airways.ipynb  # Notebook contendo a etapa de análise exploratória dos dados
    |- web_scrapping_code.ipynb  # Notebook contendo toda a etapa de scrapping dos dados
    |
    - README.md  # Arquivo contendo informações do projeto
    - requirements.txt # Arquivo contendo as dependências do projeto

### Resultados

Como resultado da primeira tarefa, insights como os seguintes foram obtidos:

- Há passageiros de 71 países diferentes.
- Há 198 modelos de aeronaves.  
- Os passageiros voaram por 1529 rotas diferentes.
- Há 4 tipos diferentes de assentos.
- Há 4 modalidades diferentes de viajantes.

Confira mais insights no notebook ```EDA_British_Airways.ipynb```. Além disso, 
também foi criado um dashboard com o intuito de facilitar a visualização dos
dados. Para acessá-lo, basta clicar [aqui](https://app.powerbi.com/view?r=eyJrIjoiODkxNmRiMTktMjI3MC00MTRiLTkxNjMtNTA3YTZjYjI3NTQ1IiwidCI6ImM5YWFjMGZmLWQ1Y2MtNDRhMi05NjIyLWNkMmVlZmQ5Zjk4MiJ9).

Já para a segunda tarefa, o modelo final obteve uma Log Loss de 0.36, o que
significa que o modelo tem uma boa capacidade de classificar os clientes com
maior probabilidade de compra. Em conjunto com o desenvolvimento do modelo, foi
realizado uma análise inferencial para entender quais variáveis mais impactam na
probabilidade de compra. Os resultados dessa análise foram combinados com os
scores gerados pelo modelo para criar um plano de ação para a equipe de negócio.
<br>
![plano de ação](/images/Plano_Acao.png)