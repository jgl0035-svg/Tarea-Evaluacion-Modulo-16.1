# Tarea Módulo 16.1 – Pruebas con Selenium y JUnit

En esta tarea he creado pruebas automatizadas para la página de login de SauceDemo utilizando **Java**, **Selenium WebDriver**, **JUnit 5** y **WebDriverManager**.

---

## Preguntas

### ¿Qué hace la anotación `@BeforeEach`?

La anotación **@BeforeEach** se ejecuta antes de cada test. La utilizo para dejar todo preparado antes de cada prueba, por ejemplo iniciar el navegador, maximizar la ventana y abrir la página de SauceDemo.

---

### ¿Para qué sirve `assertTrue`?

**assertTrue** sirve para comprobar que una condición es verdadera.  
Si la condición no se cumple, el test falla y me indica que algo no está funcionando como debería en el comportamiento que estoy probando.

---

### ¿Qué diferencia hay entre `findElement()` y `findElements()`?

- **findElement()** devuelve **un solo elemento**.  
  Si no encuentra ninguno, lanza una excepción y el test falla en ese punto.

- **findElements()** devuelve **una lista de elementos**.  
  Si no encuentra nada, devuelve una lista vacía, pero no lanza excepción.

---

### ¿Por qué utilizamos una clase LoginPage en lugar de escribir todo en el test?

Utilizamos una clase **LoginPage** para aplicar el patrón **Page Object**.  
De esta forma separo la lógica de la página (localizadores y acciones como escribir usuario, contraseña o hacer clic en Login) del código del test.  
Esto hace que el código sea más limpio, más fácil de mantener y me permite reutilizar los mismos métodos de la página en
