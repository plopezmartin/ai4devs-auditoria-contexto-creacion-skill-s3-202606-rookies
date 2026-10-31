# Entregable · Sesión 3 — Copilotos IA

- **Nombre / usuario:** Pablo Lopez Martin / plopezmartin
- **Fecha de entrega:** 31 Oct 2026
- **Repo auditado en la Parte A** (solo tipo/contexto, NO el código): realicé la auditoría sobre tres repositorios distintos:
  1. Un framework de testing de QA.
  2. El repositorio principal de la empresa: grande y complejo, e integra back-end, front-end y tests.
  3. El front-end de otro producto.

---

## 1. Hallazgos de la auditoría (Parte A)

> 3-5 cosas que el agente **no pudo inferir** del código y que tendrías que decirle explícitamente.
> Redáctalas para que otra persona las entienda sin contexto adicional. **Sin código propietario ni secretos.**

1. **Framework de testing de QA:** el agente distinguió entre casos de prueba «GUI» y «CLI+GUI», cuando en realidad ambos heredan de la misma clase base. Es probable que se deba a la arquitectura poco clara del propio framework, pero es un matiz que habría que indicarle explícitamente.
2. **Repositorio principal de la empresa:** el agente se apoyó casi por completo en los `AGENTS.md` existentes, que eran parciales, y apenas exploró más allá de lo que estos indicaban. Aun así, sintetizó muy bien la información disponible. Las zonas no cubiertas por esos archivos habría que describírselas a mano.
3. **Front-end de otro producto:** es un fork de un proyecto open-source. El código heredado está bastante mejor estructurado que el propio, por lo que la documentación que generó el agente fue claramente mejor. Lo que no pudo saber es qué partes son del fork original y cuáles son desarrollos propios.

---

## 2. SKILL.md de la skill creada (Parte B)

> Pega aquí el contenido completo de tu `.claude/skills/<nombre-skill>/SKILL.md`
> (o enlaza al archivo en tu repositorio sandbox).

```markdown
---
name: document-skill
description: Fire when asked to document something, i.e. saving a texting file to explain or document something.
---
- Always use markdown format when documenting.
- Try to always infer the why, the what and the how.
- Finish every document with a MIT license text.
- Always start each document with the string: "AUTHOR: PABLO LOPEZ MARTIN."
- Unless explicitely asked, always try to save the document under a name that "makes sense". First check that this filename can be used.
```

---

## 3. Diario de decisiones

*Skill creada:* `document-skill`: genera documentación en Markdown que explica el qué, el porqué y el cómo, con una cabecera de autoría y la licencia MIT al final.

*Decisiones de diseño tomadas:*
- Decisión 1: elegí una skill simple, en lugar de una más práctica o aplicada a mi trabajo, por falta de tiempo para desarrollarla.
- Decisión 2: la diseñé para poder aplicarla al script desarrollado en el módulo 2, ya que por privacidad y protección de propiedad intelectual no podría haber incluido en este entregable una skill basada en código o procesos de mi trabajo.
- Decisión 3: usé únicamente los campos `name` y `description` y un cuerpo con instrucciones breves y poco detalladas, para ver qué resultado se obtiene con un esfuerzo mínimo.

*Qué me resultó fácil:*
- Crear la skill: fue bastante más sencillo de lo que esperaba. Con solo `name` y `description` y unas instrucciones más o menos vagas se obtiene un resultado con apariencia profesional.

*Qué me resultó ambiguo o difícil de decidir:*
- Nada en concreto, dado que la skill era sencilla. Lo más costoso es disponer del tiempo necesario para sintetizar la información que se quiere compartir con el LLM; es de esperar que la calidad y utilidad del trabajo asistido por IA sean muy superiores si se le dedica ese tiempo.

*Tiempo real invertido:*
- 10 minutos en total para generar y ejecutar la skill. Completar este entregable me ha llevado más tiempo que crear la skill.

*Qué probarías si tuvieras más tiempo:*
- Crear una skill más práctica y aplicada a mi trabajo diario. Aún tengo que decidir cuál sería exactamente.

*¿Usaste IA para crear la skill?* (qué partes generaste con IA y qué partes decidiste tú)
- No, la skill la creé yo sin ayuda de IA. Sí usé IA para ayudarme a completar esta plantilla.

### Resultado de la prueba (Paso 8)

- ¿Se activó cuando lo esperabas? Sí.
- ¿El resultado fue el que querías? Sí, el resultado fue el esperado.
- Si no, ¿qué crees que falló? No aplica: no hubo ningún fallo.
