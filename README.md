# Toque Humano

Una skill de Claude Code que elimina signos de escritura generada por IA, haciendo que el texto suene más natural y humano.

Basada en la guía de Wikipedia "Signos de escritura de IA", mantenida por WikiProject AI Cleanup.

---

## Instalación

### Método recomendado (clonar)

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/aletinto/toque-humano.git ~/.claude/skills/toque-humano
```

### Método manual (solo archivo)

```bash
mkdir -p ~/.claude/skills/toque-humano
cp SKILL.md ~/.claude/skills/toque-humano/
```

---

## 💡 Uso

En Claude Code, invoca la skill:

```
/toque-humano
```

Pega tu texto para humanizar.

O pregunta directamente:

```
Por favor humaniza este texto: [tu texto aquí]
```

---

## 📋 Los 25 Patrones

Detecta y elimina:

### Contenido (6 patrones)
1. Énfasis indebido en significado/legado
2. Énfasis indebido en notabilidad mediática
3. Análisis superficiales con "-ando"/"-iendo"
4. Lenguaje promocional
5. Atribuciones vagas
6. Secciones "Retos y Perspectivas" formulaicas

### Lenguaje (6 patrones)
7. Vocabulario de IA sobreusado
8. Evitación de cópula ("se erige como" → "es")
9. Paralelismos negativos ("No es solo X, es Y")
10. Regla de tres forzada
11. Reciclaje de sinónimos
12. Rangos falsos

### Estilo (6 patrones)
13. Sobreuso de rayas largas (—)
14. Negritas excesivas
15. Listas con encabezados en línea
16. Mayúsculas de Título
17. Emojis decorativos
18. Comillas curvas

### Comunicación (3 patrones)
19. Artefactos de chatbot ("Espero que esto te ayude")
20. Disclaimers de corte de conocimiento
21. Tono sicarifante

### Relleno (4 patrones)
22. Frases de relleno
23. Exceso de cautela
24. Conclusiones genéricamente positivas
25. Sobreuso de palabras con guión

---

## 📖 Documentación

**Para empezar:**
- [GUIA_RAPIDA.md](GUIA_RAPIDA.md) — 30 segundos, las 5 señales más comunes

**Para profundizar:**
- [SKILL.md](SKILL.md) — El prompt completo con 25 patrones detallados y ejemplos
- [EJEMPLOS.md](EJEMPLOS.md) — 5 ejemplos reales de humanización antes/después
- [INDICE.md](INDICE.md) — Navegación completa

**Para contribuir:**
- [CONTRIBUTING.md](CONTRIBUTING.md) — Cómo reportar bugs y aportar mejoras

---

## 🎯 Ejemplo Rápido

**Antes (suena a IA):**
> El desarrollo asistido por IA se erige como un duradero testamento del potencial transformador, marcando un momento pivotal en la evolución del software.

**Después (humanizado):**
> Los asistentes de código aceleran las partes aburridas. Son buenos en boilerplate, malo en decisiones arquitectónicas.

Ver más ejemplos en [EJEMPLOS.md](EJEMPLOS.md).

---

## 🔑 Insight Clave

> "Los LLMs usan algoritmos estadísticos para adivinar qué debería venir después. El resultado tiende hacia el resultado más probable que se aplica a la variedad más amplia de casos."

Por eso la escritura de IA se siente genérica, inflada y predecible. Toque Humano lo corrige.

---

## 📝 Licencia

MIT License — Eres libre de usar, modificar y distribuir.

**Versión:** 1.0.0 | **Autor:** Ale Tinto | **Última actualización:** 2026

---

**¿Necesitas ayuda?** Lee [GUIA_RAPIDA.md](GUIA_RAPIDA.md) o consulta [INDICE.md](INDICE.md) para navegar.
