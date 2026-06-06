# Diseño

## [Usability 101: Introduction to Usability by Jakob Nielsen](https://www.nngroup.com/articles/usability-101-introduction-to-usability)

### Definición de *usabilidad* 

- Es un **atributo de calidad**.
- Compuesto por los siguientes **componentes de calidad**:
  - **Capacidad aprendizaje**: *¿Qué tan fácil es para usuario realizar las tareas básicas en su primer uso del sistema?*.
  - **Eficiencia**: Una vez aprendido. *¿Qué tan rápido puede el usuario realizar lo que quiere?*.
  - **Memorabilidad**: Al volver a utilizarlo tras un tiempo. *¿Qué tan fácil es recuperar eficacia en su uso?*.
  - **Errores**: *¿Qué errores usuario comete al utilizarlo?¿Cuántos?¿Con qué frecuencia?¿Qué tan fácil es recuperarse de ellos?*.
  - **Satisfacción**: *¿Que tan satisfactorio es el diseño y su uso?*.
- Es buena práctica destinar al menos $10%$ del presupuesto del producto a la *usabilidad*. No tomarlo como una regla fija, sino como una idea de que es un aspecto importante.

#### ¿Cómo mejorarla?

- Testeando con usuarios:
  - Pequeño grupo representativo de a quienes está orientado el producto o quienes lo usarán. Que sea un grupo reducido permite ahorrar costos y destinarlos a realizar más de estos test a lo largo del proceso de diseño.
  - Asignarles tareas a realizar con el producto.
  - No explicar ni intervenir.
  - Ver qué hacen y dónde encuentran dificultades.
- Realizar varios de estos test a medida que se va modificando el diseño, es decir hay que aplicar **diseño iterativo**
- **Evitar *focus groups*** (sesiones donde se trae usuarios para charlar sobre la interfaz de uso del producto). Es mejor *observar* cómo lo usan a *escuchar* y hacerles preguntas.

#### ¿En qué parte del proceso de desarrollo la ponemos?

- **En cada etapa** debemos **proponer variantes (*prototipos*)** y **testearlas** para solo avanzar sobre que reporte mayor *usabilidad*. Si lo dejás para cuando ya tenés producto final, realizar cambios es mucho más costoso.
- Al **iniciar el proceso de desarrollo**: Testear diseño previo para ver sus *puntos fuertes y débiles*.
- Testear interfaces de los competidores para aprender de otros diseños. Se recomiendo leer **intranet design annual*.
- Modificar ***prototipos*** en base a resultados de *tests*. Estos deben ser descartables y baratos.
- **Observar** usuario utilizándolo en su *habitat natural*.
- Testear producto final también porque *fases de implementación* suelen degradar **UX**.
- Definir *guías de usabilidad* a seguir durante el proceso.

### Definición de *útil*

- Es un **atributo de calidad**.
- *¿El producto hace lo que los usuarios necesitan?*.

### Definición de *utilidad*

- *Provee las herramientas necesarias* (**útil**) & es fácil y placentero de usar (**usable**).

## [The Definition of User Experience (UX) by Norman & Nielsen](https://www.nngroup.com/articles/definition-user-experience)

- **UI** es solo una parte de la **UX**.
- La **usabilidad** es atributo de calidad de la **UI**.
- **UX** comprende todos los aspectos de la interacción del usuario con la compañía, sus servicios y productos.

## [10 heurísticas de Nielsen sobre UX](https://www.ux-guidelines.com/nielsen.html)

- **Feedback**: *Visibilidad del estado del sistema*
  - El **sistema debe mantener constantemente informado al usuario sobre lo que está haciendo**.
  - Especialmente en acciones de larga duración, formularios o carga/descarga de archivos.
  - Mostrar progreso, tiempo y estado.
  - Más información permite elegir mejor próxima acción, da a usuario sensación de control y confianza.
  - Siempre informar si interacción resultó exitosa o no. Así evitar duda de si la realizó correctamente, si sistema anda bien, etc.
- **Familiaridad**: *Comunicación con el usuario debe ser con lenguaje familiar para él y del mundo real. Evitar tecnicismos y vocabulario del sistema*.
  - "Trash" en vez de "Removed entities".
  - Especialmente en labels, botones, íconos y mensajes de error.
  - No entender en lenguaje de un sitio hace al usuario sentirse inseguro e ignorado. Probablemente busque otro en vez de buscar su significado.
  - Al representar digitalmente objetos que tienen sus semejantes en la vida real, debemos permitir al usuario interactuar con este del mismo modo, ya que mentalmente se hizo una idea de cómo funciona basándose en el objeto real. Por ejemplo una app de reloj que cambia su horario girando manecillas.
