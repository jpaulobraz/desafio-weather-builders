<div align="center">
  <img src="https://media.giphy.com/media/dWesBcTLavkZuG35MI/giphy.gif" width="600" height="300"/>
</div>

---

# Desafio Weather App

Desafio consiste em testar um aplicação de previsão do tempo chamada SoWe. Ela obtem a localização do usuário e retorna o endereço e dados climáticos da região.

## Considerações

- Protótipo apresentado não descreve funcionalidades após cadastramento do usuário. Sendo assim seria preciso mais informações para validar corretamente a última tela do sistema.
- Não foi informado nessa versão as funcionalidades de login do sistema.

## :pushpin: Requisitos

- Obter localização do usuário
- Cadastro via SMS
- Retorno de dados climáticos de acordo com a localização do usuário


## :wrench: Stack utilizada

**Escrita:** https://app.qase.io/

**Execução:** Android v11


## :shipit:  Técnica de Teste

**Escrita:** Utilizado padrão BDD (Behaviour Driven Development)

**Execução:** Particionamento de Equivalência.

## :earth_americas: Padrão Adotado

**Nomenclatura de Teste:** [Cenário] - [ID teste] - [Nome do teste]

**Nomenclatura de Defeito:** [Tela] - [Descrição]

Testes foram divididos em duas partes:

- Teste de Unidade: Foi testado interface e campos conforme especificação.
- Teste de Sistema: Foi testado a funcionalidade da aplicação conforme regras negociais.


## :bar_chart: Report da Execução

1. Ao abrir o report gerado pela ferramenta qase 
2. Clicar em <Result> para obter informações mais detalhadas

- Teste de Unidade: https://app.qase.io/public/report/eac1d4291bb04ef17e3056b9582687e49dfd1f4a
- Teste de Sistema: https://app.qase.io/public/report/f5a3b8fd678938e79441e22cb666d256e3314617

## :white_check_mark: Sugestão de Melhoria

- Máscara de telefone (XX) XXXXX-XX ao informar telefone na tela de cadastro. Também é preciso ajustar o layout para corresponder ao DDI, para isso seria preciso saber se a aplicação só funcionaria com celulares correspondendo ao DDI brasileiro.
- Só aceitar números na tela de cadastramento do telefone.
- Limitar a quantidade de caracteres no campo [Nome Completo] O sistema aceita um valor mínimo, porém não foi definido um valor máximo para o campo.
- Validar informação no campo [Nome Completo]. Sistema aceita caracteres especiais e isso pode gerar um brecha de segurança na aplicação.
- Não há cadastramento de senha na aplicação, sendo um aplicativo social seria interessante implementar o fluxo de autenticação.
- Implementar fluxo para o usuário informar o clima em sua região. Desta forma o aplicativo poderia, além da API mostrar os dados climáticos, exibir a informação do clima do ponto de vista do usuário. O usuário também poderia verificar o clima com base nas informações das pessoas daquela região.


