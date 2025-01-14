# Beverage Sales
Este conjunto de dados foi criado para simular padrões de vendas realistas na indústria de bebidas, destacando fatores importantes como preferências regionais, flutuações sazonais e segmentação de clientes. Ele apresenta transações Business-to-Business (B2B) e Business-to-Consumer (B2C), tornando-o adaptável para uma variedade de propósitos analíticos.

# Dados utilizados:

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

**Para começar, conheci um pouco mais sobre os dados utilizando a biblioteca pandas:**

**Overview da tabela**
> sales.head()
![image](https://github.com/user-attachments/assets/6ba06efc-62fa-4101-ae73-0dd0c577f548)

**Tipos dos dados**
>sales.info()

![image](https://github.com/user-attachments/assets/5bac56e4-f3a5-4d47-a17f-18aa1e457d18)

**Verificando dados nulos**
>sales.isnull().sum()

![image](https://github.com/user-attachments/assets/5518a754-cecd-4e40-ba0c-c784ba162b1c)

**Depois do primeiro contato, comecei a me fazer algumas perguntas:**

** Quais foram as vendas por região?**
> sales.groupby('Region')['Total_Price'].sum().sort_values(ascending=False)

![image](https://github.com/user-attachments/assets/eb0795a9-7678-464e-b419-e3520d8275e3)

**Qual Categoria vendeu mais?**
> sales.groupby('Category')['Total_Price'].sum().sort_values(ascending=False)

![image](https://github.com/user-attachments/assets/bb7bacf5-7a6b-46b9-a10f-428ad1ce830a)



