## generateToRupiah Documentation

### Overview
The `generateToRupiah` function is used to generate random product data and save it to a JSON file. It takes a single parameter `total`, which specifies the number of products to generate.

### Syntax
```javascript
generateToRupiah(total)
```

### Parameters
- `total`: The number of products to generate. Must be a positive integer.

### Return Value
An array of objects representing the generated products. Each object contains the following properties:
- `id`: The unique identifier of the product.
- `name`: The name of the product.
- `price`: The price of the product in Indonesian Rupiah (IDR).
- `category`: The category of the product.
- `priceFormatted`: The formatted price of the product in Indonesian Rupiah (IDR).

### Usage
```javascript
import { generateToRupiah } from './path/to/generateToRupiah.js';

// Generate 10 products
const products = generateToRupiah(10);
```

### Example
```javascript
import { generateToRupiah } from './path/to/generateToRupiah.js';

// Generate 5 products
const products = generateToRupiah(5);

console.log(products);
// Output:
// [
//   {
//     id: 1,
//     name: 'Product 1',
//     price: 87,
//     category: 'Electronics',
//     priceFormatted: 'Rp 87'
//   },
//   {
//     id: 2,
//     name: 'Product 2',
//     price: 55,
//     category: 'Clothing',
//     priceFormatted: 'Rp 55'
//   },
//   ...
// ]
```

### File Output
The generated product data will be saved to a JSON file named `products.json`.

### Error Handling
If an error occurs while writing the file, an error message will be logged to the console.

### Lisensi
[MIT](https://github.com/Amarudinn/generate-to-rupiah/blob/main/LICENSE.txt)