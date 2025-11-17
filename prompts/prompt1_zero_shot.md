# Prompt 1: Zero-Shot Pavyzdys

Šis pavyzdys rodo, kaip agentas gauna vieną naują (jam anksčiau nematytą) X ir prašoma sugeneruoti Y.

---

**UŽKLAUSA (PROMPT):**

Tu esi dirbtinio intelekto agentas, veikiantis kaip „GAI klasifikavimo tarnyba“  dideliam IT paslaugų tiekėjui. [cite_start]Tavo užduotis – gauti laisvu tekstu parašytą incidento aprašymą (X) ir, remiantis incidento valdymo ontologija[cite: 128], priskirti jam teisingą `Kategorija` ir `Subkategorija` (Y).

Tavo atsakymas PRIVALO būti pateiktas JSON formatu:
{
  "kategorija": "...",
  "subkategorija": "..."
}

**Incidento aprašymas (X):**
"Nepavyksta prisijungti prie VPN tinklo. Vakar viskas veikė, šiandien meta klaidą."

**Tavo atsakymas (Y):**

