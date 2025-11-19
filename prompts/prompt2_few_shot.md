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
```


### Pavyzdys 2
**X:**
"Dingo Wi-Fi ryšys visame pastate, negalime dirbti."

**Y:**
```json
{
  "kategorija": "Tinklo problemos",
  "subkategorija": "WiFi"
}
```

### Pavyzdys 3
**X:**
"Nepavyksta prisijungti prie VPN."

**Y:**
```json
{
  "kategorija": "Tinklo ištekliai",
  "subkategorija": "VPN"
}
```

Tai yra labai dažna klaida dirbant su Markdown formatu. Tekstas rodomas raudonai, nes neuždarei kodo blokų.

GitHub (ir kiti redaktoriai) naudoja tris kablelius (```) kodo pradžiai ir būtinai tris kablelius kodo pabaigai. Jei pamiršti parašyti uždarymo ženklus (```), GitHub galvoja, kad visas likęs failo tekstas yra to paties kodo dalis. Kadangi paprastas tekstas nėra validus JSON kodas, jis pažymimas raudonai kaip klaida.

Štai kas buvo negerai tavo tekste:

Pavyzdys 1: Atidarei ```json, bet po JSON kodo nepadėjai ```.

Pavyzdys 2: Parašei tiesiog json { ... } be jokių kabučių – tai neveiks kaip kodo blokas.

Formatavimas: Trūksta tuščių eilučių tarp blokų, todėl Markdown gali "susipainioti".

✅ Ištaisytas kodas (Kopijuok ir įklijuok šį visą tekstą):
Ši versija bus tvarkinga, gražiai nuspalvinta ir be raudonų klaidų:

Markdown

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
```

Pavyzdys 2
X: "Dingo Wi-Fi ryšys visame pastate, negalime dirbti."

Y:

```json
{
  "kategorija": "Tinklo problemos",
  "subkategorija": "WiFi"
}
```

Pavyzdys 3
X: "Nepavyksta prisijungti prie VPN."

Y:
```json
{
  "kategorija": "Tinklo ištekliai",
  "subkategorija": "VPN"
}
```

DABARTINĖ UŽDUOTIS:
Dabar, remdamasis šiais pavyzdžiais, atlik klasifikavimą naujam incidentui.
Incidento aprašymas (X): "Mano kompiuteris labai lėtai veikia, o atidarant el. paštą iššoka keista lentelė apie užrakintus failus. Įtariu virusą."
Tavo atsakymas (Y):

