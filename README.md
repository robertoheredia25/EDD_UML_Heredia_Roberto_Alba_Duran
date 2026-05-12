# 

# 

# Diagrama Actividad

Docente:Willman Acosta  
Fecha: 12/05/2026

**Tabla de Contenido:**

[**Fase 1: Investigación Técnica (40 minutos)	1**](#fase-1:-investigación-técnica-\(40-minutos\))

[**Fase 2: Modelado del Proceso de Compra (30 minutos)	3**](#fase-2:-modelado-del-proceso-de-compra-\(30-minutos\))

[**Fase 3: Entrega Profesional en GitHub (30 minutos)	3**](#fase-3:-entrega-profesional-en-github-\(30-minutos\))

# 

## **Fase 1: Investigación Técnica (40 minutos)** {#fase-1:-investigación-técnica-(40-minutos)}

**Tarea:** Antes de empezar el diseño, debemos documentarnos sobre la sintaxis específica de UML 2.5 para nodos de control. Lo importante aquí es distinguir entre una **decisión (rombo) y una bifurcación (barra de *fork*).**

**\-Nodo de decisión (decision node)**

Se representa mediante un rombo. Se utiliza cuando el flujo llega un punto donde debe elegir solamente un camino de entre varios que haya disponible

**\- Una bifurcación (barra de *fork*).**

Se representa con una barra ya sea horizontal o vertical se usa para dividir un flujo único en múltiples flujos que se ejecutan al mismo tiempo

**Fuentes de consulta mínimas obligatorias**:

1. **OMG (Object Management Group):** Consultar la especificación formal de UML en [https://www.omg.org/spec/UML/](https://www.omg.org/spec/UML/).  
2. **IBM Documentation:** "UML activity diagrams", 2021\. Disponible en: [https://www.ibm.com/docs/en/rhapsody/9.0.1?topic=diagrams-uml-activity](https://www.ibm.com/docs/en/rhapsody/9.0.1?topic=diagrams-uml-activity).  
3. **Visual Paradigm:** "UML Activity Diagram Tutorial". Disponible en: [https://www.visual-paradigm.com/guide/uml/what-is-activity-diagram/](https://www.visual-paradigm.com/guide/uml/what-is-activity-diagram/).

## 

## Fase 2: Modelado del Proceso de Compra (30 minutos) {#fase-2:-modelado-del-proceso-de-compra-(30-minutos)}

**Herramientas:** Draw.io (app.diagrams.net) o DIA.

**Escenario a modelar:**

Debéis representar el proceso de "Confirmación de Pedido" de una tienda online:

1. **Entrada:** El usuario pulsa "Finalizar compra".  
2. **Validación:** El sistema debe verificar simultáneamente el **Stock** y la **Validez de la Sesión**.  
3. **Pago:** Si ambos son correctos, se procede a la pasarela de pago segura.  
4. **Post-Pago (Concurrencia Crítica):** Si el pago es exitoso, el sistema debe ejecutar de forma paralela:  
   * Registro del pedido en la base de datos.  
   * Generación del PDF de la factura.  
   * Envío de notificación por correo electrónico.  
5. **Cierre:** Una vez finalizadas *todas* las tareas del punto anterior (Uso de *Join*), se muestra el mensaje de confirmación al cliente.

## Fase 3: Entrega Profesional en GitHub (30 minutos) {#fase-3:-entrega-profesional-en-github-(30-minutos)}

Un desarrollador profesional se define por cómo entrega su trabajo.

1. Crear un repositorio público en GitHub: EDD\_UML\_Apellido\_Nombre.  
2. Estructura del repositorio:  
   * /src: Archivo fuente del diagrama (.drawio o .dia).  
   * /img: Imagen exportada en alta resolución (PNG o SVG).  
   * README.md: Documento principal.

# 