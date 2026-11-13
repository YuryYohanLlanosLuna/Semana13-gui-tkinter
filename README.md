# Práctica Semana 13 - Diseño de Interfaces Gráficas (GUI) con Tkinter


## 1. Archivos del Proyecto
calculadora.py: Calculadora funcional construida con el gestor de geometría grid().
formulario.py: Formulario de registro de usuarios estructurado mediante POO.
wireframe.png: Boceto de baja fidelidad que define la estructura inicial del formulario.
## 2. Decisiones de Diseño y Principios de Usabilidad
Para el desarrollo de estas aplicaciones se aplicaron los siguientes principios de usabilidad (Jakob Nielsen) y accesibilidad:


**Prevención y manejo de errores:** En el formulario, se implementaron validaciones estrictas al presionar "Registrar" (verificación de campos vacíos, formato de correo con @, contraseñas coincidentes y validación de tipos de datos en la edad). En la calculadora, se controla la excepción de "Expresión inválida" mediante bloques try-except para evitar que la aplicación se cierre inesperadamente.
**Visibilidad del estado del sistema y retroalimentación:** El sistema se comunica constantemente con el usuario. Se utilizan ventanas emergentes (messagebox) para notificar los errores específicos de validación en forma de lista o para confirmar el éxito del registro. En la calculadora, el display refleja inmediatamente cada botón presionado.
**Consistencia y estándares:** Se respetaron los modelos mentales de los usuarios utilizando convenciones estándar del sistema. Las contraseñas se ocultan visualmente usando show="*", las opciones exclusivas utilizan Radiobuttons, y los botones de acción primaria ("Registrar" y "Limpiar") se agrupan en la parte inferior.
**Accesibilidad y Claridad:** Todos los widgets de entrada (Entry) están precedidos por una etiqueta (Label) descriptiva clara alineada a la derecha. El diseño respeta un orden de tabulación (Tab order) lógico y secuencial de arriba hacia abajo.