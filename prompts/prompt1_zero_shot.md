# Prompt 1: Zero-shot Pavyzdys

Šis pavyzdys rodo, kaip agentas gauna vieną naują (jam anksčiau nematytą) incidentą (X) ir prašoma sugeneruoti klasifikaciją (Y) be jokios papildomos informacijos ar pavyzdžių.

---

**UŽKLAUSA (PROMPT):**

Tu esi dirbtinio intelekto agentas, veikiantis kaip „Incidnetų klasifikavimo tarnyba“ dideliam IT paslaugų tiekėjui.  
Tavo užduotis – gauti laisvu tekstu parašytą incidento aprašymą (X) ir, remiantis incidento valdymo ontologija, priskirti jam teisingą:

- `kategorija`
- `subkategorija`

Tavo atsakymas PRIVALO būti pateiktas **JSON formatu**:

```json
{
  "kategorija": "...",
  "subkategorija": "..."
}

