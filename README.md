# 🌤️ App del Clima

Aplicación que consulta el clima actual de cualquier ciudad del mundo usando la API de [OpenWeatherMap](https://openweathermap.org/api).

**Demo en vivo:** [pega aquí tu link de Vercel/Netlify]

![Captura de la app](./screenshot.png)

## Funcionalidades

- Búsqueda de clima por nombre de ciudad
- Ciudades sugeridas de acceso rápido
- Muestra temperatura, sensación térmica, humedad, viento, presión y visibilidad
- Iconos propios en SVG que cambian según la condición climática (soleado, nublado, lluvia, nieve, niebla)
- Manejo de estados: carga, error (ciudad no encontrada) y datos de respaldo si no hay conexión con la API
- Diseño responsive y modo claro/oscuro automático

## Tecnologías

- HTML5, CSS3, JavaScript (ES6+)
- [OpenWeatherMap API](https://openweathermap.org/current) (REST, `fetch` + `async/await`)

## Cómo correrlo localmente

1. Clona el repositorio
   ```bash
   git clone https://github.com/tu-usuario/app-del-clima.git
   ```
2. Crea una cuenta gratuita en [OpenWeatherMap](https://home.openweathermap.org/users/sign_up) y copia tu API key
3. Abre `index.html` y pega tu key en la constante `API_KEY` al inicio del `<script>`
4. Abre el archivo en tu navegador

> **Nota:** Si no configuras una API key, la app funciona igual mostrando datos de demostración para un grupo de ciudades predefinidas (Bogotá, Madrid, Tokio, entre otras).

## Qué aprendí construyendo esto

- Consumo de APIs externas con `fetch` y manejo de respuestas asíncronas con `async/await`
- Manejo de errores de red y de datos (ciudad inexistente, falla de conexión) sin romper la experiencia del usuario
- Diseño de una interfaz que comunica claramente sus estados: cargando, error y éxito
- Por qué no se debe exponer una API key sensible en el frontend en un proyecto de producción real, y cómo se resolvería con un backend intermedio o variables de entorno en el servidor

## Posibles mejoras futuras

- Pronóstico extendido a 5 días
- Geolocalización automática del usuario
- Guardar ciudades favoritas

---

Proyecto creado como parte de mi portafolio de desarrollo frontend. [Ver portafolio completo](#)
