# Projeto CI-CD Utilizando o Google Cloud Build e Terraform

Os arquivos base para o projeto foram obtidos do seguinte [repositório](https://github.com/digitalinnovationone/terraform-gcp)

Passos para a configuração do GCP:

1. Criação do bucket para possibilitar a persistência do estado do Terraform no Cloud Storage
![Cloud Storage Bucket](./images/bucket.png)
2. Configurou-se um trigger para automatizar o acionamento do pipeline
![Configuração do Trigger parte 1](images/trigger1.png)
3. Adicionou-se um novo repositório ao Cloud Build
![Sincronização do repositório parte 1](images/new-repo1.png)
![Sincronização do repositório parte 2](images/new-repo2.png)
![Sincronização do repositório parte 3](images/new-repo3.png)
4. Finalizou-se a configuração do trigger
![Configuração do Trigger parte 2](images/trigger2.png)
Após essas configurações aplicadas, basta realizar um push em qualquer branch do repositório selecionado e o Cloud Build inicia o pipeline de deploy da aplicação
