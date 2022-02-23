# Flujo de notificación

Lo primero que se debe de tomar en cuenta en la notifiación, esta se va a realizar a un endpoint expuesto por el comercio, la estructura es la que se define en el `body` del ejemplo del API que debe de generar el comercio, una vez el comercio recibe la notificación, es necesario que el parametro `sessionId` sea almacenado en la información de la orden.

El IVR notifica cuando la transacción es culminada de parte de su propio flujo, pero unicamente notificara transacciones `APPROVED` o `FAILED`, las `PENDING` van a ser notificadas a travez de una tarea programada al mismo endpoint que expone el cliente para la notificación.

<!-- Agregar modelo de flujo aca!  -->
