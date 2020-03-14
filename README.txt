Testado com JRE8 e JRE9, Apache Tomcat 7,8,9

1) Para compilar e empacotar na linha de comando use:

> mvn clean package

2) Para rodar no Eclipse com Tomcat no profile "dev" adicione "-Dspring.profiles.active=dev" 
nas "Run Configurations..." (ou descomento o método "onStartup" na classe "ServletSpringMVC")

Ao rodar pelo Eclipse e Tomcat acesse 

http://localhost:8080/casadocodigo

3) Para rodar na linha de comando (no profile dev usando tomcat 9) use:

> java -jar -Dspring.profiles.active=dev target/dependency/webapp-runner.jar target/*.war

e acesse http://localhost:8080/


