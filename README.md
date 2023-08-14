Inforiesgo

Bienvenido a Inforiesgo, una herramienta desarrollada por Consultoria SES que te proporciona información sobre zonas de riesgo en ciertas localidades. Con Inforiesgo, puedes consultar datos geoespaciales relacionados con zonas de riesgo utilizando tanto un cliente web como un bot de Telegram.
Características

    Consulta zonas de riesgo en Pereira, Dosquebradas y La Virginia.
    Realiza consultas a través del cliente web en consultoriases.com o el bot de Telegram (@inforiesgo_bot).
    Obtén información detallada sobre la amenaza y el barrio asociado a un número predial específico.
    Interfaz de usuario amigable y fácil de usar.

Guía de Instalación

Requisitos Previos:

    Node.js instalado en tu sistema.
    Tomcat para la parte del cliente web.

Pasos:

    Clona este repositorio en tu máquina local:

    bash

git clone https://github.com/SESMAPS/inforiesgo.git

Instala las dependencias para el bot de Telegram:

bash

cd inforiesgo/telegram-bot
npm install

Configura el bot de Telegram:

    Crea un bot en Telegram y obtén el token de acceso.
    Renombra el archivo config.example.js a config.js en la carpeta telegram-bot y agrega el token de acceso.

Ejecuta el bot de Telegram:

bash

    node main-bot.js

    Configura y despliega el cliente web:
        Configura tu servidor Tomcat para servir el cliente web ubicado en la carpeta web-client.
        Asegúrate de que las dependencias estén instaladas y que el servidor esté funcionando correctamente.

Guía de Uso
Cliente Web

    Accede al cliente web en consultoriases.com.
    Ingresa el número predial de 30 dígitos correspondiente a la localidad (6600s para Pereira, 6617 para Dosquebradas y 6640 para La Virginia).
    Presiona el botón "Consultar" para obtener información sobre la amenaza y el barrio asociado.

Bot de Telegram

    Abre Telegram y busca el bot @inforiesgo_bot.
    Inicia una conversación con el bot.
    Envía el número predial de 30 dígitos correspondiente a la localidad (6600s para Pereira, 6617 para Dosquebradas y 6640 para La Virginia).
    Recibirás información detallada sobre la amenaza y el barrio asociado.

Arquitectura y Diseño

Inforiesgo se compone de tres partes principales: el cliente web, el bot de Telegram y las capas geoespaciales disponibles en Geoserver de Consultoria SES. Las consultas se realizan pasando el código a buscar en un CQL, y no se almacenan datos de consultas de usuarios en CSV.
APIs y Endpoints

    Cliente Web:
        Endpoint: consultoriases.com/informacion-de-zonas-de-riesgo/
    Bot de Telegram:
        Bot: @inforiesgo_bot

Configuración

La configuración varía según si estás utilizando el cliente web o el bot de Telegram. Consulta las secciones de Guía de Instalación para obtener detalles específicos.
Mantenimiento y Contribución

Inforiesgo es un proyecto en constante evolución. Si encuentras errores, tienes ideas para mejoras o deseas contribuir de alguna manera, siéntete libre de crear un pull request en el repositorio GitHub.
Licencia y Atribuciones

Inforiesgo está licenciado bajo la licencia Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0). Para obtener más detalles sobre la licencia, consulta Licencia CC BY-NC-ND 4.0.
FAQ y Solución de Problemas

Consulta las preguntas frecuentes y la solución de problemas en la sección correspondiente de este documento.
Contacto y Soporte

Si tienes preguntas, comentarios o necesitas asistencia, puedes contactar a Consultoria SES a través de su sitio web, Telegram, teléfono (305 439 2506) o dirección en Pereira, Risaralda.
Actualizaciones y Versionado

Las actualizaciones y las versiones de Inforiesgo se encuentran en el repositorio GitHub. Asegúrate de consultar las últimas versiones para acceder a las características más recientes y las mejoras implementadas.
