# Criando um Modelo de Previsão no Azure Machine Leraning Studio

- Em sua Dashboard no Azure Studio, instale o "Azure Machine Learning".
- Dentro do Azure ML, click na barra a esquerda em "ML automatizado".
- Em ML automatizado, click em " + Novo trabalhode ML automatizado" onde aparecerá os seguintes passos:

1
Método de treinamento

2
Configurações básicas

3
Tipo de tarefa e dados

4
Configurações de tarefas

5
Computação

6
Examinar

## Configurando Trabalho de Treinamento Automático

### Configuraçãoes Básicas

- Defina o "Nome do trabalho", pode ser qualquer nome relacionado ao seu estudo.
- Em "Nome do experimento" marque a opção "Criar novo" e defina um nome de seu agrado.
- Na descrição faça um breve resumo do objetivo de sua aplicação.
- Em "Marcas" não há necessidade de preencher os campos.

## Tipo de tarefa e dados

- Em "Selecionar tipo de tarefa" escolha o tipo de análise que você gostaria de fazer. Nesse projeto utilizaremos a "Regressão", que devolve valores númericos.
- Em 'Secionar os dados" click no botão | + Criar | na qual abrirá uma nova janela para a inserção dos dados.
- Criado o banco, selecione-o e click em avançar. Caso tenha dúvidas, veja o tópico abaixo.

#### Criar ativo de dados

- Em "Tipo de Dados" defina o "Nome", uma breve descrição do tipo de dado em "Descrição"e o tipo do dado em "Tipo". Utilizaremos "Tabular" para esse último.
- Selecione a origem dos dados, pode ser um arquivo no seu computador, um link ou até mesmo usar dados da própria Microsoft em "Azure Open Datasets".
- Após tudo configurado, click em "Criar".

## Configurações de tarefa

- Nas configurações de tarefa, começamos configurando para qual tabela vamos inserir os dados de resposta dentro do banco criado anteriormente em "Coluna de destino".
- Depois configuramos os limites:

#### Máximo de avaliações

3

#### Máximo de avaliaçõessimultâneas

3

#### Máximo de nós

3

#### Limite de pontuação da métrica

0.085

#### Tempo limite do experimento (minutos)

15

#### Tempo limite de iterações (minutos)

15

#### Habilitar encerramento antecipado

Marcado

- Em "Validar teste" altera apenas o campo "Tipo devalidação" para "Divisão de validação de treinamento".

## Computação

- Nesse campo não precisamos alterar nada ao menos que queira maior poder de processamento. Sendo assim, pode utilizar a documentação da Azure ou ver as opções de máquina já pré configuradas no campo "Tamanho da máquina virtual".
- Em seguida click em "Avançar".

## Examinar

- Click em "Enviar trabalho de treinamento".
- Na janela seguinte, no campo "Propriedades", pode ser que seu "Status" demore para sair de "Não ativo". Aguarde alguns instantes que logo ele alternará para "Em execução".

## Encerramento

- Ao concluir os testes você pode baixar o arquivo "JSON bruto" e consultar os "Modelos" na aba lateral esquerda, para ver gráficos e outros modelos.
