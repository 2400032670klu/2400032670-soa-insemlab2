SERVICE LAYER DEPENDENCY MOCKING - LAB PROJECT

Requirements:
- JDK 17 or later
- Maven (or import as an Existing Maven Project in STS/Eclipse)

Project structure:
ServiceLayerMocking
|-- src/main/java/com/example/demo
|   |-- DemoApplication.java
|   |-- User.java
|   |-- UserService.java
|   `-- UserController.java
|-- src/test/java/com/example/demo
|   `-- UserControllerTest.java
`-- pom.xml

Run in Spring Tool Suite (STS):
1. Extract this ZIP file.
2. Open STS.
3. Select File > Import > Maven > Existing Maven Projects.
4. Browse to the extracted ServiceLayerMocking folder.
5. Select the pom.xml and click Finish.
6. Wait for Maven dependencies to download.
7. Open src/test/java/com/example/demo/UserControllerTest.java.
8. Right-click the file and choose Run As > JUnit Test.

Expected result:
Tests run: 1, Failures: 0, Errors: 0

The test uses @WebMvcTest and @MockBean. The real UserService is replaced
with a mock, so the controller test does not require a database connection.
