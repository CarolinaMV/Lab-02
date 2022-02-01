# Lab-02

## EJERCICIO DE LAS FIGURAS

### CREAR UN PROYECTO CON MAVEN

* Creación un proyecto maven con ayuda de los arquetipos 

  ```
  mvn archetype:generate -DgroupId=edu.eci.cvds -DartifactId=Patterns -DarchetypeArtifactId=maven-archetype-quickstart
  ```
* Para ver el conjunto de archivos y directorios creados por el comando mvn ejecute el comando tree.
  
  ![image](https://user-images.githubusercontent.com/98135902/152020192-d663ad7c-4314-47ba-979a-a6b04a77e39a.png)

### AJUSTAR ALGUNAS CONFIGURACIONES EN EL PROYECTO

* Archivo pom editado

  ![image](https://user-images.githubusercontent.com/98135902/152020258-d4b20974-da7c-4528-b992-dbf2e6c82ed5.png)


### COMPILAR Y EJECUTAR

* Ejecución del programa

  ```
  mvn package
  ```
  ![image](https://user-images.githubusercontent.com/98135902/152020441-16b38972-6ee5-4f0f-a6ef-f5727f39198c.png)

* Busque cuál es el objetivo del parámetro "package" y qué otros parámetros se podrían enviar al comando mvn.\
  El objetivo de "package" es tomar el código compilado y lo empaqueta en su formato distribuible, como un JAR.
  * mvn clean Borra todos los .class y .jar generados.
  * mvn compile Compila el proyecto.
  * mvn package Genera el jar.
  * mvn install LLeva el jar a nuestro repositorio local de jars. Queda "visible" para otros proyectos maven en nuestro ordenador.
  * mvn deploy Lleva el jar a nuestro servidor de jars. Queda "visible" para otros proyectos maven en otros ordenadores. Este comando necesita que a maven se le haya indicado       dónde está dicho servidor de jars.
  * mvn javadoc:javadoc Genera la documentación javadoc de nuestro proyecto.
  * mvn site Genera documentación html del proyecto. Por supuesto, necesitamos haber escrito en determinados ficheros el contenido de esa documentación.
*s
