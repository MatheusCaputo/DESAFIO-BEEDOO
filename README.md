# Desafio | Analista de Qualidade de Software Júnior
## [Beedoo Chalenge](https://complex-night-ddb.notion.site/Desafio-Analista-de-Qualidade-de-Software-J-nior-5cef7366f66b41e890aada4d3f47f36f)
------------------
## Features

#### [1. Cadastrar curso](https://creative-sherbet-a51eac.netlify.app/new-course) ####
#### [2.Listar cursos](https://creative-sherbet-a51eac.netlify.app/) ####

----------------
## Histórias de usuário
**Observações:** como não foram disponibilizadas as especificações do sistema, assumi algumas regras de negócio com base na minha experiência como usuário de sistemas de cursos/educação e como Analista de Qualidade de Sofware que são padrões e lógicas para aplicações de cursos e qualquer aplicação no geral. Além de base adquirida após exploração da aplicação via hipóteses e resultados obtidos. 

Seguem a pré-suposições assumidas:

### US1 - Cadastrar curso ###
**Visão do usuário**

**COMO** usuário
**PRECISO** cadastrar o curso
**PARA** que os alunos possam se matricular

**Regras de negócio**

RN1 - Um curso não pode ser cadastrado sem o preenchimento dos campos obrigatórios (Nome do curso, Data inicio e Data fim, Número de Vagas e Tipo de curso).

RN2 - Os campos Data de início e Data de fim não podem ser preenchidos com datas inválidas.

RN3 - O campo Data de fim não pode ser preenchido com uma data anterior a data preenchida no campo Data de inicio.

RN4 - O campo Número de vagas deve ser do tipo numérico, devendo aceitar somente  valores iguais ou maiores que zero.

RN5 -  Ao clicar no botão Cadastrar curso, o usuário deve permanecer na página Cadastro de curso.

RN6 - Ao clicar no botão Listar cursos o usuário deve ser redirecionado para a página de Lista de cursos. 

#### US2 - Listar cursos ####
**Visão do usuário**

**COMO** usuário 
**PRECISO** visualizar os cursos disponíveis 
**PARA** gerenciar o curso desejado 

**Regras de negócio**

RN1 - Os cursos devem ser exibidos em formato de card.

RN2 - Todos os cursos já criados, não excluidos devem estar listados na tela de Listagens de Cursos.

RN3 - Ao clicar no botão excluir curso, o mesmo deve ser excluído da lista e não mais exibido.

RN4 -  Ao clicar no botão Cadastrar curso, o usuário deve ser redirecionado para a página com o formulário de Cadastro de curso.

RN5 - Ao clicar no botão Listar cursos o usuário deve permanecer na página de Lista de cursos. 

------
## Casos de teste

Para os casos de testes foram utilizadas técnicas como partição de equivalencia, análise de valor limite e testes exploratórios.

Os casos de teste estão documentados em uma planilha do Google Docs dividida em 2 abas em que cada uma representa uma Feature da aplicação, sendo elas Cadastrar curso e Listar cursos.

Os casos de teste refentes a cada Feature estão contidos em suas respectivas abas, com os campos Feature, ID, Título, Caso de teste (Gherkin), Resultado esperado, Passo a passo e resultado obtido.

[Link da planilha com os casos de teste](https://docs.google.com/spreadsheets/d/1sPyE82hJXhuQFf448xETmOKolRHDucMMh2gOeGqi1Hc/edit?usp=sharing)

Já as evidências contidas no diretório de teste estão nomeadas seguindo o ID da planilha acima.

[Diretório com as evidências de teste](https://drive.google.com/drive/folders/14MuXB2FcBTMOaghu0eWn-9Xn5hqvN42F?usp=sharing)

-----------------
## Relatório de Bugs

Para o relatório de bugs foi decidido pela inclusão das seções Título, Gravidade, Caso de teste relacionado, Evidência do erro, Descrição do erro (Passo a passo), O que o erro pode ocasionar (contém também uma sugestão de solução) e Prováveis causas.

Essas seções foram selecionadas com o objetivo de tornar a metodologia utilizada mais clara e reproduzível, complementando a rastreabilidade entre o bug encontrado e o Caso de teste relacionado, além de agregar valor auxiliando na descoberta de prováveis causas, consequências e possíveis soluções desses bugs.

[Relatório de Bugs](https://docs.google.com/document/d/1OCHTlzPRiQ3v3ZYj3LKXxWQFQbWucvuVr4tGiooxuQs/edit?usp=sharing)

-----------------
## Melhorias sugeridas para o módulo de curso do Beedoo
- Os campos obrigatórios devem possuir alguma marcação visual sinalizando-os para o usuário.
- Os campos de data poderiam gerar mensagens em situações de invalidez logo após perderem o foco.
- Os campos de data poderiam ter travas para datas passadas e de ano.
- O campo número de vagas deveria gerar mensagem de invalidez logo após perder o foco.
- A exibição dos campos de Data serem exibidos nos cards da lista no mesmo formato em que são cadastrados, pois eles são cadastrados no formato brasileiro e exibidos no formato americano.
