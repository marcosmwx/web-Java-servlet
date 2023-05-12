# Java Servlet: web, autenticação, autorização e o padrão MVC

## Projeto
### Este projeto foi feito com apoio dos exercícios e aprendizados das aulas do curso de Java Servlet (Oracle + Alura)<br>
<p>O projeto é capaz de logar o usuário, listar empresas fazendo uma requisição de dados na memória (não foi utilizado um banco de dados específico, não era o intuito do curso, mas seria totalmente viável), adicionar uma empresa, editar empresas existentes e excluir. A aplicação está preparada para retornar um JSON para clientes webservice caso necessário.
 O projeto não tem nenhuma camada de estilo pois o foco era explorar o conteúdo aprendido nas aulas de Servlet

<p> Ciclo do projeto: 
<ol>
    <li>Simular uma aplicação de login capaz de autorizar ou não o usuário através de filtros utilizando HttpSession (ID Cookies)</li>
    <li>Com o usuário autorizado logado, ele será redirecionado para lista de empresas</li>
    <li>Na lista de empresas, ele será capaz de sair, editar uma empresa ou excluir</li>
    <li>Ele é capaz de adicionar uma empresa através do formulário</li>
    <li>Não é capaz de acessar nenhuma das páginas ou fazer requisições sem autorização ou estando deslogado</li>
    <li>O arquivo web.xml é capaz de gerenciar a ordem de execução dos filtros</li>
    <li>Utiliza servidores como Tomcat ou Jetty para ser executado</li>
    <li>Foi disponibilizado um arquivo do projeto .war para ser visualizado através do Tomcat 9</li>
</ol>

## Como executar o projeto
<ol>
  
  <li> Basta utilizar o servidor TomCat v9.0[link](https://tomcat.apache.org/download-90.cgi) </li>
  <li> Copie o arquivo WAR do projeto Java para a pasta "webapps" do TomCat </li>
  <li> Através do Cmd navegue até a pasta BIN do TomCat e Execute o arquivo "startup.bat" (Windows) ou "startup.sh" (Linux/Unix) para iniciar o servidor Tomcat. </li>
  <li> No navegador você será capaz de acessar a seguinte página:  </li>
  <li> [Pagina de Login](http://localhost:8080/gerenciador/entrada?acao=LoginForm)
  <li> Login: marcos / Senha: 123  </li>
  <li> Logado, você será redirecionado e poderá utilizar alguns métodos <</li>
  <li> Para adicionar uma nova empresa, você pode acessar este link: [Nova Empresa](http://localhost:8080/gerenciador/entrada?acao=NovaEmpresaForm) </li>
  <li> Para webservices que recebem JSON, você pode acessar diretamente com este link: [Link](http://localhost:8080/gerenciador/empresas)</li>


## Dependências do Projeto
[gson-2.8.5](https://sites.google.com/site/gson/gson-user-guide)<br>
[jstl-1.2](https://tomcat.apache.org/taglibs/site/tutorial.html)<br>
[TomCat](https://tomcat.apache.org/download-90.cgi)
