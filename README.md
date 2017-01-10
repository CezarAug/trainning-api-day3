# PráticaTecnológica@GFT: 

# Treinamento - API - Dia #3: Desenvolvimento e Arquitetura de APIs

## Exercício de Grupo - Desenhar as APIs e arquitetura de um captação de prospect:
Os grupos deverão ser estruturados em no mínimo três pessoas. Por favor, se organizem em grupo e vamos seguir para o trabalho em equipe.


## Requisitos - Captura de Dados
O cliente deseja criar um sistema totalmente automatizado para captar seus clietes por meio de um aplicativo mobile.

Para a captação dos dados do cliente as seguintes informações são necessárias:

- Nome completo
- CPF
- email
- Endereço
- Comprovante de residência (documento digitalizado)
- Comprovante de renda (documento digitalizado)
- Assinatura (documento digitalizado por meio de uma assinatura feita em um canvas com o próprio dedo do cliente na tela do celular)

As telas do aplicativo estão sendo desenhadas para capturar os dados de forma individualizada conforme especificado na lista anterior.

## Requisitos - Avaliação do Cliente
Após os dados do cliente terem sidos capturados, uma nova fase automátizada irá realizar a análise destas informações de forma assíncrona ao término da captura.

Para esta etapa de avaliação segue as verificações que devem ser realizadas:

- Endereço válido versus comprovante de residência
- CPF em blacklist
- Análise de fraude de email

## Requisitos - Disponibilização do acesso do cliente
Se o cliente for válido os seguintes requisitos devem ser realizados:
- Sua acesso deve ser criado e liberado
- Uma notificação com os respectivos direcionamentos de acesso deverá ser enviada via uma notificação para o cliente

## Requisitos - Relatórios / Dashboards
Para acompanhamento e relatórios gerenciais os seguintes requisitos deverão ser realizados:
- Relatório de acompanhamento geral de prospect
- Relatório de andamento específico do andamento de um determinado prospect

## Trabalho em Equipe
As seguintes atividades devem ser realizadas para modelarmos as APIs e desenho da arquitetura deste projeto
- Divida em domínios funcionais as APIs (Bounded Context - DDD)
- Pense no modelo de arquitetura que será aplicado para cada API de cada domínio funcional
- Como estas APIs podem conversar entre si, leve em consideração que para alguns casos a comunicação entre eles pode acontecer de forma assíncrona
- Como podemos enderaçar os erros de cada domínio funcional
- Modele as APIs de cada domínio funcional utilizando a notação RAML

obs. Desenhe o RAML somente das APIs que serão públicas os outros componentes podem ser apresentados com um blueprint da solução de forma simplificada

### Dicas
- Pense nas interface exposição das APIs que não serconsumidas diretamente pelo de uma forma diferente
- Estas APIs de backend poderão ser assíncronas, então pense no modelo arquitetural que poderá ser empregado para este cenário
- Para o repositório dos dados análitics não pense em um repositório único. Pense no melhor modelo que consiga enderaçar os requisitos de negócio e não funcionais (performance)


## Concluindo
Com este trabalho em equipe praticamos os principais conceitos de arquitetura apresentados para modelarmos e construirmos algumas APIs com os requisitos em questão. Para este tipo de trabalho não existe uma única resposta certa e sim as vantagens e desvantagens de cada escolha.


