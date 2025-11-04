## Trabajo Práctico – Algoritmos I (UNSAM)
## Apps Script + Google Sheets

**Google Sheets** es parte de la suite **Google Docs Editors** y permite trabajar con datos de forma colaborativa y en tiempo real.  
Aunque no está pensado para proyectos complejos, resulta ideal para tareas de pequeña escala donde se necesita rapidez y facilidad de uso.

En este trabajo práctico vamos a utilizar **Apps Script**, una plataforma de desarrollo basada en **JavaScript** que funciona directamente en la nube.  
No requiere instalación y nos permitirá automatizar procesos dentro de Google Sheets de manera sencilla.

Nuestro objetivo será trabajar con una tabla de datos perteneciente a una empresa ficticia llamada **Nosce Te Ipsum**, implementando distintas funcionalidades mediante código.

---

## 🔧 Acceso a Apps Script

Para empezar, abrí el archivo de Google Sheets y andá a:

> **Extensiones → Apps Script**

Ahí es donde escribiremos el código necesario para automatizar las tareas.

---

## ⚠️ Importante

- Todo lo que implementes debe hacerse con código **JavaScript** en **Apps Script**.  
- **No** vamos a usar funciones nativas de Google Sheets para resolver los ejercicios.

Se trabajará sobre una tabla que tiene las siguientes columnas:

| Columna | Descripción |
|----------|--------------|
| **Name** | Nombre y apellido del empleado. |
| **Mail** | Email con el formato “primera letra del nombre + apellido”. |
| **Alias** | A completar en el ejercicio 3. |
| **Hash** | Código único interno de 50 caracteres en minúscula. |

Además, para los ejercicios 2 y 3 deberás crear un **menú personalizado** en la barra superior, llamado **“Validaciones”**, con estas opciones:

- **Validar Mails** → para el ejercicio 2.  
- **Alias** → para el ejercicio 3.

El menú también debe crearse usando **Apps Script**.  

Antes de empezar, hacé una **copia del archivo indicado**.  
Te pedirá si querés copiar también el Apps Script: respondé que **sí**.  
Todo el trabajo se hará ahí.

---

## 🧩 Consignas

### Ejercicio 1

Cada vez que alguien modifique la hoja, en la celda **B1** debe guardarse automáticamente la **fecha y hora del último cambio**.  
Cada modificación debe actualizar este valor.

---

### Ejercicio 2

**Validación de formato de email y resaltado de errores**

En la columna **Mail (columna B)** verificar que cada dirección de correo electrónico cumpla con el formato corporativo establecido.  

La regla de formato indica que el correo debe componerse por la primera letra del nombre seguida del apellido completo, seguido del dominio de la empresa.  
Por ejemplo: jdoe@empresa.com


En caso de detectar un correo con formato incorrecto, el script deberá **resaltar la celda correspondiente con un color específico**.  
El proceso debe ejecutarse **solo cuando se presione el botón “Validar Mails”** del menú que creaste.

---

### Ejercicio 3

Para proteger la identidad de los empleados, se debe generar un **alias único y aleatorio** para cada uno.  

Se proporcionará una API que devuelve nombres de personajes de Harry Potter:

> https://hp-api.onrender.com/api/characters

La idea es usar esta API para completar la columna **C (Alias)** con los nombres obtenidos.  
El proceso debe ejecutarse **solo cuando se presione el botón “Alias”** del menú que creaste.

---

### 🪄 Bonus

Hacer un **mensaje emergente tipo pop-up** relacionado al punto 2.

---




## 📎 Archivo de trabajo

Podés acceder a la hoja de cálculo base en el siguiente enlace:

👉 [Google Sheets – Trabajo Práctico Apps Script](https://docs.google.com/spreadsheets/d/1XnFH5C-qtKUmu9xqSfuJJI0sA-DxujZReBtBxUrcP0M/edit?usp=sharing)

---

## ✉️ Docentes para la corrección

**Corrección (copiar todos):**  
flrossi@estudiantes.unsam.edu.ar, lgalizzi@unsam.edu.ar, cuellosantino11@gmail.com, jlopez@unsam.edu.ar, nvargas@estudiantes.unsam.edu.ar

---