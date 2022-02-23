# Integración con IVR
Este documento tiene como objetivo indicar las estructuras de notificación y consulta de información de las transacciones que se generan en la plataforma de IVR.

IVR PlacetoPay es un producto que surge ante la necesidad que tienen las compañías de poder vender telefónicamente, garantizando que la captura de los datos sensibles de tarjeta de crédito se realice de manera segura, es decir, sin que se exponga dicha información, dado que el usuario final registrará en el teclado de su teléfono los datos sensibles para procesar la transacción.

Para efectos de seguridad es importante saber que PlacetoPay está certificada en la norma internacional PCI DSS de seguridad como Proveedor de Servicio en el Nivel 1, el más alto estándar en seguridad en transacciones con tarjetas de crédito a nivel mundial.

Para usar el servicio web, deberás tener un lenguaje de programación que pueda comunicarse con un servicio REST.

A continuación, se describirán cada uno de los usos y los datos requeridos en la trama para cada uno de los casos. La respuesta para cada operación está unificada en un solo tipo de trama resultante.

## ¿Para quienes está diseñado este Webservice?
Este Webservice está diseñado para ser consumido por los comercios que estén conectados con Placetopay por el servicio de IVR, para consultar a partir de un dato la información de un pago que este pendiente para ser recaudar, consultar las transacciones que han generado un flujo transaccional para notificar una transacción en su estado final.

## ¿Cómo funciona?
Se realizan consumos individuales a cada uno de los endpoints de acuerdo con la necesidad.
