
# Ascory documentation

This documentation will help in mastering the basic API for working with Ascory


## API Reference

#### Create item

```
  POST /v1/item/create
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `shop` | `integer` | **Required**. Your shop ID |
| `hash` | `string` | **Required**. Your shop hash |
| `name` | `string` | **Required**. Name of item |
| `description` | `string` | **Required**. Description of item |
| `amount` | `float` | **Required**. Price of item |

#### Check item

```
  POST /v1/item/check
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `shop` | `integer` | **Required**. Your shop ID |
| `hash` | `string` | **Required**. Your shop hash |
| `id` | `amount` | **Required**. ID of item |

#### Delete item

```
  POST /v1/item/delete
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `shop` | `integer` | **Required**. Your shop ID |
| `hash` | `string` | **Required**. Your shop hash |
| `id` | `amount` | **Required**. ID of item |

#### Edit item

```
  POST /v1/item/edit
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `shop` | `integer` | **Required**. Your shop ID |
| `hash` | `string` | **Required**. Your shop hash |
| `id` | `amount` | **Required**. ID of item |
| `name` | `string` | **Optional**. Name of item |
| `description` | `string` | **Optional**. Description of item |
| `amount` | `float` | **Optional**. Price of item |

#### All items

```
  POST /v1/item/all
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `shop` | `integer` | **Required**. Your shop ID |
| `hash` | `string` | **Required**. Your shop hash |

#### Create invoice

```
  POST /v1/invoice/create
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `shop` | `integer` | **Required**. Your shop ID |
| `hash` | `string` | **Required**. Your shop hash |
| `item` | `integer` | **Required**. ID of item |
| `comment` | `string` | **Optional**. Comment of invoice |
| `backURL` | `string` | **Optional**. Back URL of invoice |
| `successURL` | `string` | **Optional**. Success URL of invoice |
| `failURL` | `string` | **Optional**. Fail URL of invoice |

#### Check invoice

```
  POST /v1/invoice/check
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `shop` | `integer` | **Required**. Your shop ID |
| `hash` | `string` | **Required**. Your shop hash |
| `id` | `amount` | **Required**. ID of invoice |

#### All invoice

```
  POST /v1/invoice/all
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `shop` | `integer` | **Required**. Your shop ID |
| `hash` | `string` | **Required**. Your shop hash |

#### Payment detail

```
  POST /v1/payment/detail
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `integer` | **Required**. ID of invoice |
| `hash` | `string` | **Required**. Hash of invoice |

#### Payment confirm

```
  POST /v1/payment/confirm
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `integer` | **Required**. ID of invoice |
| `hash` | `string` | **Required**. Hash of invoice |
| `email` | `string` | **Required**. Email of payment |
| `method` | `string` | **Required**. Method of payment |
