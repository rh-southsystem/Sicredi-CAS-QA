## Contexto:
Você está em um time ágil. Foi priorizado pelo P.O. a construção de uma API para Consultar CEP’s do Brasil. 
Foi realizado o refinamento, planejamento, desenvolvimento e agora está nas suas mãos construir os testes automatizados.
Sugerimos a utilização de linguagem Java + Maven. Framework que você irá utilizar e a estrutura do código são de livre escolha. 
O importante é que você nos mostre a linha de raciocínio e o porquê das escolhas que você fez. 

### Forma de entrega
- Crie um repositório privado no GitLab com o nome prova_sicredi_api 
- Efetue os commits de seu projeto neste repositório
- Não adicione ao repositório a pasta de projeto que sua IDE de desenvolvimento gera de forma automática
- Adicione os seguintes usuários ao repositório privado:
- No GitLab: sicredi_user  (como “developer”)
- Informe o nome do repositório na resposta do e-mail
- Adicione qualquer outra informação que você julgue relevante no e-mail ou em um arquivo readme.md

Agora é a hora da verdade! Queremos ver você mandar bem nos testes automatizados. 
Nesse desafio, os objetivos são desenvolver testes baseados nos cenários abaixo, utilizando o serviço que está no link:
URL: https://viacep.com.br/ws/91060900/json/ 
Cenário: Consulta CEP valido
Dado que o usuário inseriu um CEP válido
Quando o serviço é consultado
Então é retornado o CEP, logradouro, complemento, bairro, localidade, uf e ibge.

Cenário 1: Consulta CEP inexistente
Dado que o usuário inseri um CEP que não exista na base dos Correios
Quando o serviço é consultado 
Então é retornada um atributo erro

Cenário 2: Consulta CEP com formato inválido 
Dado que o usuário inseri um CEP com formato inválido
Quando o serviço é consultado 
Então é retornado uma mensagem de erro

Extras:
1) Criar um cenário que verifique o retorno do serviço abaixo:
URL: https://viacep.com.br/ws/RS/Gravatai/Barroso/json/
