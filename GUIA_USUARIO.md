# Guía de Uso: Generador de Plantillas de Video

## Introducción
Esta guía explica cómo utilizar la plantilla JSON y el formulario HTML para crear estructuras de video de manera eficiente.

## Estructura de la Plantilla JSON

### Técnicas de Composición de Escenas

Basado en las mejores prácticas de Google Vertex AI para generación de video, aquí hay técnicas avanzadas para mejorar cada escena:

#### 1. Ángulos de Cámara
- **Plano general (Wide Shot)**: Muestra toda la escena, ideal para establecer la ubicación
- **Plano medio (Medium Shot)**: Encuadre desde la cintura hacia arriba, perfecto para interacciones
- **Primer plano (Close-up)**: Enfatiza emociones o detalles importantes
- **Picado/Contrapicado**: Ángulos altos o bajos para dar poder o vulnerabilidad
- **Cámara en movimiento**: Travellings, grúas o steadycam para dinamismo

#### 2. Iluminación
- **Estilo tres puntos**: Luz principal, de relleno y de pelo para profundidad
- **Alto contraste**: Para un aspecto dramático
- **Iluminación suave**: Para un ambiente más natural
- **Luces prácticas**: Fuentes de luz visibles en la escena

#### 3. Composición
- **Regla de los tercios**: Coloca los elementos clave en las intersecciones
- **Líneas principales**: Usa líneas naturales para guiar la mirada
- **Encuadre dentro del encuadre**: Marcos naturales para añadir profundidad
- **Espacio negativo**: Para énfasis dramático

#### 4. Movimiento
- **Movimientos suaves**: Para un aspecto profesional
- **Movimientos intencionales**: Cada movimiento debe tener un propósito
- **Estabilidad**: Usa trípode o estabilizador cuando sea necesario

### Metadatos Básicos
```json
{
  "video": {
    "metadatos": {
      "titulo": "Nombre del Video",
      "duracion_total": "30s",
      "orientacion": "vertical",
      "resolucion": "1080x1920",
      "fps": 30,
      "tipo": "corto_creativo"
    }
  }
}
```

### Estructura de Escenas
Cada escena debe contener:
- `id`: Identificador único
- `descripcion`: Lo que sucede en la escena
- `duracion`: Duración en segundos
- `angulo_camara`: (Ej: "plano_medio", "primer_plano")
- `movimiento_camara`: (Ej: "estatica", "suave_seguimiento")
- `iluminacion`: (Ej: "tres_puntos", "alto_contraste")
- `composicion`: (Ej: "regla_tercios", "lineas_conductoras")
- `elementos`: Personajes y objetos con sus posiciones
- `transicion`: Cómo se conecta con la siguiente escena

### Estilos Visuales Recomendados

#### 1. Estilo Cinematográfico
- **Enfoque**: Narrativa visual rica
- **Técnicas**:
  - Profundidad de campo reducida
  - Iluminación dramática
  - Movimientos de cámara suaves y calculados
  - Paletas de colores limitadas

#### 2. Estilo Documental
- **Enfoque**: Autenticidad y realismo
- **Técnicas**:
  - Cámara en mano para sensación de inmediatez
  - Iluminación natural
  - Entrevistas con primeros planos
  - Imágenes B-roll para contexto

#### 3. Estilo Animado
- **Enfoque**: Creatividad y estilo visual
- **Técnicas**:
  - Colores vibrantes
  - Movimientos exagerados
  - Transiciones dinámicas
  - Efectos visuales integrados

### Ejemplos de Configuración de Escena

```json
{
  "escena": {
    "id": "escena_1",
    "descripcion": "Personaje principal camina por la calle",
    "duracion": "8s",
    "angulo_camara": "plano_medio",
    "movimiento_camara": "seguimiento_lateral",
    "iluminacion": "hora_dorada",
    "composicion": "regla_tercios",
    "elementos": {
      "personaje_principal": {
        "posicion": "derecha_tercio",
        "accion": "caminando"
      },
      "fondo": {
        "tipo": "calle_ciudad",
        "enfoque": "desenfoque_sutil"
      }
    },
    "transicion": {
      "tipo": "fundido",
      "duracion": "1s"
    }
  }
}
```

## Uso del Formulario HTML

### 1. Configuración Inicial
1. Abre `formulario_mejorado.html` en tu navegador
2. Completa los metadatos básicos del video

### 2. Añadiendo Escenas
1. Haz clic en "Agregar Escena"
2. Completa la descripción y duración
3. Especifica los elementos visuales
4. Configura la transición con la siguiente escena

### 3. Personalización de Estilo
- Selecciona un tono visual
- Ajusta la paleta de colores
- Configura la música de fondo

### 4. Exportación
1. Usa "Vista Previa" para ver el JSON generado
2. Copia el JSON o descárgalo con "Exportar JSON"

## Ejemplo de Uso

1. **Crear un video promocional**
   - Tono: Profesional
   - Duración: 60s
   - 3-5 escenas principales
   - Música de fondo energética

2. **Video tutorial**
   - Tono: Educativo
   - Duración: 120s
   - Escenas por paso
   - Transiciones suaves

## Consejos de Composición

### 1. Guía Visual
- **Planificación**: Crea un guión gráfico antes de grabar
- **Continuidad**: Mantén la continuidad entre tomas
- **Ritmo**: Varía la duración de las escenas según la emoción

### 2. Técnicas Avanzadas
- **Profundidad**: Crea capas visuales (primer plano, medio, fondo)
- **Color**: Usa la teoría del color para transmitir emociones
- **Espacio**: Deja espacio para el movimiento y la edición

### 3. Optimización para IA
- **Iluminación consistente**: Ayuda a la generación de IA
- **Composición clara**: Facilita el reconocimiento de objetos
- **Movimientos suaves**: Mejora los resultados de seguimiento

### 4. Flujo de Trabajo Eficiente
1. Previsualiza cada escena
2. Ajusta la iluminación según sea necesario
3. Revisa la composición en el visor
4. Prueba diferentes ángulos
5. Verifica la continuidad con las escenas adyacentes

## Solución de Problemas

### El JSON no se genera
- Verifica que todos los campos requeridos estén completos
- Asegúrate de que las duraciones sean números válidos

### Problemas con la vista previa
- Actualiza la página
- Verifica la consola del navegador para errores

## Recursos Adicionales
- [Guía de diseño de video](https://ejemplo.com/guia-video)
- [Paletas de colores recomendadas](https://ejemplo.com/paletas)
- [Ejemplos de plantillas](https://ejemplo.com/ejemplos)
