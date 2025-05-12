## 🌤️ Datos de una Torre Meteorológica

Cada torre meteorológica manejará distintos tipos de datos, agrupados en categorías para facilitar su gestión, visualización y almacenamiento.

---

### 🧾 Identificación de la Torre

| Campo              | Tipo        | Descripción                                 |
|-------------------|-------------|---------------------------------------------|
| `id_torre`         | UUID / int  | Identificador único de la torre             |
| `nombre`           | string      | Nombre asignado a la torre                  |
| `ubicacion`        | string / JSON | Dirección o coordenadas (`lat`, `lon`)     |
| `usuario_asignado` | int / UUID  | ID del usuario encargado (opcional)         |
| `estado`           | string      | Estado actual: Activa / Inactiva / Falla / Mantenimiento |

---

### 📡 Datos Meteorológicos en Tiempo Real

| Campo                | Tipo     | Unidad       | Descripción                           |
|---------------------|----------|--------------|---------------------------------------|
| `temperatura`        | float    | °C           | Temperatura ambiental                 |
| `humedad_relativa`   | float    | %            | Porcentaje de humedad relativa        |
| `presion_atmosferica`| float    | hPa          | Presión atmosférica                   |
| `velocidad_viento`   | float    | m/s          | Velocidad del viento                  |
| `direccion_viento`   | int      | grados (°)   | Dirección del viento (0-360°)         |
| `precipitacion`      | float    | mm/h         | Intensidad de la lluvia               |
| `radiacion_solar`    | float    | W/m²         | Radiación solar                       |
| `indice_uv`          | int      | índice (0-11+)| Índice UV                             |

---

### 🧭 Datos Técnicos / Diagnóstico

| Campo                     | Tipo     | Descripción                                    |
|--------------------------|----------|------------------------------------------------|
| `nivel_bateria`          | float    | Porcentaje de batería restante                |
| `tiempo_ultima_conexion` | datetime | Última vez que la torre se comunicó           |
| `estado_sensor_temperatura` | string | Estado del sensor de temperatura (OK/Error)   |
| `estado_sensor_humedad`     | string | Estado del sensor de humedad (OK/Error)       |
| `estado_general`            | string | Normal / Alerta / Crítico                     |

---

### 📁 Datos Administrativos

| Campo                  | Tipo     | Descripción                                   |
|-----------------------|----------|-----------------------------------------------|
| `fecha_creacion`      | datetime | Fecha de creación de la torre                 |
| `ultima_actualizacion`| datetime | Último momento en que se actualizó la torre   |
| `notas`               | text     | Comentarios u observaciones adicionales       |
| `origen_datos`        | string   | Fuente: `simulador`, `excel`, o `manual`      |
