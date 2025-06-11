# pkg-estadistica-js

pkg-estadistica-js is a js library.

## Installation

Use the package manager [npm](https://github.com/olajer/pkg-estadistica-js) to install pkg-estadistica-js.

```bash
npm install @olajer/pkg-estadistica-js@1.0.1
```

## Usage

```javascript
const { promedio, desviacionEstandar } = require('@olajer/pkg-estadistica-js/estadisticas');
const { generarGrafico } = require('@olajer/pkg-estadistica-js/graficas');


const datos = [12, 25, 33, 48, 60];
const etiquetas = ['Ene', 'Feb', 'Mar', 'Abr', 'May'];

# returns 'Promedio'
console.log('Promedio:', promedio(datos));

# returns 'Desviación estándar'
console.log('Desviación estándar:', desviacionEstandar(datos));

# returns 'chart'
generarGrafico('./public/grafica.png', etiquetas, datos).then(() => {
    console.log('Gráfica generada exitosamente.');
});
```

## Demo
[TEST PROJECT](https://github.com/olajer/demo-pkg)

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)