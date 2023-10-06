# technical_test

Resolução de problema de [Churn](https://docs.google.com/spreadsheets/d/1hyNndE4QVhjVLmB37ePBURRUkBlFUMJ3g6wlH2UenJY/edit#gid=516785925)


## Processamento

O processamento dos dados e dos modelos são feito no Jupyter Notebook _notebooks/data_prep.ipynb_, _notebooks/single_model.ipynb_ e _notebooks/check_predictions.ipynb_
enquanto a análise inicial dos dados é dado no notebook _analise-inicial-das-features.ipynb_

## Sobre o ambiente: 

**Linguagem**

Python = 3.11.5


**Gerenciamento de dependências:**

- **(Ao clonar o projeto)** Criar o ambiente, caso ele não exista:


    $ cd <path_env>

    $ python3 -m venv <env_name>

ou

    $ python -m venv <env_name>

Se a chamada 'python' refere-se a versão 3.

- **(Ao fazer um pull)** Atualizar o ambiente com as dependências caso ele já exista:

Isso pode ser feito com pip ativando o ambiente:

    $ source <path_env>/<env_name>/bin/activate
    $ pip install -r requirements.txt
    $ deactivate

Ou chamando o pip pelo diretório do ambiente

    $  <path_env>/<env_name>/bin/pip install -r requirements.txt


- **(Antes do push)** Atualizar o arquivo de dependências do ambiente:

Isso pode ser feito com pip ativando o ambiente:

    $ source <path_env>/<env_name>/bin/activate
    $ pip freeze > requirements.txt
    $ deactivate

Ou chamando o pip pelo diretório do ambiente

    $ <path_env>/<env_name>/bin/pip freeze > requirements.txt


- Ativação: 


        $ source <path_env>/<env_name>/bin/activate


- Desativação do ambiente:


        $ deactivate




## Organização do projeto

    
    ├── README.md          	    	    <- Apresentação do projeto.
    ├── datasets
    │   ├── dataset_A3Data_train            <- Dados de treino para modelagem.
    │   ├── dataset_A3Data_validation       <- Dados de validação.
    │   └── full_data                       <- Base processada completa.
    │
    ├── notebooks                           <- Jupyter notebooks.
    │	├── data_prep        		    <- Preparação dos dados.
    │   ├── single_model   		    <- Treinamento do modelo.
    │   ├── check_predictions               <- Checagem das métricas. 
    │   └── churn.pkl                       <- Modelo de churn.
    │
    ├── requirements.txt   		    <- Dependências do ambiente de desenvolvimento.
    │                 
    │
    └── analise-inicial-das-features.ipynb  <- Notebook da análise exploratória inicial                               
            
 

--------

