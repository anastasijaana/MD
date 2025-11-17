# Prompt 2: Few-Shot Pavyzdys

[cite_start]Šis pavyzdys išplečia pirmąjį, pateikdamas agentui kelis žinomus (X, Y) pavyzdžius [cite: 191] prieš pateikiant naują užklausą. Tai padeda agentui geriau suprasti laukiamą rezultatą.

---

**UŽKLAUSA (PROMPT):**

[cite_start]Tu esi dirbtinio intelekto agentas, veikiantis kaip „GAI klasifikavimo tarnyba“  dideliam IT paslaugų tiekėjui. [cite_start]Tavo užduotis – gauti laisvu tekstu parašytą incidento aprašymą (X) ir, remiantis incidento valdymo ontologija[cite: 128], priskirti jam teisingą `Kategorija` ir `Subkategorija` (Y).

Tavo atsakymas PRIVALO būti pateiktas JSON formatu.

Štai keli pavyzdžiai, kaip tu atlieki šią užduotį:

**Pavyzdys 1:**
* [cite_start]**X (Aprašymas):** "Neveikia spausdintuvas kabinete 302." 
* **Y (Rezultatas):**
    {
      "kategorija": "Spausdinimo įranga",
      "subkategorija": "Spausdintuvas"
    } 

**Pavyzdys 2:**
* [cite_start]**X (Aprašymas):** "Dingo Wi-Fi ryšys visame pastate, negalime dirbti." 
* **Y (Rezultatas):**
    {
      "kategorija": "TinkloProblemos",
      "subkategorija": "WiFiProblem"
    [cite_start]} 

**Pavyzdys 3:**
* [cite_start]**X (Aprašymas):** "Nepavyksta prisijungti prie VPN" 
* **Y (Rezultatas):**
    {
      "kategorija": "TinkloIštekliai",
      "subkategorija": "VPN"
    [cite_start]} 

---

**DABARTINĖ UŽDUOTIS:**

Dabar, remdamasis šiais pavyzdžiais, atlik klasifikavimą naujam incidentui.

**Incidento aprašymas (X):**
"Mano kompiuteris labai lėtai veikia, o atidarant el. paštą iššoka keista lentelė apie užrakintus failus. Įtariu virusą."

**Tavo atsakymas (Y):**
