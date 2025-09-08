# FLOW\.md

Este repositorio existe para ayudarte a construir proyectos que se conviertan en un portafolio atractivo. La idea es que simules cómo sería trabajar en un producto real: primero analizas y documentas la necesidad de negocio, luego eliges tu stack y justificas tu decisión, y finalmente programas la solución.

El resultado final es un **repositorio propio** por cada ejercicio, con dos partes claras:

1. Una carpeta `docs/` donde guardas el análisis.
2. La implementación de la aplicación con su demo.

---

## Carpeta `docs/`

Dentro de cada proyecto que construyas, crea una carpeta llamada `docs/` y allí escribe los siguientes archivos. Piensa en ellos como pasos que tienes que ir completando.

### 1. `ObjetivoNegocio.md`

* Describe el problema que resuelve tu producto.
* Explica quién lo usaría.
* Define qué debe lograr el MVP.

**Ejemplo:**

```
Problema: Las tiendas pequeñas no tienen control de inventario.
Usuarios: Propietario y cajero.
Objetivo MVP: Registrar productos y ventas simples.
```

---

### 2. `Requerimientos.md`

Convierte el objetivo en historias de usuario con criterios de aceptación.

**Plantilla:**

```
ID: US-001
Como [rol] quiero [objetivo] para [beneficio].
Criterios de aceptación:
- Dado...
- Cuando...
- Entonces...
```

Incluye mínimo 5 historias para dar un contexto real a tu MVP y demostrar tu análisis.

---

### 3. `DiseñoTecnico.md`

Explica cómo piensas construirlo.

* Justifica el stack que vas a usar (framework, lenguaje, base de datos).
* Incluye un esquema simple de datos.
* Escribe 3 a 6 endpoints o funciones clave con ejemplos de entrada y salida.

**Ejemplo tabla de datos:**

| Tabla Producto | Campos  |
| -------------- | ------- |
| id             | entero  |
| usuario        | texto   |
| voto           | texto   |
| fecha_voto     | fecha   |

---

### 4. `PlanTrabajo.md`

Lista las tareas que harás y ponles una prioridad.

**Ejemplo:**

* \[MUST] Crear consulta para obtener votos del usuario
* \[MUST] Registrar voto y validar duplicidad
* \[SHOULD] Listado de votos por fecha
* \[COULD] Exportar votos a CSV

Puedes usar etiquetas como MUST, SHOULD, COULD, WON’T.

---

### 5. `Pruebas_Demo.md`

Aquí anota:

* Casos de prueba básicos (te sugiero al menos 3).
* Cómo correr tu proyecto en local.
* Link a la demo o un video corto mostrando el flujo principal.

**Ejemplo caso de prueba:**

```
TC-001: Registrar voto con usuario que ya votó
Dado un usuario que ya votó con anticipación
Cuando intenta votar de nuevo
Entonces mostrar determinado mensaje
```

---

## Checklist antes de decir “terminado”

* [ ] `ObjetivoNegocio.md` completo
* [ ] `Requerimientos.md` con 5–10 historias
* [ ] `DiseñoTecnico.md` con stack justificado, datos y endpoints
* [ ] `PlanTrabajo.md` con tareas priorizadas
* [ ] `Pruebas_Demo.md` con casos, instrucciones y demo
* [ ] Código funcionando
* [ ] Demo accesible o video
* [ ] README principal actualizado
