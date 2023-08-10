
![badge](Imagenes/Logo_estratego_horneg.webp)

# Manual Reporte Masivos

## Indice

- [Manual Reporte Masivos](#manual-reporte-masivos)
  - [Indice](#indice)
  - [1. Recursos](#1-recursos)
    - [Aliados de trabajo y herramientas](#aliados-de-trabajo-y-herramientas)
    - [Fuentes de trabajo](#fuentes-de-trabajo)
    - [Dimensión de variables](#dimensión-de-variables)
  - [2. Herramientas](#2-herramientas)
    - [Botón de ayuda](#botón-de-ayuda)
    - [Filtro relacional](#filtro-relacional)
  - [3. Indicadores tarjetas](#3-indicadores-tarjetas)
  - [4. SMS-Resumen Mensual](#4-SMS-resumen-mensual)
    - [Indicadores gráficos](#indicadores-gráficos)
    - [Resultado por Encargado de Envío](#resultado-por-encargado-de-envío)
    - [$ Capital Gestionado Vs % Efectividad Pago](#-capital-gestionado-vs-efectividad-pago)
    - [% Participación por filas de SMS mora inicial vs final](#-participación-por-filas-de-SMS-mora-inicial-vs-final)
    - [% Efectividad pago score](#efectividad-pago-score)
  - [5. Bots-Resumen Mensual](#5-Bots-resumen-mensual)
    - [Indicadores gráficos Bots](#indicadores-gráficos-Bots)
    - [Resultados por Encargado Envío Bots](#resultados-por-encargado-envío-Bots)
    - [$ Capital Gestionado Vs %Efectividad Pago Bots](#-capital-gestionado-vs-efectividad-pago-Bots)
    - [% Participación por filas de SMS mora inicial vs final Bots](#-participación-por-filas-de-SMS-mora-inicial-vs-final-Bots)
    - [% Efectividad pago Score Bots](#efectividad-pago-score-Bots)
  - [6. SMS - Campañas Diarias](#6-SMS---campañas-diarias)
    - [% Pago Día](#-pago-día)
  - [7. Bots - Campañas Diarias](#7-Bots---campañas-diarias)
    - [% Pago Día Bots](#-pago-día-Bots)
  - [8. Contacto](#8-contacto)

## 1. Recursos

### Aliados de trabajo y herramientas

![Imagenes/aliadosyherramientas.png](Imagenes/aliadosyherramientas.png)

[Indice](#indice)

### Fuentes de trabajo

![Imagenes/fuentesdetrabajo.png](Imagenes/fuentesdetrabajo.png)

[Indice](#indice)

### Dimensión de variables

- Optimización de intervalos, focos y prácticas de gestión y ejecución por temporalidades.

- Descripción de variables de ejecución, comportamiento y otros factores de la gestión en controlnext

- Medición y retroalimentación de focos, gestores y canales de mayor eficiencia y efectividad (comportamiento variables Score asignación C-Universe).

![Imagenes/dimensiondevariables.png](Imagenes/dimensiondevariables.png)

[Indice](#indice)

## 2. Herramientas

### Botón de ayuda

Se realiza la creación de marcadores por medio de botones para facilitar la interpretación de indicadores y generar un acceso más rápido a la sección de filtros que se encuentra oculta para una mejor visualización de los datos.

![Imagenes/botondeayuda.png](Imagenes/Botonesmasivos.png)

[Indice](#indice)

### Filtro relacional

**- Primer Recuadro:** Este filtro está habilitada para vistas en específico como lo son las campañas diarias que se envían tanto de SMS como de CallBotss, se podrá seleccionar diferentes tipos de rangos sea por meses, semanas o días. Por ejemplo: De meses se puede seleccionar la opción “Último”, igualmente se puede seleccionar la opción “Este” para referenciar fecha o mes actual. Evitar usar la opción “Siguiente” ya que la información que se almacena es día vencido.

**- Segundo Recuadro:** Escribiendo un número se podrá seleccionar la temporalidad a consultar.

**- Tercer Recuadro:** Preferiblemente seleccionar la opción “Meses”, aunque igualmente se pueden referenciar otras temporalidades.

![Imagenes/filtrorelacional.png](Imagenes/filtrosmasivos.png)

[Indice](#indice)

## 3. Indicadores tarjetas

![Imagenes/medicion1.png](Imagenes/Tarjetasmasivosms.png)

**- Total Mensajes:** Total mensajes enviados (un mensaje debe tener máximo 60 caracteres, desde el carácter 61 se contará como uno nuevo).

**- Total Gestiones:** Total de gestiones por dato del cargue.
  
**- Créditos Gestionados:** Total de créditos gestionados en el mes en curso.
  
**- Créditos Contacto Causado:**  Créditos que generaron contacto entre los 3 días siguientes al envió del cargue.
  
**- Créditos Pago Causado:** Créditos que generaron pago en los 3 días siguientes al envió del cargue.

![Imagenes/medicion1.png](Imagenes/Tarjetasmasivosbots.png)
  
**- Gestiones:** Total gestiones realizadas por cargue (se cuenta por dato).

**- Créditos Gestiones:** Total de créditos únicos gestionados por cargue.
  
**- Total Tono:** Se entiende cuando se marca y timbra 4 veces (teléfono es útil)
  
**- Total Contacto:** Es la confirmación del titular cuando se solicita la verificación de su identidad en el CallBots.

**- Total Acuerdos:** Créditos con Promesa de pago en llamada.

[Indice](#indice)

## 4. SMS-Resumen Mensual

![Imagenes/gestionporalivioyvehiculo.png](Imagenes/indicadoresmsresumen.png)

### Indicadores gráficos

**- Intensidad Gestión:** Intensidad de SMS que se envían por créditos (teléfonos/créditos).

**- %Efectividad Contacto:** Posibles contactos que se fomentaron por él envió de los SMS, debido a que se tipifico como contacto entre los siguientes 3 días del envió.
  
**- %Efectividad Acuerdo:** Posibles acuerdo que se fomentó por él envió de los SMS ya que se tipifico como promesa de pago entre los siguientes 3 días del envió.
  
**- %Efectivcidad pago Cuota:** Posibles pago que se fomentó por él envió de los SMS ya que se realizó entre los siguientes 3 días del envió.

### Resultado por Encargado de Envío

Grafica de barras donde se podrán visualizar 4 indicadores (gestión, contacto, negociación y pago) según los encargados de cada envió.

### $ Capital Gestionado Vs % Efectividad Pago

Se puede visualizar en esta grafica agrupada de columnas y líneas el valor capital gestionado comparado con el porcentaje de efectividad de pago por cada uno de los encargados de los cargues.
### % Participación por filas de SMS mora inicial vs final 

En esta matriz se podrá visualizar el porcentaje de participación de los SMS según el rango de mora inicial comparado con la mora final.

### % Efectividad pago Score

Porcentaje de efectividad del posible pago que se tuvieron de los SMS según la participación por cada uno de los tipos de riesgo.

[Indice](#indice)

## 5. Bots-Resumen Mensual

![Imagenes/gestionporalivioyvehiculo.png](Imagenes/indicadoresmsresumenbot.png)

### Indicadores gráficos Bots

**- % Efectividad Tono:** Total gestiones realizadas por cargue (se cuenta por dato).

**- % Efectividad Contacto:** Total de créditos únicos gestionados por cargue.
  
**- % Efectividad Acuerdo:** Se entiende cuando se marca y timbra 4 veces (teléfono es útil).
  
**- % Efectivcidad pago Cuota:** Es la confirmación del titular cuando se solicita la verificación de su identidad en el CallBots.

### Resultados por Encargado Envío Bots

Grafica de barras donde se podrán visualizar 4 indicadores (Total Tono, Total contacto, acuerdo y pago) según los encargados de cada envió.

### $ Capital Gestionado Vs %Efectividad Pago Bots

Se puede visualizar en esta grafica agrupada de columnas y líneas el valor capital gestionado comparado con el porcentaje de efectividad de pago por cada uno de los encargados de los cargues.

### % Participación por filas de SMS mora inicial vs final Bots

En esta matriz se podrá visualizar el porcentaje de participación de los SMS según el rango de mora inicial comparado con la mora final.

### % Efectividad pago Score Bots

Porcentaje de efectividad del posible pago que se tuvieron de los SMS según la participación por cada uno de los tipos de riesgo.

[Indice](#indice)

## 6. SMS - Campañas Diarias

![Imagenes/gestionasesorporasesor.png](Imagenes/smscampañasdiarias.png)

**- Filtro por indicadores temporales:** Línea de tiempo por meses, días o semanas esta puede ser modificada para seleccionar un campo específico de días que no interrumpa el espacio entre tablas dinámicas.

**- Filtro por Encargados de Envió:** Se puede filtrar la información para mostrar solo los cargues de coordinador o encargado de envío que se requiera.

- **Campaña:** Nombre de la campaña que se carga, se puede evidenciar que la estructura del nombre está conformada por fecha y encargado del cargue.
  
- **Mensajes:** Cuantos SMS salieron del cargue seleccionado.
  
- **Créditos:** Cantidad de titulares que se relacionan en la base para envió de SMS.
  
- **$ Cuota:** Valor vencido a la fecha del cargue.
  
- **Teléfonos:** Cantidad de teléfonos a los que se les enviaran los SMS.
  
- **% Intensudad:** Intensidad de SMS que se envían por créditos (teléfonos/créditos).
  
- **Contactos:** Posible contacto que se fomentó por él envió de los SMS ya que se realizó entre los 3 días siguientes al envió.
  
- **% Contacto:** Porcentaje de contacto según el indicador anterior (contacto/créditos).
  
- **Acuerdos:** Posible promesa de pago que se fomentó por él envió de los SMS ya que se realizó entre los 3 días siguientes al envió.
  
- **% Acuerdo:** Porcentaje de promesas de pago según el indicador anterior (acuerdos/créditos).
  
- **Crédito Pago:** Posible cantidad de créditos que pagaron fomentados por él envió de los SMS ya que se realizó entre los 3 días siguientes al envió.
  
- **$ Mensajes Costo:** Costo del cargue (cantidad de SMS enviados * el costo unitario).
  
- **$ Cuota Pago:** Posible valor de pagos que se fomentó por él envió de los SMS ya que se realizó entre los 3 días siguientes al envió.
  
- **% Pago Cuota:** Porcentaje de pagos según el indicador anterior (valor del pago que realizaron/valor vencido a la fecha del cargue).

#### % Pago Día

En este grafico de termómetro podremos visualizar como está el porcentaje de pago al día.

[Indice](#indice)

## 7. Bots - Campañas Diarias

![Imagenes/gestionasesorporcanalyfranja.png](Imagenes/botcampañasdiarias.png)

**- Filtro por indicadores temporales:** Línea de tiempo por meses, días o semanas esta puede ser modificada para seleccionar un campo específico de días que no interrumpa el espacio entre tablas dinámicas.

**- Filtro por Encargados de Envió:** Se puede filtrar la información para mostrar solo los cargues de coordinador o encargado de envío que se requiera.

- **Campaña:** En este grafico de termómetro podremos visualizar como está el porcentaje de pago al día.
- **Créditos Gestionados:** Cantidad de créditos cargados por campaña. 
- **Cuota Gestionados:** Valor vencido a la fecha.
- **Duración Conversación:** Tiempo en llamada por las diferentes líneas (segundos).
- **Gestiones:** Gestiones de los teléfonos cargados por cada campaña (se tienen en cuenta las remarcaciones).
- **Tono:** Se entiende cuando se marca y timbra 4 veces (teléfono es útil).
- **Contactos:** Es la confirmación del titular cuando se solicita la verificación de su identidad en el CallBots.
- **% Contactos:** Porcentaje del contacto según indicador anterior (contacto/total tono).
- **Acuerdo:** Créditos con promesa de pago en llamada.
- **% Acuerdo:** Porcentaje de créditos con promesa de pago según indicador anterior (negociaciones/contactos).
- **Crédito Pago:** Cantidad de créditos que se les brindo la información por el canal del BOT y después de esta gestión pagaron en el transcurso del mes.
- **Cuota Pago:** Valor total de los créditos del indicador anterior que pagaron después de brindarse la información por el canal del BOT y pagaron en el transcurso del mes.
- **% Pago Cuota:** Porcentaje de pagos según el indicador anterior (valor del pago que realizaron/valor vencido).

#### % Pago Día Bots

En este grafico de termómetro podremos visualizar como está el porcentaje de pago al día.
  
[Indice](#indice)

## 8. Contacto

Para sugerencias, dudas o peticiones contactar a el siguiente correo:

*turbot.ia@finanzauto.com.co*




                                                    2023 © Estratego