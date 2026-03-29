# Toque Humano

Una skill de Claude Code que elimina signos de escritura generada por IA, haciendo que el texto suene más natural y humano.

## Instalación

### Recomendado (clonar directamente en el directorio de skills de Claude Code)

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/aletinto/toque-humano.git ~/.claude/skills/toque-humano
```

### Instalación manual/actualización (solo el archivo skill)

Si ya tienes este repositorio clonado (o descargaste SKILL.md), copia el archivo de skill en el directorio de skills de Claude Code:

```bash
mkdir -p ~/.claude/skills/toque-humano
cp SKILL.md ~/.claude/skills/toque-humano/
```

---

## Uso

En Claude Code, invoca la skill:

```
/toque-humano
```

Luego pega tu texto para humanizar.

O pregunta directamente a Claude:

```
Por favor humaniza este texto: [tu texto aquí]
```

---

## Descripción General

Basada en la guía de Wikipedia "Signos de escritura de IA", mantenida por WikiProject AI Cleanup. Esta guía comprehensiva proviene de observaciones de miles de instancias de texto generado por IA.

**Insight clave de Wikipedia:**

> "Los LLMs usan algoritmos estadísticos para adivinar qué debería venir después. El resultado tiende hacia el resultado más estadísticamente probable que se aplica a la variedad más amplia de casos."

---

## 25 Patrones Detectados

### Patrones de Contenido
1. **Énfasis indebido en significado, legado y tendencias amplias** — *"marcando un momento pivotal en la evolución de..."* → *"fue establecido en 1989 para recopilar estadísticas"*
2. **Énfasis indebido en notabilidad y cobertura mediática** — *"citado en NYT, BBC, FT"* → *"En una entrevista de 2024 con NYT, argumentó..."*
3. **Análisis superficiales con terminaciones en "-ando"/"-iendo"** — *"simbolizando... reflejando... exhibiendo..."* → Eliminar o expandir con fuentes reales
4. **Lenguaje promocional y publicitario** — *"ubicado en la impresionante región"* → *"es una ciudad en la región"*
5. **Atribuciones vagas y palabras ambiguas** — *"Los expertos creen que juega un papel crucial"* → *"según estudio de 2019 por..."*
6. **Secciones esquemáticas "Retos y Perspectivas"** — *"A pesar de retos... continúa prosperando"* → Hechos específicos sobre desafíos reales

### Patrones de Lenguaje
7. **Vocabulario de IA sobreusado** — *"Además... testamento... panorama... exhibiendo"* → *"también... siguen siendo comunes"*
8. **Evitación de cópula (es/son/tiene)** — *"se erige como... presenta... cuenta con"* → *"es... tiene"*
9. **Paralelismos negativos** — *"No es solo X, es Y"* → Afirma el punto directamente
10. **Sobreuso de Regla de Tres** — *"innovación, inspiración, e insights"* → Usa número natural de items
11. **Reciclaje de sinónimos (Variación elegante)** — *"protagonista... personaje principal... figura central... héroe"* → *"protagonista"* (repite cuando sea más claro)
12. **Rangos falsos** — *"del Big Bang a la materia oscura"* → Lista temas directamente

### Patrones de Estilo
13. **Sobreuso de rayas largas (—)** — *"instituciones—no la gente—sin embargo esto continúa—"* → Usa comas o puntos
14. **Sobreuso de negritas** — *"OKRs, KPIs, BMC"* → *"OKRs, KPIs, BMC"*
15. **Listas verticales con encabezados en línea** — *"Rendimiento: El rendimiento mejoró"* → Convierte a prosa
16. **Mayúsculas de Título en Encabezados** — *"Negociaciones Estratégicas Y Asociaciones"* → *"Negociaciones estratégicas y asociaciones"*
17. **Emojis** — *"🚀 Fase de Lanzamiento: 💡 Insight Clave:"* → Elimina emojis
25. **Sobreuso de palabras con guión** — *"multifuncional, basado en datos, orientado al cliente"* → Elimina guiones en pares comunes

### Patrones de Comunicación
18. **Artefactos de chatbot** — *"¡Espero que esto te ayude! Hazme saber si..."* → Elimina completamente
19. **Disclaimers de corte de conocimiento** — *"Mientras que detalles son limitados en fuentes disponibles..."* → Encuentra fuentes o elimina
20. **Tono sicarifante** — *"¡Gran pregunta! ¡Tienes toda la razón!"* → Responde directamente

### Relleno y Exceso de Cautela
21. **Frases de relleno** — *"Con el propósito de"*, *"Debido al hecho de que"* → *"Para"*, *"Porque"*
22. **Exceso de cautela** — *"podría potencialmente posiblemente"* → *"puede"*
23. **Conclusiones genéricamente positivas** — *"El futuro se ve brillante"* → Planes o hechos específicos
24. **Comillas curvas** — *"el proyecto"* → *"el proyecto"*

---

## Ejemplo Completo

### Antes (suena a IA)

> ¡Gran pregunta! Aquí hay un ensayo sobre este tema. ¡Espero que esto te ayude!
>
> El desarrollo asistido por IA se erige como un duradero testamento del potencial transformador de los modelos de lenguaje grande, marcando un momento pivotal en la evolución del desarrollo de software. En el panorama tecnológico actual en rápida evolución, estas herramientas innovadoras—ubicadas en la intersección de la investigación y la práctica—están remodelando cómo los ingenieros idealizan, iteran y entregan, subrayando su papel vital en flujos de trabajo modernos.
>
> En su esencia, la propuesta de valor es clara: agilizar procesos, mejorar la colaboración y fomentar alineación. No es solo sobre autocompletado; es sobre desbloquear creatividad a escala, asegurando que las organizaciones puedan mantenerse ágiles mientras entregan experiencias fluidas, intuitivas y poderosas a los usuarios.
>
> Los observadores de la industria han notado que la adopción se ha acelerado desde experimentos aficionados hasta despliegues empresariales. La tecnología ha sido presentada en The New York Times, Wired y The Verge. Además, la capacidad de generar documentación, tests y refactorizaciones exhibe cómo la IA puede contribuir a mejores resultados.
>
> - 💡 Velocidad: La generación de código es significativamente más rápida
> - 🚀 Calidad: La calidad ha mejorado a través de entrenamiento mejorado
> - ✅ Adopción: El uso continúa creciendo
>
> A pesar de desafíos típicos de tecnologías emergentes, el ecosistema continúa prosperando. Para realizar plenamente este potencial, los equipos deben alinearse con mejores prácticas. En conclusión, el futuro se ve brillante. ¡Hazme saber si quieres que expanda alguna sección!

### Borrador reescrito

> Los asistentes de código impulsados por IA pueden acelerar las partes aburridas del trabajo. Son excelentes en boilerplate: archivos de configuración y el código pegajoso que no quieres escribir. También pueden ayudarte a esbozar un test, pero aún tienes que leerlo.
>
> La parte peligrosa es lo seguros que se ven los suggestions. He aceptado código que compiló y pasó lint, luego descubrí más tarde que se perdió el punto porque dejé de prestar atención.
>
> Si lo tratas como autocompletado y revisas cada línea, es útil. Si lo usas para evitar pensar, te ayudará a enviar bugs más rápido.
>
> El único respaldo real es los tests. Sin ellos, principalmente estás juzgando vibes.

### "¿Qué hace esto tan obviamente generado por IA?"

- Aún hay un énfasis demasiado en frases de apertura limpias
- La estructura sigue siendo un poco demasiado ordenada (contrastes limpios, párrafos paced uniformemente)
- El cierre se inclina un poco slogan-y en lugar de sonar como una persona hablando

### Reescritura final

> Los asistentes de código pueden hacer que seas más rápido en las partes aburridas. No en todo. Definitivamente no en arquitectura.
>
> Son excelentes en boilerplate: archivos de config, scaffolding de tests, refactorizaciones repetitivas. También son excelentes sonando correctos mientras están equivocados. He aceptado sugerencias que compilaron, pasaron lint, y aun así se perdieron el punto porque dejé de prestar atención.
>
> La gente con la que hablo tiende a caer en dos campos. Algunos la usan como autocompletado para tareas y revisan cada línea. Otros la desactivan después de que sigue sugiriendo patrones que no quieren. Ambos se sienten razonables.
>
> Las métricas de productividad son resbaladizas. GitHub puede decir que los usuarios de Copilot "aceptan el 30% de sugerencias," pero aceptación no es corrección, y corrección no es valor. Si no tienes tests, básicamente estás adivinando.

### Cambios realizados

- Eliminados artefactos de chatbot ("¡Gran pregunta!", "¡Espero que esto te ayude!", "Hazme saber si...")
- Eliminada inflación de significado ("testamento", "momento pivotal", "panorama en evolución", "papel vital")
- Eliminado lenguaje promocional ("innovador", "ubicado", "fluidas, intuitivas y poderosas")
- Eliminadas atribuciones vagas ("Observadores de la industria")
- Eliminadas frases superficiales en "-ando"/"-iendo" ("subrayando", "destacando", "reflejando", "contribuyendo a")
- Eliminado paralelismo negativo ("No es solo X; es Y")
- Eliminados patrones de regla de tres y reciclaje de sinónimos ("catalyst/partner/foundation")
- Eliminados rangos falsos ("de X a Y, de A a B")
- Eliminadas rayas largas, emojis, negritas de encabezados, y comillas curvas
- Eliminada evitación de cópula ("se erige como", "funciona como", "se configura como") a favor de "es"/"son"
- Eliminada sección formulaica de desafíos ("A pesar de desafíos... continúa prosperando")
- Eliminada cautela excesiva en disclaimers ("Mientras que detalles específicos son limitados...")
- Eliminado exceso de cautela ("podría potencialmente argumentarse que... podría tener algo")
- Eliminadas frases de relleno ("Para poder", "En esencia")
- Eliminada conclusión genéricamente positiva ("el futuro se ve brillante", "tiempos emocionantes se avecinan")
- Hecha la voz más personal y menos "armada" (ritmo variado, menos placeholders)

---

## Referencias

Esta skill se basa en [Wikipedia: Signos de escritura de IA](https://en.wikipedia.org/wiki/Talk:Artificial_intelligence/Archive_8#Signs_of_AI_writing), mantenida por WikiProject AI Cleanup. Los patrones documentados allí provienen de observaciones de miles de instancias de texto generado por IA en Wikipedia.

---

## Licencia

MIT License - Consulta [LICENSE](LICENSE) para detalles.

---

**Creado por:** Ale Tinto
**Versión:** 1.0.0
**Última actualización:** 2026
