# Op Art Interactivo

**Autor:** Antonia Rivera Reyes

---

# Descripción General

**Op Art Interactivo** es una experiencia visual desarrollada en **p5.js** inspirada en el movimiento artístico **Op Art**, particularmente en las composiciones geométricas de **Victor Vasarely**.

La experiencia propone que el usuario explore cómo pequeñas modificaciones en el color, la proximidad y el movimiento pueden transformar completamente la percepción de una imagen. Mediante el uso del mouse y el teclado, el usuario interviene directamente sobre la composición, generando variaciones visuales y cromáticas en tiempo real.

---

# Descripción Objetiva

El proyecto está compuesto por tres pantallas o estados principales:

- Pantalla de inicio.
- Pantalla interactiva.
- Pantalla final.

Durante la experiencia se dibuja una grilla de círculos distribuidos uniformemente sobre un fondo degradado. Cada círculo modifica su color según la distancia entre el cursor y su posición.

Cuando el usuario mantiene presionadas las teclas **R**, **G** o **B**, cambia completamente la paleta cromática de la composición y se reproduce un sonido mecánico.

Además:

- Los círculos aumentan de tamaño al presionar el mouse.
- La pantalla inicial posee una portada animada.
- La pantalla final muestra una animación de cierre donde la composición desaparece progresivamente.

---

# Descripción Conceptual

La obra busca explorar cómo la percepción visual puede modificarse mediante pequeñas variaciones de color, repetición y movimiento.

Inspirándose en los principios del **Arte Óptico (Op Art)**, la pieza propone una composición geométrica aparentemente estática que cobra vida gracias a la interacción del espectador.

El usuario deja de ser un observador pasivo para transformarse en parte del sistema visual, modificando continuamente la apariencia de la obra mediante sus acciones.

---

# Referentes

## Movimiento artístico

- Op Art

## Referente principal

- Victor Vasarely

Obra utilizada como inspiración:


**Agev (1974)**

Aunque la composición no replica directamente la obra original, toma como referencia:

- repetición modular
- contraste cromático
- sensación de profundidad
- ilusión óptica
- movimiento visual

---

# Principios de diseño explorados

- Repetición
- Ritmo
- Contraste
- Color
- Modulación
- Movimiento aparente
- Interactividad

---

# Sistema Computacional

## Inputs

El proyecto utiliza los siguientes datos de entrada:

- Posición del mouse (X,Y)
- Click del mouse
- Tecla ENTER
- Teclas R
- Teclas G
- Teclas B

---

## Procesos

El programa realiza continuamente los siguientes procesos:

- Calcula la distancia entre cada círculo y el mouse utilizando `dist()`.
- Convierte esa distancia en valores de color mediante `map()`.
- Mezcla colores usando `lerpColor()`.
- Genera una grilla mediante dos ciclos `for`.
- Cambia la paleta de colores según la tecla presionada.
- Actualiza constantemente la pantalla mediante `draw()`.
- Controla el cambio de estados utilizando la variable `pantalla`.

---

## Estados

El sistema posee tres estados:

### Inicio

Muestra una portada con una grilla, título y mensaje de bienvenida.

↓

### Experiencia

Presenta la composición interactiva donde el usuario modifica el color y el tamaño de los círculos.

↓

### Final

Muestra una animación de cierre donde la grilla desaparece progresivamente y aparece un mensaje final.

---

## Eventos

Los principales eventos del programa son:

### ENTER

- Inicio → Experiencia
- Experiencia → Final
- Final → Inicio

### Mouse

- modifica el color de los círculos según la cercanía

### Mouse Presionado

- aumenta el tamaño de los círculos

### Teclas R G B

- cambian la paleta cromática
- reproducen sonido

### Soltar tecla

- vuelve a la paleta base
- detiene el sonido

---

## Outputs

El sistema responde generando:

### Visuales

- cambio de color
- gradientes
- variación del tamaño de los círculos
- aparición de textos
- transición entre pantallas
- animación final

### Sonoros

- sonido de inicio
- sonido de cambio de color
- sonido final

---

# Explicación de la Interacción

El usuario comienza observando una portada donde se le invita a presionar ENTER.

Al ingresar, puede mover el cursor sobre la composición. La cercanía del mouse altera progresivamente el color de los círculos, generando una sensación de profundidad y movimiento.

Si mantiene presionado el mouse, todos los círculos aumentan su tamaño.

Las teclas **R**, **G** y **B** modifican completamente la paleta cromática mientras reproducen un sonido asociado.

Finalmente, al presionar nuevamente ENTER se accede a una pantalla de cierre donde la composición desaparece lentamente y aparece un mensaje final.

---

# Recursos Multimedia

## Tipografías

- Tipo01.otf
- Tipo2.otf

Utilizadas para diferenciar el título y los textos secundarios.

---

## Sonidos

### Intro01.mp3

Reproducido al comenzar la experiencia.

### teclas01.mp3

Reproducido durante el cambio de color.

### outro.mp3

Reproducido al finalizar la experiencia.

---

# Registro del Proceso

## Referentes

- Victor Vasarely
- Op Art

## Bocetos

Durante el proceso se exploraron distintas configuraciones de grillas, colores y composiciones antes de llegar al resultado final.

## Iteraciones

Se realizaron múltiples modificaciones relacionadas con:

- organización de pantallas
- incorporación de sonido
- cambio de tipografías
- transición entre estados
- mejora de la portada
- diseño de la pantalla final

## Capturas

*(Aquí pueden agregarse imágenes del proceso de desarrollo.)*

---

# Reflexión Final

Este proyecto permitió comprender cómo estructuras geométricas simples pueden generar experiencias visuales complejas cuando se combinan con interacción y programación.

Uno de los principales desafíos fue organizar el código mediante estados y lograr que las transiciones funcionaran correctamente sin afectar la experiencia del usuario.

También fue necesario aprender a integrar distintos recursos multimedia como tipografías y sonidos, además de controlar eventos mediante teclado y mouse.

Finalmente, el proyecto permitió entender cómo herramientas básicas de programación pueden utilizarse para construir experiencias visuales inspiradas en referentes históricos del diseño y el arte.

---

# Presentación

Durante la exposición se abordarán los siguientes puntos:

- Concepto del proyecto
- Referentes utilizados
- Inspiración en Victor Vasarely y el Op Art
- Funcionamiento general
- Estados del sistema
- Eventos e interacción
- Inputs y Outputs
- Uso de recursos multimedia
- Estructura general del programa
- Reflexión final
