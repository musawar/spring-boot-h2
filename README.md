# Spring-boot-h2 Swagger
In this example I have used H2 as in memory database and rest web services are exposed via Swagger-UI.
Project can be executed as follows: 

 - mvn clean
 - mvn install
 - mvn spring-boot:run

After the project is up and running DB , Services and Swagger-UI can be accessed as follows:

 - DB
	 - Access localhost:8080/h2-console     with schema jdbc:h2:mem:testdb  connect and see tables data.
 
 - Services

	 - Department
		 - GET  localhost:8080/dept/getAllDept
	 	 - GET  localhost:8080/dept/getDeptById/{deptno}
		 - POST localhost:8080/dept/insertDept
		 - PUT localhost:8080/dept/updateDept
		 - DELETE localhost:8080/dept/deleteDept/{deptno}	

	 - Employee
		 - GET  localhost:8080/emp/getAllEmployee
		 - GET  localhost:8080/emp/getEmpById/{empno}
		 - DELETE localhost:8080/emp/deleteEmp/{empno} 
		 
 - Swagger-UI
	 - localhost:8080/swagger-ui.html
