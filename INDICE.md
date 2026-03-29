# Índice de Toque Humano

Tu guía para entender y usar esta skill.

## 📖 Documentación Principal

### Para empezar rápido
- **[GUIA_RAPIDA.md](GUIA_RAPIDA.md)** — 30 segundos de instalación + 5 patrones más comunes
- **[README.md](README.md)** — Descripción completa, instalación, 25 patrones resumidos

### Para entender a fondo
- **[SKILL.md](SKILL.md)** — El prompt completo con toda la metodología
  - Personalidad y alma
  - 25 patrones detallados con ejemplos
  - Proceso paso a paso
  - Formato de salida

### Para ver ejemplos reales
- **[EJEMPLOS.md](EJEMPLOS.md)** — 5 ejemplos completos (email, blog, producto, biografía, reporte)

---

## 🛠️ Información Técnica

- **[package.json](package.json)** — Metadatos de la skill
- **[LICENSE](LICENSE)** — MIT License
- **[CONTRIBUTING.md](CONTRIBUTING.md)** — Cómo contribuir

---

## 🚀 Instalación

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/aletinto/toque-humano.git ~/.claude/skills/toque-humano
```

O solo copia el archivo SKILL.md si ya clonaste:

```bash
mkdir -p ~/.claude/skills/toque-humano
cp SKILL.md ~/.claude/skills/toque-humano/
```

---

## 💡 Cómo empezar

### Opción 1: Usar la skill
En Claude Code:
```
/toque-humano

[pega tu texto aquí]
```

### Opción 2: Pedir humanización directa
```
Por favor humaniza este texto: [tu texto]
```

---

## 🎯 Navegación por tipo de contenido

### Escribes emails
→ Ver [EJEMPLOS.md - Ejemplo 1: Email corporativo](EJEMPLOS.md)

### Escribes artículos de blog
→ Ver [EJEMPLOS.md - Ejemplo 2: Artículo de blog](EJEMPLOS.md)

### Escribes descripciones de productos
→ Ver [EJEMPLOS.md - Ejemplo 3: Descripción de producto](EJEMPLOS.md)

### Necesitas reportes profesionales
→ Ver [EJEMPLOS.md - Ejemplo 5: Reporte ejecutivo](EJEMPLOS.md)

### Quieres la lista completa de 25 patrones
→ Ver [SKILL.md](SKILL.md)

### Quieres aportar mejoras
→ Ver [CONTRIBUTING.md](CONTRIBUTING.md)

---

## 📚 Los 25 patrones explicados

| # | Patrón | Detecta | Corrección |
|----|--------|---------|-----------|
| 1 | Inflación de significado | "pivotal", "testamento" | Simplifica el lenguaje |
| 2 | Notabilidad name-dropping | Listas de medios sin contexto | Menciona casos específicos |
| 3 | Análisis superficial -ando/-iendo | "simbolizando", "reflejando" | Elimina o concretiza |
| 4 | Lenguaje promocional | "vibrante", "impresionante" | Neutral, descriptivo |
| 5 | Atribuciones vagas | "expertos creen", "reportes indican" | Cita específicamente |
| 6 | Secciones formulaicas | "A pesar de, continúa prosperando" | Hechos reales |
| 7 | Vocabulario IA | Palabras repetidas (crucial, clave) | Vocabulario variado |
| 8 | Evitación de cópula | "se erige como", "cuenta con" | Usa "es", "tiene" |
| 9 | Paralelismos negativos | "No es solo X; es Y" | Afirma directamente |
| 10 | Regla de tres | Siempre 3 items | Número natural |
| 11 | Reciclaje de sinónimos | Mismo concepto con 4 palabras | Repite cuando sea claro |
| 12 | Rangos falsos | "de A a B, de C a D" | Lista directamente |
| 13 | Sobreuso de rayas largas (—) | Múltiples — en párrafo | Usa comas o puntos |
| 14 | Negritas excesivas | **Muchas negritas** | Solo si es muy necesario |
| 15 | Listas con encabezados | **Título:** descripción | Prosa natural |
| 16 | Mayúsculas de título | Las Palabras Principales | Mayúscula normal |
| 17 | Emojis | 🚀 💡 ✅ en el texto | Elimina |
| 18 | Artefactos de chatbot | "Espero que esto te ayude" | Elimina completamente |
| 19 | Disclaimers de corte | "Mis datos son hasta..." | Encuentra fuentes reales |
| 20 | Tono sicarifante | "¡Tienes razón!" | Responde directamente |
| 21 | Frases de relleno | "Con el propósito de" | Simplifica |
| 22 | Exceso de cautela | "podría posiblemente" | "Puede" |
| 23 | Conclusiones genéricas | "El futuro se ve brillante" | Datos específicos |
| 24 | Comillas curvas | "texto" vs "texto" | Rectas |
| 25 | Palabras con guión | "data-driven", "client-facing" | "data driven", "client facing" |

---

## ❓ Preguntas frecuentes

**¿Cómo empiezo?**
→ Lee [GUIA_RAPIDA.md](GUIA_RAPIDA.md) (5 min)

**¿Por qué suena mi texto a IA?**
→ Lee [SKILL.md](SKILL.md) sección "Patrones de contenido" (15 min)

**¿Tengo un patrón que no está documentado?**
→ Abre un issue o lee [CONTRIBUTING.md](CONTRIBUTING.md)

**¿Puedo usar esto para textos en otro idioma?**
→ El SKILL.md está en español. Para otros idiomas necesitarías adaptar los ejemplos.

**¿Debo eliminar toda mi personalidad?**
→ No. La goal es *añadir* voz humana genuina, no eliminarla. Ver "Personalidad y Alma" en [SKILL.md](SKILL.md)

---

## 🔗 Referencias externas

- [Wikipedia: Signos de escritura de IA](https://en.wikipedia.org/wiki/Talk:Artificial_intelligence/Archive_8#Signs_of_AI_writing)
- [WikiProject AI Cleanup](https://en.wikipedia.org/wiki/Wikipedia:WikiProject_AI_cleanup)

---

## 📝 Licencia

MIT License — Eres libre de usar, modificar y distribuir. Ver [LICENSE](LICENSE)

---

**Versión:** 1.0.0  
**Última actualización:** 2026-03-29  
**Creador:** Ale Tinto  
**Repositorio:** https://github.com/aletinto/toque-humano

