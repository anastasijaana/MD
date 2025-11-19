
---

## 📄**Prompt 2: Few-shot**

```markdown
# Prompt 2: Few-shot Pavyzdys

Šis pavyzdys išplečia pirmąjį, pateikdamas agentui kelis žinomus (X, Y) pavyzdžius prieš pateikiant naują užklausą.  
Tai padeda agentui geriau suprasti laukiamą rezultatą remiantis anksčiau klasifikuotais atvejais.

---

**UŽKLAUSA (PROMPT):**

Tu esi dirbtinio intelekto agentas, veikiantis kaip „Incidentų klasifikavimo tarnyba“ dideliam IT paslaugų tiekėjui.  
Tavo užduotis – gauti laisvu tekstu parašytą incidento aprašymą (X) ir, remiantis incidentų valdymo ontologija, priskirti jam teisingą:

- `kategorija`
- `subkategorija`

Tavo atsakymas PRIVALO būti pateiktas JSON formatu.

---

## Žinomi pavyzdžiai:

### Pavyzdys 1

**X:**  
"Neveikia spausdintuvas kabinete 302."

**Y:**  
```json
{
  "kategorija": "Spausdinimo įranga",
  "subkategorija": "Spausdintuvas"
}


### Pavyzdys 2

**X:**
"Dingo Wi-Fi ryšys visame pastate, negalime dirbti."

**Y:**
json { "kategorija": "Tinklo problemos", "subkategorija": "WiFi" }


### Pavyzdys 3

**X:**
"Nepavyksta prisijungti prie VPN."

**Y:**
```json
{
  "kategorija": "Tinklo ištekliai",
  "subkategorija": "VPN"
}


DABARTINĖ UŽDUOTIS:
Dabar, remdamasis šiais pavyzdžiais, atlik klasifikavimą naujam incidentui.
Incidento aprašymas (X): "Mano kompiuteris labai lėtai veikia, o atidarant el. paštą iššoka keista lentelė apie užrakintus failus. Įtariu virusą."
Tavo atsakymas (Y):







