# E-commerce Marketing Performance Dashboard in Looker Studio
![Status: Completed](https://img.shields.io/badge/status-completed-brightgreen?style=for-the-badge&logo=git)
---

>  **Kontekst akademicki:**  
> Projekt zrealizowany w ramach przedmiotu **Analiza danych o klientach: data-driven marketing**.  
> Celem projektu było zaprojektowanie wielowymiarowego dashboardu analitycznego w Google Looker Studio na podstawie danych Google Analytics 4 (Google Merchandise Store) oraz sformułowanie strategicznych rekomendacji optymalizacyjnych dla lejka marketingowego e-commerce.

---

## Przegląd projektu

Projekt stanowi kompleksowy audyt efektywności kanałów pozyskiwania ruchu i konwersji sklepu internetowego za okres od 1 stycznia 2025 do 1 czerwca 2026 roku. Raport łączy makrometryki sprzedażowe z granularną analizą zachowań użytkowników w podziale na kanały akwizycji, demografię, geolokalizację oraz typy urządzeń.

### Kluczowe metryki globalne (High-Level KPIs)
* **Sesje ogółem:** 964 685
* **Liczba konwersji:** 922 154
* **Zdarzenia na sesję (Events per session):** 14,43
* **Całkowity przychód (Total revenue):** $2,38 mln
<img width="762" height="94" alt="image" src="https://github.com/user-attachments/assets/94d39138-d545-44d3-b96b-583c392aa773" />
<img width="1012" height="274" alt="image" src="https://github.com/user-attachments/assets/7a732940-b633-4368-a518-5e07e1e037ab" />


---

## 🛠️ Architektura dashboardu

Repozytorium zawiera trzystronicowy interaktywny raport analitycznym dostepny pod poniższym linkiem:<br>
[E-commerce_Marketing_Performance_Dashboard ](http://https://datastudio.google.com/s/goIOb6qmjZU "E-commerce_Marketing_Performance_Dashboard ")

### 1. Przegląd kanałów marketingowych

* **Rozkład ruchu vs. konwersji:** Zestawienie udziału poszczególnych kanałów (Direct, Organic Search, Paid Search, Referral, Email, Cross-network, Organic Social) w wolumenie sesji i wygenerowanych celach biznesowych.
* **Dynamika czasowa:** Wykres liniowy prezentujący stabilność i sezonowość konwersji w domyślnych grupach kanałów w analizowanym okresie.
* **Profil demograficzny:**
  * Najsilniejsza grupa wiekowa generująca konwersje: **25–34 lata** (ponad 140 tys. konwersji), a następnie **18–24 lata** (ok. 120 tys.).
  * Rozkład płciowy w kanałach ruchu z dominacją użytkowników niezidentyfikowanych (*unknown*) oraz mężczyzn w kanałach bezpośrednich i organicznych.
* **Efektywność SEO:** Granularne zestawienie wyszukiwarek organicznych (Google, Yahoo, Baidu) z metrykami sesji, engagement rate i przychodu.

---

### 2. Search Engine Marketing / Google Ads Deep Dive [0.1.SEM_EMPDF](http://https://github.com/Maxik121/Marketing-Analytics-Portfolio-Project/blob/main/assets/0.1.SEM_EMPD.pdf "0.1.SEM_EMPDF")

* **Geografia ruchu płatnego:** Szczegółowa segmentacja użytkowników pozyskanych z płatnych wyników Google w podziale na miasta USA (m.in. Nowy Jork, San Francisco, Mountain View, Los Angeles).
* **Wyniki kampanii i grup reklam:**
  * Łączna liczba kliknięć: **343 237** przy ponad **23,4 mln wyświetleń** (średni CTR: **1,47%**).
  * Całkowity koszt kampanii (Spend): **$168 329,37** przy średnim CPC na poziomie **$0,49**.
  * Wygenerowany przychód SEM: **$2 405 227,02** z łączną liczbą 922 069 konwersjii.
* **Słowa kluczowe i zapytania (Search terms):**
  * Słowa dopasowane do frazy (*Phrase match*) oraz ścisłe (*Exact match*), m.in. z klastrów odzieżowych (*hoodies*, *Google T-shirt*).
  * Wysoki współczynnik konwersji (ponad 70%) zapytań o charakterze stricte brandowym (np. *google merchandise*, *youtube merchandise*).
* **Top produkty kupowane przez ruch z SEM:** Artykuły brandowe YouTube i Google (odzież, akcesoria, gadżety).

---

### 3. Email Marketing & Newsletter Performance [0.2. E-mail_Marketing_EMPDF](http://https://github.com/Maxik121/Marketing-Analytics-Portfolio-Project/blob/main/assets/02.Email-Marketing_EMPD.pdf "0.2. E-mail_Marketing_ED")

* **Wkład w e-commerce:** Subskrybenci newslettera wygenerowali **$128,13 tys.** bezpośredniego przychodu.
* **Efektywność kampanii wysyłkowych:** Analiza wolumenu sesji, liczby odsłon oraz transakcji dla poszczególnych edycji newslettera (m.in. edycje jesienne *Fall V1*, holidayowe czy back-to-school).
* **Segmentacja urządzeń:** Wyraźna dysproporcja platformowa – ponad **21,7 tys. sesji** oraz niemal cały wolumen przychodów pochodzi z urządzeń desktopowych, podczas gdy ruch mobile odpowiadał za niespełna 2 tys. sesji.
* **Rozkład tygodniowy (Day of week):**
  * Najwyższe zaangażowanie i wolumen transakcji przypada na środek tygodnia (czwartek i środa).
  * Wyraźny spadek otwieralności i konwersji w dniach weekendowych (sobota: 401 sesji).
* **Zasięg geograficzny:** Dominacja rynku północnoamerykańskiego (USA, Kanada), z rosnącym zaangażowaniem rynków azjatyckich (Singapur) i europejskich.
<img width="620" height="262" alt="image" src="https://github.com/user-attachments/assets/391805a4-9eaa-4ef4-a595-e734599456f0" />
<img width="444" height="270" alt="image" src="https://github.com/user-attachments/assets/16a660b3-4b38-48ed-ad76-7e26b011300a" />


---

## 💡 Główne wnioski i rekomendacje biznesowe

1. **Skalowanie kampanii brandowych w Google Ads:**
   * Zapytania brandowe cechują się bardzo wysokim współczynnikiem konwersji (74%+) oraz relatywnie niskim kosztem CPC ($0,49). Rekomenduje się zabezpieczenie pełnego udziału w wyświetleniach (Impression Share) na frazy związane z marką.
2. **Optymalizacja harmonogramu wysyłek Email Marketingu:**
   * Dane wskazują, że subskrybenci realizują zakupy w dni robocze na komputerach stacjonarnych. Należy zoptymalizować okna wysyłkowe na wtorki i czwartki w godzinach porannych oraz godzinach pracy, ograniczając komunikację weekendową.
3. **Audyt ścieżki mobilnej dla kanału Email:**
   * Niski udział konwersji mobilnych w newsletterze przy znacznym ruchu sugeruje potencjalne bariery UX/UI w responsywności szablonów mailingowych lub na samym checkoutcie w widoku mobilnym.
4. **Personalizacja oferty pod dominujący segment wiekowy (25-34 lata):**
   * Grupa ta generuje największy wolumen konwersjii. Komunikacja wizualna i promocje produktowe w kanałach paid social i display powinny być profilowane pod preferencje tego segmentu.

---

## 📂 Struktura repozytorium

```text

├── assets/
│   ├── 01.SEM_EMPD.png
│   └── 0.2.Email-Marketing_EMPD.png
│
├── reports/
│   └── Marketing_Analytics_Report.pdf
│
└── README.md             
