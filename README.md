# ⚡ Parámetros de Secuencia – Líneas Aéreas

Aplicación de escritorio desarrollada en **Python** para el cálculo y análisis de parámetros eléctricos de líneas aéreas de transmisión.

Permite definir la geometría de los conductores y cables de guarda, calcular matrices de impedancia y susceptancia, obtener parámetros de secuencia y generar automáticamente un **reporte técnico en PDF** con los resultados.

---

## Características

- Cálculo de parámetros eléctricos de líneas aéreas.
- Configuración de **uno o dos circuitos**.
- Soporte para conductores de fase y cables de guarda.
- Configuración de subconductores por fase.
- Representación de haces de conductores.
- Definición de coordenadas `x / h` de cada conductor.
- Consideración de resistividad del terreno.
- Cálculo de impedancias de fase.
- Transformación a componentes simétricas.
- Cálculo de impedancias de secuencia.
- Matriz reducida `Zabc`.
- Cálculo de susceptancias.
- Visualización gráfica de la geometría de la estructura.
- Desarrollo detallado de los cálculos.
- Generación automática de **reportes PDF**.
- Aplicación independiente de Excel.

---

## Resultados disponibles

La aplicación organiza los resultados mediante diferentes pestañas:

### Resultados clave

Presenta los principales parámetros eléctricos obtenidos para la línea.

### Impedancia de secuencia Z012

Muestra las impedancias correspondientes a las componentes:

- Secuencia cero `Z0`
- Secuencia positiva `Z1`
- Secuencia negativa `Z2`

### Impedancia reducida Zabc

Presenta la matriz de impedancia reducida de las fases después de realizar las reducciones correspondientes.

### Susceptancia de secuencia

Entrega los parámetros asociados a la capacitancia y susceptancia de la línea.

### Desarrollo de cálculos

Incluye el procedimiento y los valores intermedios utilizados para obtener los resultados finales.

Esta sección permite revisar y verificar el desarrollo matemático realizado por el programa.

### Geometría de la estructura

Representa gráficamente la disposición física de los conductores.

La visualización incluye:

- Conductores de fase.
- Cables de guarda.
- Circuitos de la línea.
- Coordenadas horizontales `x`.
- Alturas `h`.
- Eje central de la estructura `x = 0`.
- Número de subconductores.
- Separación del haz.
- RMG individual.
- RMG equivalente del haz.

Esto facilita la revisión visual de la configuración antes de interpretar los resultados eléctricos.

### Notas

Espacio destinado a información adicional relacionada con el cálculo o la configuración utilizada.

---

## Reporte PDF

El programa permite generar directamente un **reporte técnico en PDF** desde la aplicación.

El reporte incorpora información de las principales pestañas:

- Resultados clave
- Impedancia de secuencia Z012
- Impedancia reducida Zabc
- Susceptancia de secuencia
- Desarrollo de cálculos
- Geometría de la estructura
- Notas

La sección de geometría incorpora el esquema de la estructura junto con el resumen de conductores y sus parámetros.

---

## Tecnologías utilizadas

El proyecto está desarrollado principalmente con:

- **Python**
- **Tkinter** para la interfaz gráfica
- **NumPy** para operaciones numéricas y matriciales
- **Matplotlib** para representación gráfica
- **ReportLab** para generación de reportes PDF
- **PyInstaller** para generar la aplicación ejecutable

---

## Instalación

Clona el repositorio:

```bash
git clone <URL-DEL-REPOSITORIO>
cd <NOMBRE-DEL-REPOSITORIO>
```

Instala las dependencias:

```bash
pip install numpy matplotlib reportlab pyinstaller
```

Luego ejecuta:

```bash
python ParametrosSecuencia.py
```

---

## Generar el ejecutable

El proyecto incluye:

```text
CREAR_EXE.bat
```

Ejecuta este archivo en Windows para instalar las dependencias necesarias y generar la versión ejecutable mediante **PyInstaller**.

El ejecutable generado permite utilizar la aplicación sin necesidad de iniciar manualmente el script de Python.

---

## Flujo de trabajo

1. Seleccionar la configuración de la línea.
2. Ingresar los parámetros eléctricos de los conductores.
3. Definir las coordenadas `x` y `h`.
4. Configurar circuitos y subconductores.
5. Definir los parámetros del terreno.
6. Ejecutar el cálculo.
7. Revisar los resultados.
8. Verificar gráficamente la geometría de la estructura.
9. Generar el reporte PDF.

---

## Aplicaciones

La herramienta puede utilizarse como apoyo para:

- Estudios eléctricos de líneas de transmisión.
- Cálculo de parámetros de secuencia.
- Modelación de líneas aéreas.
- Preparación de datos para estudios de sistemas eléctricos.
- Verificación de geometrías de estructuras.
- Documentación técnica de cálculos.

---

## Advertencia

Los resultados entregados por esta aplicación deben ser revisados por un profesional competente antes de utilizarse en estudios, diseños, especificaciones o decisiones de ingeniería.

El software constituye una herramienta de apoyo al cálculo y no reemplaza la revisión técnica del ingeniero responsable.

---

## Autor

**Víctor Marcelo Alvarez Catalán**

Proyecto desarrollado como herramienta de ingeniería para el cálculo y análisis de parámetros eléctricos de líneas aéreas de transmisión.

---

## Licencia

Revisa el archivo `LICENSE` del repositorio para conocer las condiciones de uso, modificación y distribución del software.
