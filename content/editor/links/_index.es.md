---
title: "Enlazando Registros/Recursos"
date: 2021-12-08
draft: false
weight: 110
authors: ["Katie Pearson"]
translators: ["Samanta Orellana"]
keywords: ["recursos genéticos","secuencias de ADN","secuencias","listados de especies","voucher","duplicados","ocurrencias asociadas"]
---

{{< notice info >}}
  Esta página describe cómo vincular ocurrencias asociadas, listados de especies, duplicados, o recursos genéticos con registros de ocurrencias.
{{</ notice >}}

Para vincular una ocurrencia con un recurso o registro externo (o interno), navegue a la página de editor de ocurrencias de ese registro (vea [esta página](https://biokic.github.io/symbiota-docs/es/editor/edit/) para instrucciones) y haga click en la pestaña de Recursos Enlazados.

![Linked Resources Tab](/symbiota-docs/images/linkedresourcestab.PNG)

### Enlazando ocurrencias asociadas

En el recuadro de Ocurrencias asociadas de la pestañña Recursos Enlazados, puede vincular una ocurrencia con (1) otra ocurrencia en el portal que está trabajando actualmente, (2) una ocurrencia en otro portal o base de datos, y/o (3) un registro observacional (sin voucher) de un taxon específico.

#### Enlazando una ocurrencia a un registro dentro del portal
1. Hacer click en el ícono del signo más en la casilla de Ocurrencias Asociadas para añadir un nuevo enlace.
2. Introducier el nombre del identificador (número de catálogo, otro número de catálogo, u occurrenceID/SymbiotaID) en la casilla **Identificador** para que la ocurrencia sea vinculada.  
3. Seleccione ya sea Números de Catálogo u PK de Ocurrencia de la lista desplegable **Objetivo para Búsqueda**, dependiendo de lo que ingresó en la casilla de **Identificador**. 
4. Seleccione la colección dentro del portal a la que la ocurrencia a ser vinculada pertenece (si aplica).
5. Haga click en el botón de Búsqueda.
6. Desde los resultados de la búsqueda, haga click en el botón circular a la izquierda de la ocurrencia a la que le gustaría enlazar la ocurrencia actual. 

{{< notice note >}}
  Puede hacer click en la porción subrayada en los resultados de búsqueda de ocurrencias, para ver la ocurrencia antes de vincularla.
{{</ notice >}}

![Create New Association Example](/symbiota-docs/images/createassociation.PNG)

7. Busque el campo de **Relaciones** en la parte inferior, y seleccione un término que describa la relación entre su ocurrencia y la ocurrencia que está siendo vinculada.

{{< notice note >}}
  Note que el **sujeto** del término de Relación corresponde a la ocurrencia que usted está editando actualmente, y que el **objeto** del término de Relación es la ocurrencia que va a ser vinculada. Por ejemplo, si se encuentra en la página de edición del registro 12345, debe utilizar la casilla de Ocurrencias Asociadas para encontrar el registro 54321, y seleccionar "partOf" (parte de) del menú desplegable, para que la relación sea registrada como "Registro 12345 es parte del registro 54321".
{{</ notice >}}

8. Selleccione un **Subtipo de Relación** (Relationship Subtype), y **Base del Registro** (Basis of Record) de los menús desplegables, si aplica. Agregue cualquier otra información en el campo de **Notas** (Notes). 
9. Si la relación que seleccionó fue hasHost (tiene hospedero) o hostOf (es hospedero de), introducir la información de **Ubicación en hospedero** (Location on host), de estar disponible.
10. Haga click en el botón Crear Asociación.

#### Enlazando un registro de ocurrencia en un portal o base de datos diferente
1. Haga click en el ícono de signo más en la ventana de Ocurrencias Asociadas para añadir un nuevo enlace. 
2. En la casilla de Ocurrencia Externa, ingrese el número de catálogo o algún otro identificadore del registro que está vinculando en la casilla **Identificador Externo** (External Identifier).
3. Ingrese una URL que pueda ser utilizada para acceder al registro que está vinculando en el campo **URL del Recurso** (Resource URL). Por ejemplo, aquí está la URL para un registro del Portal de Briophytas que puede ser ingresado: [https://bryophyteportal.org/portal/collections/individual/index.php?occid=4595185](https://bryophyteportal.org/portal/collections/individual/index.php?occid=4595185).
4. Complete los pasos 7-10 descritos anteriormente.

#### Enlazando una ocurrencia a una observación que no tiene un registro 
1. Haga click en el ícono del signo más en la casilla de Ocurrencias asociadas para añadir un nuevo enlace.
2. Introducir el nombre científico del taxón que tiene relación con su ocurrencia. 
3. Complete los pasos 7-10 descritos anteriormente.

### Enlazando una ocurrencia a un listado de especies
1. En la casilla  the **Checklist Voucher Linkages** box of the Linked Resources tab, select the checklist to which you would like to link you occurrence from the dropdown menu. Note that you will only see checklists for which you have editor or administrator permissions.

{{< notice note >}}
  To batch link vouchers to a checklist, see the [Adding Vouchers to Checklist page](https://biokic.github.io/symbiota-docs/user/checklist/voucher/).
{{</ notice >}}

### Linking an occurrence to a duplicate specimen
There are several ways to link an occurrence to duplicate specimens. You can:
* In the Linked Resource tab of the occurrence editor, click the Search for Records to Link button in the **Specimen Duplicates** box. This will open a search window that you can use to identify and link duplicate specimens. You can search according to collector name, collector number, date, catalog number, or occid (SymbiotaID) using this tool.
* In the main Occurrence Data tab of the occurrence editor, click the Duplicates button. This will search the portal for occurrences with the same collector last name, number, and date. If a potential identical duplicate is identified, you can check the box next to Link as Duplicate, then click Transfer All Fields or Transfer to Empty Fields Only to initiate the link. This will also transfer any data from that duplicate into your specimen record. Newly transferred data will be highlighted in blue.
* Batch link records to their duplicates using the [Duplicate Clustering tool](https://biokic.github.io/symbiota-docs/coll_manager/dup).

### Linking an occurrence to a genetic resource
In the **Genetic Resources** box of the Linked Resources tab, enter information about the genetic sequence associated with your occurrence in the provided fields. Be sure to provide a URL to the sequence. Here is an example for a URL from GenBank: [https://www.ncbi.nlm.nih.gov/nuccore/BV165924.1](https://www.ncbi.nlm.nih.gov/nuccore/BV165924.1).
