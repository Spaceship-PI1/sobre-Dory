<h1 align="center">Dory 🐟</h1>

<div align="center">
  <a href="*"><img title="Dory" src="logo.svg" style="width: 440px;" /></a>
</div>

## :computer: Projeto

Dory é uma aplicação web que tem como objetivo ajudar os alunos de Sistemas e Mídias Digitais, da Universidade Federal do Ceará, a encontrarem um professor orientador para o seu TCC. O projeto foi desenvolvido durante a disciplina de Projeto Integrado I no semestre 2021.2 pela equipe Spaceship, formada por [Larissa Araújo](https://github.com/araujlarissa), [Letícia Torres](https://github.com/leticialimatorres) e [Myguel Angello](https://github.com/myguelangello).

## :pushpin: Requisitos funcionais

<table>
  <tr>
    <td>
      <strong>Código/Funcionalidade</strong>
    </td>
    <td>
      <strong>Descrição</strong>
    </td>
    <td>
      <strong>Codificação</strong>
    </td>
  </tr>
  <tr>
    <td>RF G001 / Cadastrar</td>
    <td>
      O aluno/professor precisa se cadastrar e inserir informações como nome,
      sobrenome, e-mail, senha e tipo de perfil para ter acesso a aplicação.
    </td>
    <td>Diretório (back): src/app/controllers/authController.js. Linha: 18 até 55.
    <br>
    Diretório (front): src/pages/Cadastro.js
    </td>
  </tr>
  
  <tr>
    <td>RF G002 / Autenticar (login)</td>
    <td>
      O aluno/professor precisa colocar o e-mail e a senha que foram cadastrados
      para acessar a aplicação.
    </td>
    <td>Diretório (back): src/app/controllers/authController.js. Linha: 58 até 87
    <br>
    Diretório (front): src/pages/Login.js
    </td>
  </tr>
  
  <tr>
    <td>RF G003 / Esquecer senha</td>
    <td>
      O aluno/professor precisa informar o seu e-mail para ser enviado um token
      de recuperação de senha.
    </td>
    <td>Diretório (back): src/app/controllers/authController.js. Linha: 89 até 160</td>
  </tr>
  
  <tr>
    <td>RF G004 /Resetar senha</td>
    <td>
      O aluno/professor precisa pegar o token de resetar a senha e informar o
      seu email, o token recebido, a nova senha e a confirmação da nova senha no
      respectivo formulário dentro da aplicação.
    </td>
    <td>
      Diretório (back): src/app/controllers/authController.js. Linha: 162 até 211
    </td>
  </tr>
  
  <tr>
    <td>RF G005 / Sair da aplicação</td>
    <td>
      O aluno/professor precisa clicar no dropdown da navbar onde tem a opção “Sair”, ao selecioná-la ele encerra a sessão
    </td>
    <td>Diretório (front): src/components/NavBarGlobal/index.js. Linha: 153 e 159.</td>
  </tr>
  
  <tr>
    <td>RF A001 / Cadastrar foto de perfil</td>
    <td>O aluno precisa fazer o upload de uma foto para colocar no seu perfil</td>
    <td>Diretório (front): src/components/InputImage/index.js.</td>
  </tr>
  
  <tr>
    <td>RF A002 / Cadastrar descrição “Sobre você”</td>
    <td>O aluno precisa informar uma breve descrição sobre ele</td>
    <td>Diretório (back): src/app/controllers/editController.js. Linha: 5 até 31.
    <br>
    Diretório (front):
    src/pages/CadastroAluno.js. Linha 39 a 43
    </td>
  </tr>

  <tr>
    <td>RF A003 / Cadastrar interesses em pesquisa</td>
    <td>
      O aluno precisa informar quais áreas ele tem interesse, por exemplo,
      ilustração, animação, etc
    </td>
    <td>Diretório (back): src/app/controllers/registrationController.js. Linha: 5 até 31.
    <br>
    Diretório (front):
    src/pages/CadastroAluno.js. Linha 45 a 59</td>
    </tr>
  
  <tr>
    <td>RF A004 / Cadastrar tema do TCC</td>
    <td>
      O aluno pode cadastrar o tema do TCC dele, caso ele já tenha definido, ou
      ele pode cadastrar uma lista de possíveis temas, ou simplesmente não
      informar seu tema
    </td>
    <td>Diretório (back): src/app/controllers/registrationController.js. Linha: 5 até 31.
    <br>
    Diretório (front):
    src/pages/CadastroAluno.js. Linha 68 a 80</td>
  </tr>
  
  <tr>
    <td>RF A005 / Cadastrar modalidade do TCC</td>
    <td>
      O aluno precisa escolher uma das 3 modalidades de TCC: artigo científico,
      monografia ou relatório técnico. Mas se ele ainda estiver em dúvida, tem a
      opção de “Não sei ainda”
    </td>
    <td>Diretório (back): src/app/controllers/registrationController.js. Linha: 5 até 31.
    <br>
    Diretório (front):
    src/pages/CadastroAluno.js. Linha 83 a 104</td>
  </tr>
  
  <tr>
    <td>RF A006 / Cadastrar estágio de desenvolvimento do TCC</td>
    <td>
      O aluno precisa dizer o estágio de escrita do TCC dele, se ele começou a
      escrever na disciplina de TCC 1, ou se ele já estava escrevendo por estar
      sendo acompanhado por outro orientador, ou se ele estava escrevendo por
      conta próprio ou se ainda não escreveu nada
    </td>
    <td>Diretório (back): src/app/controllers/registrationController.js. Linha: 5 até 31.
      <br>
      Diretório (front):
      src/pages/CadastroAluno.js. Linha 110 a 131</td>
  </tr>
  
  <tr>
    <td>RF A007 / Cadastrar pretensão de defesa do TCC</td>
    <td>
      O aluno precisa informar qual semestre ele pretende defender o TCC dele,
      por exemplo, 2022.2
    </td>
    <td>Diretório (back): src/app/controllers/registrationController.js. Linha: 5 até 31.
    <br>
    Diretório (front):
    src/pages/CadastroAluno.js. Linha 132 a 147</td>
  </tr>
  
  <tr>
    <td>RF A008 / Editar perfil</td>
    <td>O aluno precisa acessar seu perfil para editar suas informações pessoais</td>
    <td>Diretório (back): src/app/controllers/registrationController.js. Linha: 5 até 31.</td>
  </tr>

   <tr>
    <td>RF P001 / Cadastrar foto do perfil</td>
    <td>O professor precisa fazer o upload de uma foto para colocar no seu perfil</td>
    <td>Diretório (front): src/components/InputImage/index.js.</td>
  </tr>
  
  <tr>
    <td>RF P002 / Cadastrar descrição da sua forma de orientação</td>
    <td>
      O professor pode dizer em algumas palavras a forma que ele costuma
      orientar
    </td>
    <td>Diretório (back): src/app/controllers/registrationController.js. Linha: 31 até 56
    <br>
    Diretório (front):
    src/pages/CadastroProfessor.js. Linha 41 a 45
    </td>
  </tr>
  
  <tr>
    <td>RF P003 / Cadastrar disponibilidade para orientação</td>
    <td>
      O professor precisa informar a disponibilidade de orientação dele, se está
      disponível, indisponível ou a disponibilidade está em análise
    </td>
    <td>Diretório (back): src/app/controllers/registrationController.js. Linha: 31 até 56
    <br>
    Diretório (front):
    src/pages/CadastroProfessor.js. Linha 47 a 64
    </td>
  </tr>
  
  <tr>
    <td>RF P004 / Cadastrar preferência de modalidade do TCC</td>
    <td>
      O professor pode informar as suas modalidades de TCC que ele tem
      preferência por orientar
    </td>
    <td>
      Diretório (back): src/app/controllers/registrationController.js. Linha: 31 até 56
      <br>
      Diretório (front):
      src/pages/CadastroProfessor.js. Linha 66 a 87
    </td>
  </tr>
  
  <tr>
    <td>RF P005 / Cadastrar áreas de pesquisa</td>
    <td>
      O professor precisa informar as suas áreas de pesquisa, como animação,
      ilustração, etc
    </td>
    <td>Diretório (back): src/app/controllers/registrationController.js. Linha: 31 até 56
    <br>
    Diretório (front):
    src/pages/CadastroProfessor.js. Linha 96 a 110
    </td>
  </tr>
  
  <tr>
    <td>RF P006 / Cadastrar projetos de pesquisa/extensão</td>
    <td>
      O professor pode informar quais projetos de pesquisa ou projetos de
      extensão ele participa ou já participou, e informar o período que
      participou do projeto
    </td>
    <td>Diretório (back): src/app/controllers/registrationController.js. Linha: 31 até 56
    <br>
    Diretório (front):
    src/pages/CadastroProfessor.js. Linha 112 a 154
    </td>
  </tr>
  
  <tr>
    <td>RF P007 / Cadastrar disciplinas que lecionou</td>
    <td>
      O professor pode informar as disciplinas que ele já lecionou e leciona,
      por exemplo, História do Design
    </td>
    <td>Diretório (back): src/app/controllers/registrationController.js. Linha: 31 até 56
    <br>
    Diretório (front):
    src/pages/CadastroProfessor.js. Linha 218 a 231
    </td>
  </tr> 
  
  <tr>
    <td>RF P008 / Editar Perfil</td>
    <td>O professor precisa acessar seu perfil para editar suas informações pessoais</td>
    <td>Diretório (back): src/app/controllers/registrationController.js. Linha: 31 até 56.</td>
  </tr>
  
  <tr>
    <td>RF P009 / Cadastrar Orientando do Portfólio de TCCs</td>
    <td>O professor precisa cadastrar o nome do aluno que foi seu orientando para determinado tema do TCC que está a cadastrar.</td>
    <td>Diretório (back): src/app/controllers/tccController.js. Linha: 3 até 30.</td>
  </tr>
  
  <tr>
    <td>RF P010 / Cadastrar Tema do TCC do Portfólio de TCCs</td>
    <td>O professor precisa cadastrar o tema de um TCC já orientado.</td>
    <td>Diretório (back): src/app/controllers/tccController.js. Linha: 3 até 30.</td>
  </tr>
  
   <tr>
    <td>RF P011 / Cadastrar Descrição do TCC do Portfólio de TCCs</td>
    <td>O professor pode cadastrar uma pequena descrição sobre o TCC, para introduzi-lo e gerar interesse, e até mesmo inspiração, para futuros orientandos.</td>
    <td>Diretório (back): src/app/controllers/tccController.js. Linha: 3 até 30</td>
  </tr>

  <tr>
    <td>RF P012 / Cadastrar palavras-chaves do TCC do Portfólio de TCCs</td>
    <td>O professor pode cadastrar as palavras-chaves do TCC que orientou, para que os alunos possam ver os principais tópicos abordados.</td>
    <td>Diretório (back): src/app/controllers/tccController.js. Linha: 3 até 30.</td>
  </tr>
  <tr>

  <td>RF P013 / Cadastrar Modalidade do TCC do Portfólio de TCCs</td>
    <td>O professor pode cadastrar a modalidade do TCC orientado (artigo científico, relatório técnico ou monografia), para que os alunos identifiquem qual é o tipo de TCC.
</td>
    <td>Diretório (back): src/app/controllers/tccController.js. Linha: 3 até 30.</td>
  </tr>
  
  <tr>
    <td>RF P014 / Cadastrar semestre de defesa do TCC do Portfólio de TCCs</td>
    <td>O professor pode cadastrar o semestre de defesa do TCC orientado.
</td>
    <td>Diretório (back): src/app/controllers/tccController.js. Linha: 3 até 30.</td>
  </tr>

  <tr>
    <td>RF P015 / Cadastrar link do PDF do TCC do Portfólio de TCCs</td>
    <td>O professor pode cadastrar o link do PDF do TCC para que os alunos tenham acesso ao documento completo.</td>
    <td>Diretório (back): src/app/controllers/tccController.js. Linha: 3 até 30.</td>
  </tr>
  
  <tr>
    <td>RF P016 / Editar Portfólio de TCCs</td>
    <td>O professor pode ter a opção de editar o portfólio de TCCs, assim editar informações como o semestre ou a modalidade do TCC.</td>
    <td>Diretório (back): src/app/controllers/tccController.js. Linha: 31 até 48</td>
  </tr>
  
  <tr>
    <td>RF G006 / Pesquisar Professores</td>
    <td>O aluno/professor pode pesquisar os professores pelo nome, por meio de um campo de pesquisa, por exemplo, “Liandro”.</td>
    <td>
      Diretório (back):
    src/app/controllers/listController.js. Linha: 110 até 122.
    <br>
    Diretório (front): src/pages/Search.js. Linha 45 até 48.
    </td>
  </tr>
  
  <tr>
    <td>RF G007 / Pesquisar Área de Pesquisa</td>
    <td>O aluno/professor pode pesquisar uma área de pesquisa, por meio de um campo de pesquisa, por exemplo, “Design”.</td>
    <td>
      Diretório (back):
    src/app/controllers/listController.js. Linha: 124 até 141.
    <br>
    Diretório (front): src/pages/Search.js. Linha 50 até 53.
    </td>
  </tr>
  
  <tr>
    <td>RF G008 / Filtrar por Área de Pesquisa</td>
    <td>O aluno/professor pode filtrar pela área de pesquisa, por meio da barra de navegação que tem os interesses dele que foram cadastrados.
</td>
    <td>
      Diretório (back): src/listControlle.js. Linha 75 até 80. 
      <br>
      Diretório (front): src/components/Carrosel/index.js. Linha 23 até 26
    </td>
  </tr>
  
  <tr>
    <td>RF G009 / Filtrar Professores por Disponibilidade</td>
    <td>O aluno/professor pode filtrar os professores pela disponibilidade, por exemplo, apenas os “disponíveis”.</td>
    <td>
    Diretório (front): src/components/CardGroup/index.js. Linha 73 até 108
    </td>
  </tr>

  <tr>
    <td>RF G010 / Filtrar Professores por Preferência de Modalidade</td>
    <td>O aluno/professor pode filtrar os professores pela preferência de modalidade, por exemplo, apenas os professores que preferem orientar “Relatórios Técnicos”.</td>
    <td>Diretório (front): src/components/CardGroup/index.js. Linha 73 até 108</td>
  </tr>
  
  <tr>
    <td>RF G011 / Filtrar TCC por Modalidade</td>
    <td>O aluno/professor pode filtrar os TCCs pela modalidade, por exemplo, só os TCCs que são “Monografia”.</td>
    <td>Diretório (front): src/components/CardGroup/index.js. Linha 118 até 154</td>
  </tr>
  
  <tr>
    <td>RF G012 / Filtrar TCC por Semestre</td>
    <td>O aluno/professor pode filtrar os TCCs por semestre, por exemplo, só os TCCs que foram defendidos em 2021.1</td>
    <td>Diretório (front): src/components/CardGroup/index.js. Linha 118 até 154</td>
  </tr>

 <tr>
    <td>RF G013 / Visualizar Lista de Professores</td>
    <td>O aluno/professor pode visualizar uma lista de professores como resultado da pesquisa.</td>
    <td>
      Diretório (back): src/controllers/listController.js. Linha 82 até 86.
      <br>
Diretório (front): src/contexts/ListContext.js Linha 21 até 24 
   </td>
  </tr>
 
 <tr>
    <td>RF G014 / Visualizar Lista de TCCs</td>
    <td>O aluno/professor pode visualizar uma lista de TCCs como resultado da pesquisa.</td>
    <td>Diretório (back): src/controllers/listController.js. Linha 63 até 66
  <br>
  Diretório (front): src/contexts/ListContext.js Linha 21 até 24
  </td>
  </tr>

  <tr>
    <td>RF G016 / Visualizar Meu Perfil</td>
    <td>O aluno/professor pode visualizar seu próprio perfil por meio de um menu dropdown localizado na barra de navegação global, assim ao clicar em “Ver perfil”, ele tem acesso ao próprio perfil.</td>
    <td>Diretório (back): src/controllers/listController.js. Linha 6 a 61.
  <br>
  Diretório (front): src/pages/VisualizarMeuPerfil.js
  </td>
  </tr>
  
  <tr>
    <td>RF G017 / Visualizar Perfil do Professor</td>
    <td>O aluno/professor pode visualizar o perfil do professor por meio do botão “Ver perfil” localizado no card do resultado da pesquisa.</td>
    <td>Diretório (back): src/controllers/listController.js. Linha 88 a 93.
  <br>
  Diretório (front): src/pages/VisualizarProfessor.js Linha 20 até 23
  </td>
  </tr>
  
  <tr>
    <td>RF G018 / Visualizar um TCC</td>
    <td>O aluno/professor pode visualizar um TCC por meio do botão “Ver TCC” localizado no card do resultado da pesquisa.</td>
    <td>Diretório (back): src/controllers/listController.js. Linha 95 a 101.
  <br>
  Diretório (front): src/pages/VisualizarTCC.js
  </td>
  </tr>
  
  <tr>
    <td>RF P019 / Visualizar Perfil do Aluno</td>
    <td>O professor pode visualizar o perfil do aluno para verificar se os seus interesses estão alinhados.</td>
    <td>
      Diretório (back): src/controllers/listController.js. Linha 103 a 108.
<br>
Diretório (front): src/pages/VisualizarAluno.js Linha 17 a 20.
  </td>
  </tr>
</table>

## :memo: Licença

Este projeto está sob a licença MIT. Veja o [LICENSE](https://img.shields.io/badge/License-ISC-yellow.svg) para maiores informações.

## :love_letter: Contribua com o projeto!

Você é do SMD e se interessou pelo projeto? Que tal contribuir com o desenvolvimento da aplicação? É só entrar em contato com esse [email](
https://mail.google.com/mail/u/?authuser=lariaraujo201@gmail.com), que batemos um papo 🐟 

---

Feito com 💜 by [Spaceship](https://github.com/Spaceship-PI1)
