# external-Case-Creation
#	Descripción

Se quiere revisar la posibilidad de crear casos desde una web externa a Salesforce, sin que se requiera iniciar sesión, esto, con el fin de que los clientes puedan crear casos adjuntando archivos
# Diagnostico

•	Se debe crear un visualforce con su controlador respectivo ya que se evidencia que por defecto Salesforce no permite añadir archivos.
#	Solución

<ol>
  <li>Se crea un formulario visualforce con los campos que se necesiten haciendo uso de los campos predeterminados con los que cuenta visualforce.</li>
  <li>Se crea un controlador que se encarga de enviar los datos ingresados en el formulario.</li>
  <li>Se crea desde configuración un “Site” desde el cual se llama a la página visualforce, se debe tener en cuenta que este no debe estar protegido y que al usuario se le deben asignar todos los permisos, esto con el objetivo, de que al llamarlo desde la web externa no se presenten errores.</li>
  <li>Para añadirlo al sitio requerido se hace usando un iframe en el cual se pone el enlace del site creado anteriormente.</li>
</ol>

• Github que contiene los códigos utilizados:  https://github.com/creacioncasos/external-Case-Creation
<br/>
•	Demo (Estilo Salesforce classic):  https://creacioncasos.github.io/