- **Reversibilidad**: *Ofrecer siempre una opción de salida o undo/redo de la última acción ya que usuario suele cometer errores*.
  - Nunca dejar caminos sin salida o retorno.
  - Siempre ofrecer opción de *undo* o de salir.
  - Las opciones que podemos ofrecer son:
    - *Back*: Ir a pantalla previa.
    - *Cancel*: Cancelar tarea actual o proceso de múltiples pasos. En caso de pérdida de progreso informar y solicitar confirmación.
    - *Close*: Cerrar view.
    - *Undo*: Deshacer última acción.
  - Botones de salida fáciles de encontrar.
  - Se recomienda no abrir links en nuevas pestañas porque deja de funcionar el botón de atrás del browser.
  - Si se muestra un dialog, este no debe ocupar toda la pantalla haciendo creer a usuario que está en otro sitio. Además si este presiona botón de ir hacia atrás en navegador, debe tener misma funcionalidad que nuestro botón de cerrar el dialog.
  - Usar 'X' tiene significado ambiguo, puede ser cancelar o cerrar. Aclararlo o evitarlo.
  - Si usuario puede realizar múltiples acciones en poco tiempo soportar múltiples *undo/redo*.
  - No deben ser botones temporales, sino estar siempre disponibles.
- **Predicibilidad**: *Usuario no debe tener que pensar si palabras, acciones o situaciones con nombres diferentes son distintas*
  - Ser consistente en nomenclatura.
  - Coinciden en nombre sii hacen lo mismo.
  - Definirlo en un solo lugar y en resto usarlo de ahí.
- **Guarda rails**: *Mejor que buenos mensajes de error son los diseños que evitan que los cometas*.
  - Siempre exigir confirmación y ofrecer opción de cancelar al tomar caminos riesgosos.
  - Informar explícitamente sobre consecuencias de acción a realizar.
  - Evitar que se pueda llegar a una situación así por error, por ejemplo que presionando un solo botón se borre todo o que si gato pisa el teclado se realice una acción irreversible o de difícil reversión.
  - Evitar acciones destructivas en silencio.
  - Especialmente en subidas/modificaciones de información.
- **Memory load**: *Evitar que usuario en uso de producto tenga que memorizar el significado de algo*.
  - Siempre hacer objetos, acciones y opciones visibles para el usuario.
  - Evitar códigos de colores, botones, etc sin texto que explique su significado.
  - Si se referencia un concepto de otra parte de la interfaz poner también explícitamente cuál es, así evito que usuario deba hacer memoria.
- **Aceleradores**: *Permitir shortcuts y aceleradores de interacción para que usuarios avanzados puedan sacar provecho*.
  - Ideal es que el usuario sea quién defina los comandos así también reducimos *memory load*.
  - Permitirlos para las acciones básicas.
  - No exigirlos ya que así perdemos a público principiante.
- **Signal-to-noise**: *No contener información poco útil o irrelevante porque interfiere en la visibilidad y atención de la más importante*.
  - Todo lo que no es necesario puede ser evitado.
- **Lenguaje plano**: *Errores deben ser ayudar a su reconocimiento, diagnóstico y recuperación*.
  - Expresar mensajes de error al usuario en lenguaje plano, sin tecnicismos.
  - Mensajes de error deben estar orientados a que usuario identifique fácilmente el problema y sugerir una solución.
  - Explicar *qué pasó*, *por qué* y *cómo solucionarlo*.
- **Just-in-time**: *Ofrecer ayudas concretas y documentación breve*.
  - Lo ideal es que el sistema pueda ser utilizado sin necesidad de leer documentación por parte del usuario.
  - Si es necesario proveer información extra hacerlo con un botón cercano al elemento asociado.
  - Ofrecer la posibilidad de ir directo a una fuente de documentación más detallada.
  - Ofrecer *ayudas/hints* en esos apartados.

### Extras para AI Era

- **Mostrar razonamiento del modelo**: *Evitando silent waiting*.
  - Mantener al usuario actualizado de cada paso para que esté consciente del progreso.
- **Permitir *stop & regenerate***: *Darle al usuario libertad de control*.
  - No hacer que no pueda cancelar una operación, por más costosa que sea.
  - Evitar generación infinita.
  - Que pueda iterar sobre las respuestas previas del modelo para ir adaptando respuesta a sus necesidades.