# Beverage Sales
Este conjunto de dados foi criado para simular padrões de vendas realistas na indústria de bebidas, destacando fatores importantes como preferências regionais, flutuações sazonais e segmentação de clientes. Ele apresenta transações Business-to-Business (B2B) e Business-to-Consumer (B2C), tornando-o adaptável para uma variedade de propósitos analíticos.

# Colunas 

- Order_ID Identificador exclusivo para cada pedido. Agrupa vários produtos no mesmo pedido.
- Customer_ID Identificador exclusivo para cada cliente, distinguindo compradores individuais.
- Customer_Type Indica se o cliente é B2B (business-to-business) ou B2C (business-to-consumer).
- Product O nome do produto adquirido, como "Coca-Cola" ou "Erdinger Weißbier".
- Category A categoria do produto, como "Refrigerantes" ou "Bebidas Alcoólicas".
- Unit_Price O preço por unidade do produto.
- Quantity O número de unidades compradas para o produto especificado no pedido.
- Discount O desconto aplicado ao produto (por exemplo, 0,1 para 10%). Os descontos são concedidos apenas a clientes B2B.
- Total_Price O preço total do produto após a aplicação dos descontos.
- Region A região do cliente, como "Bayern" ou "Berlin".
- Order_Date A data em que o pedido foi feito.
