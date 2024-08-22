
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
