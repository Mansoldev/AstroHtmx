[HTMX](https://htmx.org/)

###### **Versión 1.9.10:**

```
- hx-get="URL" > Hace un get a la URL
- hx-trigger="load delay:2s" > (click por defecto) Hace la petición al cargar con un delay de 2s
```

Modificadores [hx-trigger](https://htmx.org/attributes/hx-trigger/):

* **once:** Solo se ejecuta una vez.
* **changed**: Cuando cambia el value del elemento.
* **delay:time**: Tras x tiempo.
* **every time:** Cada x tiempo.

```
- hx-target="CSSSelector": hace la petición y devuelve los resultados a la etiqueta con id o clase.
- hx-swap="outerHTML": Reemplaza el target (innerHTML por defecto)
```

Valores [hx-swap](https://htmx.org/attributes/hx-swap/):

* textContent: Reemplaza el contenido sin parsear la respuesta a HTML.
* beforebegin: Inserta la respuesta antes del target.
* afterbegin: Inserta la respuesta antes del primer hijo del target.
* beforeend: Inserta la respuesta despues del último hijo del target.
* afterend: Inserta la respuesta despues del target.
* delete: Elimina el target independientemente de la respuesta.
* none: No aparece el contenido de la respuesta.

```
- hx-indicator="CSSSelector": Indica que html tiene que cambiar cuando se activa la petición.
- hx-disabled-elt="this": Deshabilita el elemento actual mientras sucede la petición.
```

###### Versión 2:
