
## API Reference

#### Create item

```http
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

```http
  POST /v1/item/check
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `shop` | `integer` | **Required**. Your shop ID |
| `hash` | `string` | **Required**. Your shop hash |
| `id` | `amount` | **Required**. ID of item |

#### Delete item

```http
  POST /v1/item/delete
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `shop` | `integer` | **Required**. Your shop ID |
| `hash` | `string` | **Required**. Your shop hash |
| `id` | `amount` | **Required**. ID of item |

#### Edit item

```http
  POST /v1/item/edit
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `shop` | `integer` | **Required**. Your shop ID |
| `hash` | `string` | **Required**. Your shop hash |
| `name` | `string` | **Optional**. Name of item |
| `description` | `string` | **Optional**. Description of item |
| `amount` | `float` | **Optional**. Price of item |
