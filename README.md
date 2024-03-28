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
Recency: número de días transcurridos desde la última compra
