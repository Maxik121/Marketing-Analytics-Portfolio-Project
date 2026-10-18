# E-commerce Marketing Performance Dashboard in Looker Studio
![Status: In Progress](https://img.shields.io/badge/status-in%20progress-yellow?style=for-the-badge&logo=git)
---

>  **Kontekst akademicki:**  
> Projekt zrealizowany w ramach przedmiotu **Analiza danych o klientach: data-driven marketing**.  
> Celem projektu było zaprojektowanie wielowymiarowego dashboardu analitycznego w Google Looker Studio na podstawie danych Google Analytics 4 (Google Merchandise Store) oraz sformułowanie strategicznych rekomendacji optymalizacyjnych dla lejka marketingowego e-commerce.

---

## Przegląd projektu

Projekt stanowi kompleksowy audyt efektywności kanałów pozyskiwania ruchu i konwersji sklepu internetowego za okres od 1 stycznia 2025 do 1 czerwca 2026 roku[cite: 1]. Raport łączy makrometryki sprzedażowe z granularną analizą zachowań użytkowników w podziale na kanały akwizycji, demografię, geolokalizację oraz typy urządzeń[cite: 1, 2, 3].

### Kluczowe metryki globalne (High-Level KPIs)
* **Sesje ogółem:** 964 685[cite: 1]
* **Liczba konwersji:** 922 154[cite: 1]
* **Zdarzenia na sesję (Events per session):** 14,43[cite: 1]
* **Całkowity przychód (Total revenue):** $2,38 mln[cite: 1]

---

## 🛠️ Architektura dashboardu

Repozytorium zawiera trzystronicowy interaktywny raport analityczny:

### 1. Przegląd kanałów marketingowych (`01_overview.png`)
![Przegląd kanałów marketingowych](assets/01_overview.png)

* **Rozkład ruchu vs. konwersji:** Zestawienie udziału poszczególnych kanałów (Direct, Organic Search, Paid Search, Referral, Email, Cross-network, Organic Social) w wolumenie sesji i wygenerowanych celach biznesowych[cite: 1].
* **Dynamika czasowa:** Wykres liniowy prezentujący stabilność i sezonowość konwersji w domyślnych grupach kanałów w analizowanym okresie[cite: 1].
* **Profil demograficzny:**
  * Najsilniejsza grupa wiekowa generująca konwersje: **25–34 lata** (ponad 140 tys. konwersji), a następnie **18–24 lata** (ok. 120 tys.)[cite: 1].
  * Rozkład płciowy w kanałach ruchu z dominacją użytkowników niezidentyfikowanych (*unknown*) oraz mężczyzn w kanałach bezpośrednich i organicznych[cite: 1].
* **Efektywność SEO:** Granularne zestawienie wyszukiwarek organicznych (Google, Yahoo, Baidu) z metrykami sesji, engagement rate i przychodu[cite: 1].

---

### 2. Search Engine Marketing / Google Ads Deep Dive (`02_sem_analysis.png`)
![SEM Analysis](assets/02_sem_analysis.png)

* **Geografia ruchu płatnego:** Szczegółowa segmentacja użytkowników pozyskanych z płatnych wyników Google w podziale na miasta USA (m.in. Nowy Jork, San Francisco, Mountain View, Los Angeles)[cite: 2].
* **Wyniki kampanii i grup reklam:**
  * Łączna liczba kliknięć: **343 237** przy ponad **23,4 mln wyświetleń** (średni CTR: **1,47%**)[cite: 2].
  * Całkowity koszt kampanii (Spend): **$168 329,37** przy średnim CPC na poziomie **$0,49**[cite: 2].
  * Wygenerowany przychód SEM: **$2 405 227,02** z łączną liczbą 922 069 konwersji[cite: 2].
* **Słowa kluczowe i zapytania (Search terms):**
  * Słowa dopasowane do frazy (*Phrase match*) oraz ścisłe (*Exact match*), m.in. z klastrów odzieżowych (*hoodies*, *Google T-shirt*)[cite: 2].
  * Wysoki współczynnik konwersji (ponad 70%) zapytań o charakterze stricte brandowym (np. *google merchandise*, *youtube merchandise*)[cite: 2].
* **Top produkty kupowane przez ruch z SEM:** Artykuły brandowe YouTube i Google (odzież, akcesoria, gadżety)[cite: 2].

---

### 3. Email Marketing & Newsletter Performance (`03_email_performance.png`)
![Email Performance](assets/03_email_performance.png)

* **Wkład w e-commerce:** Subskrybenci newslettera wygenerowali **$128,13 tys.** bezpośredniego przychodu[cite: 3].
* **Efektywność kampanii wysyłkowych:** Analiza wolumenu sesji, liczby odsłon oraz transakcji dla poszczególnych edycji newslettera (m.in. edycje jesienne *Fall V1*, holidayowe czy back-to-school)[cite: 3].
* **Segmentacja urządzeń:** Wyraźna dysproporcja platformowa – ponad **21,7 tys. sesji** oraz niemal cały wolumen przychodów pochodzi z urządzeń desktopowych, podczas gdy ruch mobile odpowiadał za niespełna 2 tys. sesji[cite: 3].
* **Rozkład tygodniowy (Day of week):**
  * Najwyższe zaangażowanie i wolumen transakcji przypada na środek tygodnia (czwartek i środa)[cite: 3].
  * Wyraźny spadek otwieralności i konwersji w dniach weekendowych (sobota: 401 sesji)[cite: 3].
* **Zasięg geograficzny:** Dominacja rynku północnoamerykańskiego (USA, Kanada), z rosnącym zaangażowaniem rynków azjatyckich (Singapur) i europejskich[cite: 3].

---

## 💡 Główne wnioski i rekomendacje biznesowe

1. **Skalowanie kampanii brandowych w Google Ads:**
   * Zapytania brandowe cechują się bardzo wysokim współczynnikiem konwersji (74%+) oraz relatywnie niskim kosztem CPC ($0,49)[cite: 2]. Rekomenduje się zabezpieczenie pełnego udziału w wyświetleniach (Impression Share) na frazy związane z marką.
2. **Optymalizacja harmonogramu wysyłek Email Marketingu:**
   * Dane jednoznacznie wskazują, że subskrybenci realizują zakupy w dni robocze na komputerach stacjonarnych[cite: 3]. Należy zoptymalizować okna wysyłkowe na wtorki–czwartki w godzinach porannych i biznesowych, ograniczając komunikację weekendową.
3. **Audyt ścieżki mobilnej dla kanału Email:**
   * Niski udział konwersji mobilnych w newsletterze przy znacznym ruchu sugeruje potencjalne bariery UX/UI w responsywności szablonów mailingowych lub na samym checkoutcie w widoku mobilnym[cite: 3].
4. **Personalizacja oferty pod dominujący segment wiekowy (25–34 lata):**
   * Grupa ta generuje największy wolumen konwersji[cite: 1]. Komunikacja wizualna i promocje produktowe w kanałach paid social i display powinny być profilowane pod preferencje tego segmentu.

---

## 📂 Struktura repozytorium

```text
├── assets/                  
│   ├── 01_overview.png
│   ├── 02_sem_analysis.png
│   └── 03_email_performance.png
├── reports/                 
│   └── Marketing_Analytics_Report.pdf
└── README.md                
