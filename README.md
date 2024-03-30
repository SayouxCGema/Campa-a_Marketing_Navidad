# Campaña_Marketing_Navidad
Proyecto de análisis para ayudar al departamento de marketing a definir el cliente que tiene mayores probabilidades de realizar la oferta de la campaña de Navidad.

Acerca del conjunto de datos:
- Un gran supermercado está planeando las rebajas de fin de año. Quieren lanzar una nueva oferta: la afiliación de oro, que ofrece un 20% de descuento en todas las compras, por solamente 499 €, que son 999 € en otros días. Solo será válida para los clientes actuales, para los que se está planeando una campaña de llamadas telefónicas.

La dirección considera que la mejor manera de reducir el coste de la campaña es realizar un modelo predictivo que clasifique a los clientes que podrían comprar la oferta.

[Source](https://www.kaggle.com/datasets/ahsan81/superstore-marketing-campaign-dataset/data)

### Objetivo
El supermercado quiere predecir la probabilidad de que el cliente dé una respuesta positiva y quiere identificar los diferentes factores que afectan a la respuesta del cliente. Hay que analizar los datos proporcionados para identificar estos factores y luego construir un modelo de predicción para predecir la probabilidad de que un cliente dé una respuesta positiva.

- Response (target): 1 si el cliente aceptó la oferta en la última campaña, 0 en caso contrario
- ID: Identificación única de cada cliente
- Year_Birth: Age of the customer
- Complain: 1 si el cliente se ha quejado en los últimos 2 años
- Dt_Customer: fecha de inscripción del cliente en la empresa
- Education: nivel de estudios del cliente
- Marital:estado civil del cliente
- Kidhome: número de niños pequeños en casa del cliente
- Household Teenhome: número de adolescentes del cliente
- Household Income: ingresos familiares anuales del cliente
- MntFishProducts: el importe gastado en productos pesqueros en los últimos 2 años
- MntMeatProducts: el importe gastado en productos cárnicos en los últimos 2 añoss
- MntFruits: el importe gastado en frutas en los últimos 2 años
- MntSweetProducts: el importe gastado en dulces/postres en los últimos 2 años
- MntWines: el importe gastado en vinos en los últimos 2 años
- MntGoldProds: el importe gastado en productos premium/dorados en los últimos 2 años
- NumDealsPurchases: número de compras realizadas con descuento
- NumCatalogPurchases: número de compras realizadas por catálogo (compra de productos que se envían por correo)
NumStorePurchases: número de compras realizadas en tienda
NumWebPurchases: número de compras realizadas en en la web
NumWebVisitsMonth: numero de visitantes en la pág web en el último mes.

### Preparación de los datos.
- No se encuentran valores duplicados en el análisis
- Tampoco se encuentran valores nulos
- Se agregan variables para segmenentar a los clientes por grupos de edad


### Análisis

Visto que tenemos una variable que nos muestra el total de participantes en la última campaña de promoción, esta será la que utilizaré para definir el perfil de los clientes y comprobar si están datos que muestren una correlación que permita identificar el total de clientes a los que informar sobre la campaña de Navidades.
Sobre esta base, se puede observar qué: 
- El 14,91% de clientes, participaron en la última promoción, mientras que el otro 85,09% no lo hicieron.
- De este 14,91% el 31% de los clientes son solteros. PD: Se puede pedir que implementen en la información de registro la opción de identificar a los clientes por su género.
- Son más personas con títulos de graduados y doctorados. Aunque el gasto medio mayor es de personas con un doctorado.
- Dentro de 14,91% de clientes que han realizado el descuento, los que muestran un mayor gasto medio acumulado en estos dos años, son el grupo de mayores. [+60] Pero han mostrado mayor indice de participación el grupo de usuarios jovenes[27-49].
- Al aplicar un modelo de clasificación se encontró que si el número de **pedidos online es superior a 5** y han realizado **más de 9 descuentos**, es un posible cliente que esté interesado en la oferta.
- Si realizan **4 pedidos online y más de 10 compras en tienda**, también es mayor la probabilidad de que hagan una oferta.En cambio, están con menor probabilidades de obtar por una oferta, aquellos que han realizado menos de 2 compras online, que han utilizado las promociones menos de 2 ocasiones.

### Resultados.

- Después de poder identificar en la base de datos, aquellos clientes que cumplen con esas condiciones, hemos detectado que están **10 usuarios**, a los que se les puede informar de esta promoción, ya que han demotsrado mayores probabilidades de participación.

