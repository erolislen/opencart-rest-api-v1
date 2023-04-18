

## API Endpoints for Category

The following API endpoints are available for managing category related data:

#### Get Category Details

```http
  GET /api/rest/category
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `category_id`| `string` | Belirtilen kategori ID'sine sahip kategorinin ayrıntılarını alır. |

#### Get List of Categories

```http
  GET /api/rest/categories
```


| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `status` `orderby` `sort` `limit`| `string` | Mağazadaki tüm kategorilerin listesini alır.|



#### Deleting Category Data

```http
  DELETE /api/rest/category
```

| Parameter    | Type     | Description                |
| :--------    | :------- | :------------------------- |
| `category_id`| `string` | Belirtilen kategori ID'sine sahip kategoriyi siler.      |



## API Endpoints for Customer

The following API endpoints are available for managing customer related data:

#### Get Customer Details

```http
  GET /api/rest/customer
```

| Parameter    | Type     | Description                |
| :--------    | :------- | :------------------------- |
| `customer_id`| `string` | Belirtilen müşteri ID'sine sahip müşterinin ayrıntılarını alır.|

#### Get Customer By Email

```http
  GET api/rest/customer/getCustomerByEmail
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `email`     | `string` | Mağazadaki tüm müşterilerin listesini alır.|


#### Get Customers

```http
  GET api/rest/customer/getCustomers
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `status` `orderby` `sort` `limit`| `string` | Belirtilen e-posta adresine sahip müşterinin ayrıntılarını alır.|

#### Delete Customer

```http
  DELETE /api/rest/customer/deleteCustomer
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `customer_id`| `string` | Belirtilen müşteri ID'sine sahip müşteriyi siler.    |

#### Get Customer Group Details

```http
  GET /api/rest/customer/getCustomerGroup
```

| Parameter    | Type     | Description                |
| :--------    | :------- | :------------------------- |
| `customer_group_id`| `string` | Belirtilen müşteri grubu ID'sine sahip müşteri grubunun ayrıntılarını alır.|

#### Get Customer Groups

```http
  GET api/rest/customer/getCustomerGroups
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `orderby` `sort` `limit`| `string` | Mağazadaki tüm müşteri gruplarının listesini alır.|


## API Endpoints for Localisation

The following API endpoints are available for managing localisation related data:

#### Get Country Details

```http
  GET /api/rest/localisation/getCountry
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `country_id`| `string` | Belirtilen ülke ID'sine sahip ülkenin ayrıntılarını alır  |

#### Get List of Countries

```http
  GET /api/rest/localisation/getCountries
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `status` `orderby` `sort` `limit`| `string` | Mağazadaki tüm ülkelerin listesini döndürür.|


#### Get Zone Details
```http
  GET /api/rest/localisation/getZone
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `zone_id`    | `string` | Belirtilen bölge ID'sine sahip bölgenin ayrıntılarını alır      |

#### Get List of Zones for a Country

```http
  GET /api/rest/localisation/getZonesByCountryId
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `country_id` | `string`| Belirtilen ülke ID'sine sahip tüm bölgelerin listesini döndürür.     |


#### Get Currency Details by Code or List of Currencies

```http
  GET /api/rest/localisation/getCurrencyByCode
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `code`       | `string`| Belirtilen para birimi koduna sahip para biriminin ayrıntılarını alır.   |

#### Get List of Currencies

```http
  GET /api/rest/localisation/getCurrencies
```


| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `status` `orderby` `sort` `limit`| `string` | 	Mağazadaki tüm para birimlerinin listesini döndürür.|


#### Get Language Details

```http
  GET /api/rest/localisation/getLanguage
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `code`       | `string`| Belirtilen dil koduna sahip dilin ayrıntılarını alır.

#### Get List of Languages

```http
  GET /api/rest/localisation/getLanguages
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `status` `orderby` `sort` `limit`| `string` | Mağazadaki tüm dillerin listesini döndürür.|


#### Get Order Status Details by ID or List of Order Statuses

```http
  GET /api/rest/localisation/getOrderStatus
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `order_status_id`| `string`| Belirtilen sipariş durumu ID'sine sahip sipariş durumunun ayrıntılarını alır.|


#### Get List of Order Statuses

```http
  GET /api/rest/localisation/getOrderStatuses
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `language_id` `orderby` `sort` `limit`| `string` | Mağazadaki tüm sipariş durumlarının listesini döndürür.|

 

