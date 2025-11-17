# Prompt 1 – Zero-shot Example

## 🧠 Kontekstas:
Jūs esate dirbtinio intelekto agentas, skirtas IT incidentų valdymui. Jūsų užduotis – analizuoti incidento aprašymą ir priskirti jį tinkamai ontologijos kategorijai bei subkategorijai.

## 🎯 Užduotis (Input X):
Incidentas: „Nepavyksta prisijungti prie e. sveikatos sistemos, sistema užstrigo.“

Papildoma informacija:
- Pranešėjas: gyventojas
- Prioritetas: aukštas
- Data: 2025-10-01
- Skubumas: skubus

## 🤖 Jūsų veiksmai:
1. Suprask pateiktą tekstą (natural language understanding).
2. Remiantis turima ontologija, priskirk tinkamą kategoriją ir subkategoriją.
3. Nurodyk tinkamą vykdytojo grupę ar rolę.
4. Pateik rezultatą struktūrizuotu formatu (JSON).

## ✅ Laukiamas rezultatas (Output Y):
```json
{
  "category": "Programinė įranga",
  "subcategory": "E. sveikata",
  "assignee_group": "IT Servisas"
}
