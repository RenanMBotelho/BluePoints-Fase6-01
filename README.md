# BluePoints

É um aplicativo de pontos de coleta seletiva. Seu objetivo é ajudar cidadãos a gerenciar e separar corretamente o lixo, indicando o ponto de coleta seletiva mais próximo e fornecendo informações sobre os dias e horários de coleta de resíduos.

## Índice

- Descrição
- Funcionalidades
- Pré-requisitos
- Instalação
- Uso
- Testes

## Descrição

O aplicativo BluePoints, através de seu objetivo de fortalecer uma cidade mais sustentável, permite que o usuário encontre locais apropriados de coleta de materiais, faz o controle dessas reciclagens e ainda oferece pontos ao usuário para que ele possa trocar por benefícios oferecidos pelo aplicativo, fornecidos por empresas parceiras.
Este fonte realiza testes via api das funcionalidades de CRUD do aplicativo.

## Funcionalidades

- Fazer cadastro no aplicativo.
- Fazer login para recebimento do token para teste de api.
- Cadastro de reciclagem também através de api.
- Consulta de registros.
- Alteração de registros.
- Exclusão de registros.

## Pré-requisitos

- Intellij para clonar o código.
- Arquivos de teste de api para o aplicativo.
- Programa Postman ou Insomnia para testes de api com os arquivos.
- Liberação da porta 8080 para o programa rodar via Docker.

## Instalação

Siga os passos abaixo para configurar o ambiente de desenvolvimento:

1. Clone este repositório no ambiente de desenvolvimento (indicado o programa Intellij): https://github.com/RenanMBotelho/BluePoints-Fase3.git
2. Caso não tenha, instale o programa Postman ou Insomnia.
3. Pegue no diretório do programa o json de teste de api e importe no programa instalado.

## Uso

1. Rode o programa e se certifique que não tenha apresentado erro no terminal.
2. Abra o programa Postman ou similar com o json de api já importado.

## Testes

1. Primeiro teste: fazendo login com o usuário predefinido no json, no endpoint "login usuário", para recebimento do token. É possível, caso desejado, fazer o cadastro de um usuário.
2. Segundo teste: com o token recebido, o mesmo deverá ser aplicado em todos os demais testes de CRUD, na opção "Auth", como Bearer Token.
3. Terceiro teste: na opção "incluir reciclagem", com o token já aplicado, pode ser usado o conteúdo do body como exemplo para registro de reciclagem no aplicativo.
4. Quarto teste: na opção "listar reciclagens", é possível obter um get com todos os registros de reciclagem do banco de dados.
5. Quinto teste: na opção de "atualizar reciclagem", é passado o ID que se deseja alterar e as alterações a serem feitas.
6. Sexto teste: por fim, para concluir o CRUD, é possível exluir um registro passando o ID que se deseja deletar no endereço do endpoint.
