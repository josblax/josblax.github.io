# Práctica de Laboratorio: Selección Multicriterio del Empleo Ideal mediante AHP

## 1. Contexto del Caso
Al concluir sus estudios universitarios, un graduado en ingeniería, tecnología o ciencia de datos se enfrenta a múltiples ofertas laborales que difieren radicalmente en su naturaleza. A diferencia de una decisión basada únicamente en el salario, elegir dónde trabajar requiere sopesar factores personales, profesionales y geográficos. 

El objetivo de esta práctica es aplicar el Proceso Analítico Jerárquico (AHP) para evaluar cuantitativamente y seleccionar la mejor opción laboral entre tres opciones reales o simuladas.

---

## 2. Definición del Modelo Jerárquico
* **Objetivo:** Seleccionar la mejor opción de empleo al egresar de la universidad.
* **Criterios de Evaluación ($n = 4$):**
  1. **$C_1$ - Compensación y Beneficios:** Salario base, bonos de desempeño, seguro médico y prestaciones.
  2. **$C_2$ - Tipo de Industria:** Sector de actividad de la empresa (ej. Fintech, Consultoría Global, Startup de IA, Sector Público).
  3. **$C_3$ - Geografía y Modalidad:** Ubicación física, costo de vida local, opciones de trabajo remoto o híbrido.
  4. **$C_4$ - Oportunidad de Crecimiento:** Planes de carrera, capacitación técnica continua y mentoría.

---

## 3. Enunciado y Consignas para el Estudiante

### Parte A: Ponderación de los Criterios (Matriz $4 \times 4$)
Construye una matriz de comparaciones pareadas utilizando la escala fundamental de Saaty para ponderar los 4 criterios anteriores. 
* *Instrucción de diseño:* Define tus propios juicios de valor justificando tus prioridades personales (por ejemplo, si para ti el crecimiento profesional es mucho más importante que la geografía, o si la compensación supera a la industria).
* *Requerimiento matemático:* 
  1. Calcula la suma de columnas y normaliza la matriz.
  2. Obtén el **vector de prioridad** (pesos porcentuales de cada criterio).
  3. Calcula el valor propio máximo ($\lambda_{max}$), el Índice de Consistencia ($CI$) y la **Tasa de Consistencia ($CR$)**, utilizando obligatoriamente el factor de Índice Aleatorio para 4 variables (**$RI = 0.90$**).
  4. Verifica que tu matriz cumpla con la regla de consistencia ($CR < 0.1$). Si no se cumple, ajusta tus juicios hasta lograrlo.

### Parte B: Evaluación de las Alternativas
Supongamos tres ofertas laborales ficticias o reales analizadas bajo los criterios anteriores:
* **Alternativa 1 (Opción A):** Multinacional de Consultoría en la capital (Alta compensación, industria tradicional, presencial estricto, crecimiento moderado).
* **Alternativa 2 (Opción B):** Startup de Inteligencia Artificial en el extranjero o remota (Compensación variable en acciones/equity, industria de punta, 100% remoto, crecimiento explosivo).
* **Alternativa 3 (Opción C):** Empresa del sector financiero local / Fintech (Compensación competitiva, sector financiero, modelo híbrido, crecimiento estructurado).

* *Instrucción:* Evalúa las tres alternativas frente a cada uno de los 4 criterios construyendo matrices secundarias de $3 \times 3$ (o asignando los vectores de puntuación obtenidos mediante AHP). Multiplica los vectores locales de las alternativas por el vector de prioridad global de los criterios obtenido en la Parte A para obtener la **puntuación global final**.

### Parte C: Conclusión Ejecutiva y Reflexión
* Redacta un reporte de una cuartilla donde respondas: ¿Coincide la opción ganadora del modelo matemático con tu intuición inicial antes de hacer el ejercicio? ¿Cómo afectó la restricción de consistencia ($CR < 0.1$) a la forma en que evaluaste tus preferencias personales?

---

## 4. Soluciones Aplicando Criterios Diferentes (Casos Prácticos de Alumnos)

Para enriquecer el ejercicio y mostrar cómo dos perfiles estudiantiles distintos llegan a decisiones completamente opuestas utilizando la misma metodología AHP, se presentan los siguientes dos perfiles de resolución:

### Peril 1: "El Buscador de Estabilidad y Crecimiento Técnico"
* **Perfil:** Un graduado enfocado puramente en acelerar su curva de aprendizaje técnico y maximizar su compensación a corto plazo, sin importarle la presencialidad o el sector tradicional.
* **Vector de Prioridad (Criterios normalizados):**
  * Peso de Compensación ($W_1$): **$0.415$** (41.5%)
  * Peso de Crecimiento ($W_2$): **$0.415$** (41.5%)
  * Peso de Industria ($W_3$): **$0.115$** (11.5%)
  * Peso de Geografía ($W_4$): **$0.055$** (5.5%)
  * *Verificación de Consistencia:* Con $RI = 0.90$ para 4 variables, su cálculo arroja un **$CR = 0.048$** ($< 0.1$), por lo que los juicios son perfectamente coherentes.

* **Evaluación de Alternativas y Resultado Final:**
  * **Opción A (Multinacional de Consultoría - Alta compensación, presencial):** **$0.485$** (48.5%)
  * **Opción C (Fintech local - Compensación competitiva, híbrido):** **$0.362$** (36.2%)
  * **Opción B (Startup en el extranjero - Remoto, compensación variable):** **$0.153$** (15.3%)

> **Conclusión Perfil 1:** Su opción ganadora es la **Opción A (Multinacional de Consultoría)**. Su modelo matemático refleja que al priorizar fuertemente la compensación y el crecimiento estructurado, las desventajas de la presencialidad o la industria tradicional pasan a un segundo plano.

---

### Perfil 2: "El Defensor de la Flexibilidad y Calidad de Vida"
* **Perfil:** Un graduado que prioriza la libertad geográfica (trabajo remoto), trabajar en industrias tecnológicas disruptivas y evitar el desgaste de las grandes corporaciones tradicionales.
* **Vector de Prioridad (Criterios normalizados):**
  * Peso de Crecimiento ($W_1$): **$0.442$** (44.2%)
  * Peso de Geografía/Modalidad ($W_2$): **$0.263$** (26.3%)
  * Peso de Industria ($W_3$): **$0.187$** (18.7%)
  * Peso de Compensación ($W_4$): **$0.108$** (10.8%)
  * *Verificación de Consistencia:* Utilizando $RI = 0.90$, su tasa de consistencia resulta en **$CR = 0.072$** ($< 0.1$), cumpliendo con la validez analítica.

* **Evaluación de Alternativas y Resultado Final:**
  * **Opción B (Startup de IA - 100% remoto, crecimiento explosivo):** **$0.591$** (59.1%)
  * **Opción C (Fintech local - Modelo híbrido, crecimiento estructurado):** **$0.284$** (28.4%)
  * **Opción A (Multinacional de Consultoría - Presencial estricto):** **$0.125$** (12.5%)

> **Conclusión Perfil 2:** Su opción ganadora es de forma contundente la **Opción B (Startup de IA)**. El modelo demuestra cómo un cambio en los pesos iniciales (otorgando mayor valor a la modalidad remota y al crecimiento en tecnología punta) desplaza por completo a la multinacional tradicional al fondo de sus preferencias.
