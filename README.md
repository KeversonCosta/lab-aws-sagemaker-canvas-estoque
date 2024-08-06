# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Bem-vindo ao desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas. Neste Lab DIO, você aprenderá a usar o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML). Siga os passos abaixo para completar o desafio!

## 📋 Pré-requisitos

Antes de começar, certifique-se de ter uma conta na AWS. Se precisar de ajuda para criar sua conta, confira nosso repositório [AWS Cloud Quickstart](https://github.com/digitalinnovationone/aws-cloud-quickstart).


## 🎯 Objetivos Deste Desafio de Projeto (Lab)




## 🚀 Passo a Passo
1. Selecionar Dataset

    O dataset utilizado foi disponibilizado neste projeto, na seção de datasets.
    Possuindo exatas 1.001 rows e pouco mais de 5.000 células, se trata de um dataset até que robusto. print dataset
   ![351154774-c4ed8b6d-887b-4ef2-9482-3113d38c5b5e](https://github.com/user-attachments/assets/3b7b13ce-2956-4a2c-b1f1-b883d8249982)

2. Construir/Treinar
Ao importar o dataset, devemos escolher a QUANTIDADE_ESTOQUE como target e a tabela ID_PRODUTO como item id.
Não fiz muitas alterações nas configurações, apenas adicionei a use schedule holliday.
![351158213-fa6f0105-eb81-4de4-9ee0-4475743be1bd](https://github.com/user-attachments/assets/3c3ee655-27ca-49d1-968b-2e85b760c80d)

3. Analisar
Com tudo já configurado, utilizei o método Quick build para realizar a análise.
Considero que as métricas de Avg.wQL, WAPE, MAPE, RMSE e WASE bem satistfatórias. 
![351159136-e2021304-bc7b-4083-a27f-ecd5cd306e38](https://github.com/user-attachments/assets/c24dc8a8-d1f9-4db9-a0f3-a802258ccf47)
Outro ponto de vista: PRECO = 9.14% HOLLIDAY_BR = 2.79% FLAG_PROMOCAO = 0.00% 
![351159171-3c93edb9-8c84-4251-a866-deaffd298d47](https://github.com/user-attachments/assets/7f648a76-7036-4d11-b6c5-966e655be1db)

4. Prever
Aos realizar as predições de maneira singular, podemos encontrar métricas como P10, P50 e P90.
P10 é um indicativo, digamos, "pessimista".
P50 seria um indicativo neutro.
Enquanto o P90 é mais otimista e prevê números mais satisfatórios.
![351160134-8d5f3916-b8de-47dd-9bd4-235a3a379609](https://github.com/user-attachments/assets/7e4cbac9-6c7d-4c6d-b901-6f6ceae3b193)



