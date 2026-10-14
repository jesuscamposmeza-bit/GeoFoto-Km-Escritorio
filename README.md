# GeoFoto Km - Escritorio 🗺️📸
🛒 **¿Deseas adquirir este software?**  
[👉 HAZ CLIC AQUÍ PARA COMPRAR LA LICENCIA EN GUMROAD](https://jesusmeza.gumroad.com/l/GeoFoto-Km-Escritorio))
**GeoFoto Km** es una herramienta de software diseñada para ingenieros civiles, supervisores de obra, coordinadores de conservación y topógrafos. Automatiza por completo el proceso de renombrar lotes de fotografías geoetiquetadas, asignándoles su **cadenamiento (kilometraje) exacto** basándose en el eje de un archivo **DXF**.

El programa genera un archivo `.zip` con las fotos organizadas y un reporte detallado en Excel, ahorrándote horas de trabajo manual en gabinete.

---

## 🔥 Ventajas Principales

1. **Ahorro masivo de tiempo:** Olvídate de identificar y renombrar manualmente cada fotografía relacionándola con los planos. El programa lo hace en segundos.
2. **Eficiencia en campo:** Dedícate exclusivamente a capturar imágenes en el terreno; al regresar a la oficina, la herramienta procesará todo el lote automáticamente.
3. **Seguridad de datos:** Tus fotografías originales nunca se modifican ni se borran. El programa trabaja sobre copias y exporta todo en un archivo comprimido.

---

## 💻 Instalación y Requisitos

1. Descarga el archivo comprimido desde la sección de **Releases** de este repositorio.
2. Descomprime la carpeta en la ubicación de tu preferencia (por ejemplo, en *Documentos* o el *Escritorio*).
3. Entra a la carpeta llamada `dist`, donde encontrarás el archivo ejecutable (`.exe`).
4. Da doble clic sobre el ejecutable para iniciar la instalación.
5. Si Windows te solicita permisos de administrador diciendo *"¿Quieres permitir que esta aplicación haga cambios en el dispositivo?"*, selecciona **Sí/Confirmar**. El instalador es **100% seguro y funcional**.

---

## 🛠️ Guía de Uso Paso a Paso

### Paso 1: Ejecutar el programa
Al abrir la aplicación, verás una interfaz limpia y organizada dividida en secciones para cargar tus datos:
![Interfaz Inicial](https://github.com)

### Paso 2: Seleccionar el archivo del Eje (DXF)
Haz clic en el botón **Buscar...** de la sección 1 para seleccionar el archivo vectorial con el eje de tu vía.
![Selección del DXF](https://github.com)

### Paso 3: Lectura automática de datos
Una vez seleccionado el archivo, el sistema detecta de forma automática la capa del eje, la longitud del tramo, el número de vértices y el cadenamiento inicial (por ejemplo: `0+000.000`).
![Eje Cargado](https://github.com)

### Paso 4: Cargar tus fotografías
Haz clic en **Carpeta...** o **Archivos...** en la sección 2. Selecciona el directorio que contiene todas las imágenes capturadas en campo (el sistema leerá automáticamente las subcarpetas). El contador indicará cuántas fotos fueron seleccionadas correctamente.
![Fotos Cargadas](https://github.com)

### Paso 5: Configurar opciones y procesar
Ajusta los parámetros en la sección 3 (Prefijo de nombre o distancia máxima de tolerancia al eje en metros). Luego, presiona el botón **4. Procesar y guardar .zip**, el cual te solicitará elegir la ruta y el nombre del archivo comprimido de salida.
![Guardar Archivo](https://github.com)

### Paso 6: ¡Proceso completado!
Una barra de progreso verde te mostrará el avance en tiempo real analizando los metadatos de las imágenes. Al finalizar, el programa te confirmará el éxito de la tarea y te ofrecerá abrir directamente la carpeta contenedora.
![Proceso Terminado](https://github.com)

---

## 📦 El Antes y el Después (Resultados en el .zip)

### Antes del procesamiento:
Las fotos de las cámaras o dispositivos móviles suelen tener nombres genéricos basados en la fecha y la hora (`TimePhoto_YYYYMMDD_HHMMSS.jpg`), imposibles de clasificar rápidamente.
![Fotos Originales](https://github.com)

### Después del procesamiento (Resultado final):
El programa procesa las coordenadas y renombra cada archivo con su **cadenamiento correspondiente sin decimales** (ej. `7+529.jpg`, `11+198.jpg`). Si dos o más fotos coinciden en el mismo metro exacto, el sistema las enumera de forma automática (`9+425_2.jpg`).
![Fotos Renombradas](https://github.com)

Además, la herramienta genera de forma automática:
*   **Carpeta `REVISAR_LEJOS_DEL_EJE\`:** Para las fotos que superaron el límite de distancia configurado.
*   **Carpeta `SIN_COORDENADAS\`:** Para las fotos que no contaban con metadatos de ubicación.
*   **`reporte_cadenamientos.xlsx`:** Un archivo de Excel completo que detalla: nombre original, coordenadas exactas, cadenamiento asignado, distancia métrica al eje, lado de la vía (Izquierda/Derecha) y el origen de la coordenada.

---

## ⚠️ Recomendaciones Importantes

* **Habilita el GPS:** Asegúrate de tener activada la función de ubicación/GPS en tu dispositivo móvil o cámara antes de tomar las fotos en campo.
* **Calidad Original:** Transfiere las fotos a tu computadora usando un cable USB, Google Drive o la aplicación "Archivos". 
* **NO uses WhatsApp:** Esta aplicación comprime las imágenes y **elimina por completo los metadatos GPS ocultos**. Si usas fotos de WhatsApp, el programa solo podrá leer el texto impreso de la imagen (si la app de tu cámara lo añade), lo cual reduce la precisión del metraje.
