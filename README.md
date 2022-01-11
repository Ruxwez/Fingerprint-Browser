# Fingerprint-browser

Este paquete no necesita ninguna dependencia, sirve para obtener una huella dactilar única para cada navegador.

## Usage

Obtener Huella dactilar del navegador:  
```javascript

import fingerprintBrowser from 'fingerprint-browser';

const fingerprint = fingerprintBrowser();

console.log(fingerprint);

```

Options available:
- `WebGL`: habilitar el render con WebGL, este es 5 veces más lento pero añade otra capa de detección de hardware (por defecto es `false`)
- `debug`: Registra los datos utilizados para generar la huella dactilar en la consola (default `false`)

## Atención

- El factor de discriminación más fuerte es el token de canvas que no puede ser calculado en los dispositivos antiguos (por ejemplo: iPhone 6)
