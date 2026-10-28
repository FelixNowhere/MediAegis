# Proyecto Integrador Proyecto 2 (Red Bayesiana) - MediAegis

## Descripción
Este módulo implementa una Red Bayesiana para el diagnóstico médico probabilístico en el contexto del proyecto MediAegis. El objetivo es calcular la probabilidad posterior de que un paciente presente una determinada enfermedad clínica dado el reporte de un conjunto de síntomas clave observados (Fiebre, Tos, Dolor).

## Estructura de la Red
**Variables:**
- **Fiebre:** Presencia de temperatura corporal elevada. Estados: {No, Sí}.
- **Tos:** Presencia de reflejo de tos o afección respiratoria. Estados: {No, Sí}.
- **Dolor:** Presencia de dolor corporal o malestar generalizado. Estados: {No, Sí}.
- **Enfermedad:** Diagnóstico probable de la condición patológica. Estados: {No, Sí}.

**Dependencias:**
- `Fiebre` -> `Enfermedad`: La presencia de fiebre incrementa el riesgo de infección o enfermedad.
- `Tos` -> `Enfermedad`: La presencia de tos influye directamente en la probabilidad del cuadro patológico.
- `Dolor` -> `Enfermedad`: La presencia de dolor físico contribuye a la sospecha diagnóstica.

**Diagrama (DAG):**
```text
   [Fiebre]       [Tos]       [Dolor]
      \             |            /
       \            |           /
        v           v          v
              [Enfermedad]





USO DE AI
La AI fue utilizada para corroborar que se estuviera ejecutando el código de la mejor manera posible. También fue usada para corregir errores la ejecución en diferentes partes del proyecto. Gemini estudiantil fue usado, modelo 3.6 thinking en diversos prompts. 
