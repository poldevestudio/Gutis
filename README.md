# Guti's · Burger, Beer & Drinks 🍔🍺

Sitio web oficial, catálogo interactivo y motor de pedidos de alta conversión desarrollado para **Guti's Burger, Beer & Drinks**, hamburguesería y cervecería artesanal ubicada en el complejo **Villa Borguesa**, Belén de Escobar, Provincia de Buenos Aires.

---

## 📍 Datos Oficiales del Comercio (Ficha de Google Maps)
- **Nombre:** Guti's Burger, Beer & Drinks
- **Ubicación Oficial:** Complejo Villa Borguesa, Ruta Provincial 25 (RP25), Local 3, Belén de Escobar, Provincia de Buenos Aires (B1625).
- **Ficha Google Maps:** [Guti's en Google Maps](https://maps.app.goo.gl/oKqWUAHPPs1K6RfB7)
- **Calificación en Google:** **4.7 ★** (Excelente reputación y comentarios)
- **Coordenadas GPS:** `-34.3267988, -58.7593188`
- **Instagram Oficial:** [@gutis.escobar](https://www.instagram.com/gutis.escobar/)
- **Teléfono Oficial del Comercio:** `+54 11 2609-7141`
- **Teléfono de Testing Configurado:** `+54 9 11 2673-1952` (Polo - Poldev Estudio)
- **Diferencial Gastronómico:** Medallones 100% elaborados con **carne de ojo de bife seleccionada**, papas rejilla y rústicas crocantes, canillas de cerveza artesanal tirada (IPA, Golden) y barra de coctelería con bartenders profesionales (Gin Tonic, tragos de autor).
- **Horarios Habituales:**
  - **Lunes y Martes:** Cerrado.
  - **Miércoles y Jueves:** 19:30 a 01:00 hs.
  - **Viernes:** 19:30 a 02:00 hs.
  - **Sábados:** Mediodía (12:00 a 16:00 hs.) y Noche (19:30 a 01:00 hs.).
  - **Domingos:** Mediodía (12:00 a 16:00 hs.) y Noche (19:30 a 02:00 hs.).

---

## 🎨 Identidad Visual & Paleta de Colores Formal (Craft & Heritage)

A partir del isotipo oficial de Guti's (*Burger, Beer & Drinks*), se seleccionó una paleta formal, sobria y artesanal que combina los tonos del tostado del pan brioche, el dorado de la cerveza artesanal tirada y la elegancia del fondo oscuro:

| Rol | Variable CSS | Hex | Descripción y Aplicación |
| :--- | :--- | :--- | :--- |
| **Fondo Principal** | `--bg` | `#0E0F0C` | Negro carbón profundo con matiz cálido café tostado. |
| **Paneles & Tarjetas** | `--panel` | `#171815` | Gris grafito oscuro con bordes sutiles para jerarquía de contenido. |
| **Hover de Paneles** | `--panel-hover` | `#20211d` | Elevación sutil al pasar el cursor o interactuar. |
| **Acento Primario** | `--orange` / `--amber` | `#D4A359` | Ámbar dorado / malta tostada formal que armoniza con el logo. |
| **Sombra Acento** | `--orange-dark` | `#8C6328` | Sombra y bisel de botones para efecto 3D táctil. |
| **Tipografía Clara** | `--cream` | `#F4EDE1` | Marfil cálido vintage para títulos y lectura descansada. |
| **Texto Secundario** | `--muted` | `#A69F92` | Tono almendra atenuado para descripciones y precios unitarios. |
| **Insignias & Estrellas**| `--gold` | `#E5B96A` | Dorado brillante para las 4.7 estrellas de Google Maps. |
| **Conversión WhatsApp** | `--wa-green` | `#25D366` | Verde oficial con pulso luminoso animado permanente. |

---

## 🛠️ Criterio Senior & Funcionalidades Implementadas

1. **Arquitectura Idéntica & Reutilización de Esqueleto:**
   - Se mantuvo **el 100% del esqueleto probado de La Papota**, sin alterar botones, secciones ni flujos de usuario, adaptando con máxima precisión todos los copys, branding, horarios y oferta gastronómica a Guti's.

2. **100% Mobile First & Experiencia Celular:**
   - Menú hamburguesa animado con drawer lateral y bloqueo de scroll al abrir.
   - Prevención de zoom accidental en inputs para dispositivos iOS / Android (`font-size: 16px` mínimo).
   - Botón flotante permanente de WhatsApp con pulso de atención.
   - Barra flotante inferior de pedido que aparece de forma fluida tan pronto se selecciona un producto.

3. **Verificación de Horarios en Tiempo Real (`checkBusinessHours`):**
   - Sistema inteligente adaptado al cronograma real de Guti's (franjas nocturnas Mié a Dom, doble turno los fines de semana y manejo de trasnoche hasta las 02:00 am). Muestra dinámicamente si la cocina y barra están abiertas o cuándo reabren.

4. **SEO Local & Rich Snippets:**
   - Schema.org con `@type: BarOrPub` y datos completos: calificación 4.7★, dirección en Belén de Escobar (Villa Borguesa), coordenadas GPS y enlace oficial a Google Maps.
   - Open Graph para compartir enlaces con preview en WhatsApp e Instagram.

---

## 📂 Arquitectura y Dos Propuestas para el Cliente (Poldev Estudio)

### 1️⃣ Propuesta Básica — Landing de Presencia Local & Conversión Directa (`index.html`)
- **Objetivo:** Imagen de alto nivel para posicionar a Guti's como referente de Villa Borguesa y Belén de Escobar.
- **Características:**
  - Ficha oficial con mapa embebido interactivo y **pin rojo** en Ruta 25.
  - Botón directo *"CÓMO LLEGAR CON GOOGLE MAPS"* (apertura GPS inmediata).
  - Ticker infinito con los diferenciales del local (100% Ojo de Bife, Cerveza Tirada, Tragos de Autor, 4.7★).
  - Sección *"Nuestra Onda"* con fotografía de ambiente (`local_gutis.jpg`).

### 2️⃣ Propuesta Pro — Menú Digital Interactivo & Motor de Pedidos Autónomo (`menu.html`)
- **Objetivo:** Automatizar la toma de pedidos, eliminar cuellos de botella en la barra/caja y aumentar el ticket promedio.
- **Características:**
  - **Filtros por categoría:** Todo el Menú, Hamburguesas (Ojo de Bife), Papas Rústicas & Rejilla, Tapeos & Lomitos, Super Panchos & Snacks, Cervezas & Tragos.
  - **Carrito reactivo con persistencia local (`localStorage`):** Guarda la selección del cliente si recarga la página.
  - **Modal de Checkout completo:**
    - Modalidad de entrega: *Envío a Domicilio* (con campo de dirección en Escobar) o *Retiro en el Local (Villa Borguesa)*.
    - Opciones de pago: *Efectivo* (con cálculo de vuelto), *Transferencia Bancaria* o *Mercado Pago*.
    - Notas personalizadas para la cocina (ej: "sin cebolla", "bien cocido").
  - **Comanda automatizada a WhatsApp:** Genera un ticket estructurado, claro y listo para que la cocina y la barra empiecen a preparar en el instante.

---

## 📁 Archivos del Proyecto
- `index.html`: Landing institucional / comercial de alta conversión (Propuesta 1).
- `menu.html`: Menú digital interactivo con carrito y generador de comanda a WhatsApp (Propuesta 2).
- `gutis_logo.png`: Logo oficial de Guti's (Burger, Beer & Drinks) recortado y optimizado con fondo transparente.
- `local_gutis.jpg`: Fotografía de ambiente cálido, mesas y barra artesanal.
- `README.md`: Documentación técnica y comercial de la maqueta.

---
Desarrollado y optimizado por **Poldev Estudio** · Presencia Digital & Sitios Web de Alta Conversión.
