# 🧮 Input Character Counter - README

<https://via.placeholder.com/600x400/4a90e2/ffffff?text=Character+Counter+App> <!-- Sugerencia: Reemplazar con imagen real -->

## ✨ Descripción

Una aplicación web ligera y elegante que cuenta en tiempo real los caracteres ingresados en un campo de texto. Perfecta para verificar longitudes de texto en formularios, publicaciones o mensajes. ¡Escribe y observa cómo aumenta el contador!

## 🚀 Características

✅ Conteo en tiempo real de caracteres  
✅ Diseño responsive con efectos visuales  
✅ Incluye espacios y caracteres especiales en el conteo  
✅ Animaciones suaves y feedback visual  
✅ Interfaz minimalista y fácil de usar  

## ⚙️ Funcionamiento

El núcleo de la aplicación se basa en un simple pero poderoso mecanismo de JavaScript que detecta cada pulsación de tecla en el campo de texto y actualiza dinámicamente el contador:

```javascript
const count = document.querySelector("p");
const input = document.querySelector("input");

input.addEventListener("keyup", () => {
    count.innerHTML = input.value.length;
});
```

**Explicación del código JavaScript:**

1. **Selección de elementos DOM:**

    - **``document.querySelector("p")``** selecciona el párrafo donde se mostrará el conteo
    - **``document.querySelector("input")``** selecciona el campo de texto

2. **Manejo de eventos:**

    - **``addEventListener("keyup", ...)```** detecta cuando el usuario libera una tecla

    - La función flecha **``() => {...}``** se ejecuta después de cada pulsación

3. **Actualización dinámica:**

    - **``input.value.length``** obtiene la longitud actual del texto

    - **``count.innerHTML = ...``** actualiza el contenido del párrafo con el nuevo valor

## 🎨 Diseño y Experiencia de Usuario

El CSS proporciona una experiencia visual atractiva con:

```css
/*Efecto hover en el contenedor*/
.container:hover {
    transform: scale(1.05);
}

/*Transiciones suaves en campos de texto*/
input {
    transition: all 0.3s ease;
}

/*Feedback visual al enfocar el campo*/
input:focus {
    border-color: #666;
    box-shadow: 0 0 5px rgba(0, 0, 0, 0.5);
}
```

**Características destacadas:**

- Gradiente dinámico de fondo

- Animaciones al pasar el ratón sobre el contenedor

- Efectos de transición suaves en elementos interactivos

- Diseño responsive que funciona en móviles y escritorio

## 🛠 Tecnologías Utilizadas

**Frontend:**

Estructura semántica: [![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)  

Estilos y animaciones: [![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)

Lógica interactiva: ![JAVASCRIPT](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 📥 Instalación y Uso

1. Clona el repositorio:

    ```bash
    git clone https://github.com/Seb-RM/Javascript_Html_Css-Input-Character-Counter.git
    ```

2. Abre el proyecto:

    ```bash
    cd Javascript_Html_Css-Input-Character-Counter
    ```

3. Ejecuta la aplicación:

    - Abre index.html en tu navegador

4. Para usar:

    - Escribe en el campo de texto

    - Observa cómo el contador aumenta/disminuye

    - ¡El conteo incluye espacios y caracteres especiales!