## API Endpoints for Manufacturer

The following API endpoints are available for managing manufacturer related data:

#### Get Manufacturer Details

```http
  GET /api/rest/manufacturer/getManufacturer
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `manufacturer_id`| `string` | Belirtilen üretici ID'sine sahip üreticinin ayrıntılarını alır.  |

#### Get List of Manufacturers

```http
  GET /api/rest/manufacturer/getManufacturers
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `status` `orderby` `sort` `limit`| `string` | Mağazadaki tüm üreticilerin listesini alır.|


#### Get Total Manufacturers
```http
  GET /api/rest/manufacturer/getTotalManufacturers
```

Mağazadaki tüm üreticilerin toplam sayısını döndürür.

#### Get List of Zones for a Country

```http
  DELETE /api/rest/manufacturer/deleteManufacturer
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `manufacturer_id` | `string`| Belirtilen üretici ID'sine sahip üreticiyi siler.     |


## API Endpoints for Order

The following API endpoints are available for managing order related data:

#### Get Order Details

```http
  GET /api/rest/order/getOrder
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `order_id`| `string` | Retrieves the details of the specified order.  |

#### Get List of Orders

```http
  GET /api/rest/order/getOrders
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `order_status` `orderby` `sort` `limit` `start_date` `end_date`|  `string` | Retrieves a list of all orders in the store..|


#### Get Order Products
```http
  GET /api/rest/order/getOrderProducts
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `order_id`| `string` | Retrieves the products associated with the specified order.  |

#### Get Order Options

```http
  GET /api/rest/order/getOrderOptions
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `order_id` `order_product_id` | `string`| Retrieves the options associated with the specified order.   |


#### Get Order Totals
```http
  GET /api/rest/order/getOrderTotals
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `order_id`| `string` | Retrieves the totals associated with the specified order.  |

#### Delete Order
```http
  DELETE /api/rest/order/deleteOrder
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `order_id`| `string` | Deletes the specified order. |

## API Endpoints for Product

The following API endpoints are available for managing product related data:

#### Get Product Details

```http
  GET /api/rest/product/getProduct
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `product_id`| `string` | Get details of the product with the specified ID.  |

#### Get Products

```http
  GET /api/rest/product/getProducts
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `status` `orderby` `sort` `limit` |  `string` | Get a list of all products in the store.|


#### Get Product Images
```http
  GET /api/rest/product/getProductImages
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `product_id`| `string` | Get a list of images for the product with the specified ID. |

#### Get Product Attributes

```http
  GET /api/rest/product/getProductAttributes
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `product_id` | `string`| Get a list of attributes for the product with the specified ID.   |


#### Get Product Options
```http
  GET /api/rest/product/getProductOptions
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `order_id`| `string` | Get a list of options for the product with the specified ID. |


#### Get Popular Products
```http
  GET /api/rest/product/getPopularProducts
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `limit`| `string` | Get a list of the most popular products in the store. |

#### Get Products By Category Id
```http
  GET /api/rest/product/getProductsByCategoryId
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `category_id` `status` `limit` `sort` `orderby`| `string` | Get a list of products in the specified category. |

#### Delete Product
```http
  DELETE /api/rest/product/deleteProduct
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `product_id`| `string` | Delete the product with the specified ID. |

## API Endpoints for Report

The following API endpoints are available for managing report related data:

#### Get Statistics

```http
  GET /api/rest/report/getStatistics
```

Retrieves store statistics.

## API Endpoints for Review

The following API endpoints are available for managing review related data:

#### Get Reviews By Product Id

```http
  GET /api/rest/review/getReviewsByProductId
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `product_id`| `string` | Retrieves all comments with the specified product ID. |

#### Get Total Reviews By Product Id

```http
  GET /api/rest/review/getTotalReviewsByProductId
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `product_id`| `string` | Returns the total number of reviews with the specified product ID. |

## API Endpoints for Whishlist

The following API endpoints are available for managing whishlist related data:

#### Get Reviews By Product Id

```http
  GET /api/rest/wishlist/getWishlist
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `customer_id`| `string` | Retrieves the wishlist of the customer with the specified customer ID. |

#### Get Total Reviews By Product Id

```http
  GET /api/rest/wishlist/getTotalWishlist
```

| Parameter   | Type     | Description                |
| :--------   | :------- | :------------------------- |
| `customer_id`| `string` | Returns the total number of wishlists for the customer with the specified customer ID. |


