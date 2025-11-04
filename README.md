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
Por ejemplo:

