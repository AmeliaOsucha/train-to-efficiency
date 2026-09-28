### train-to-efficiency
## MY FULL CHAPTER: https://books.google.pl/books?id=x9QAEgAAQBAJ&newbks=0&lpg=PA99&dq=Analiza%20ilo%C5%9Bciowa%20wybranych%20problem%C3%B3w%20z%20zakresu%20ekonomii%20i%20finans%C3%B3w&hl=pl&pg=PA219#v=onepage&q&f=false 
## Założenia i wyniki niniejszego badania przedstawiono w maju 2026 roku podczas ogólnopolskiej konferencji Narzędzia Analityczne w Naukach Ekonomicznych (NAWNE)
---
Project TL;DR (for recruiters): Evaluation of Subcarpathian Metropolitan Railway (PKA)
### Main Goal: To evaluate the impact of the PKA railway system on passenger stop efficiency and ridership growth between 2021 and 2024, addressing attribution challenges using a control group.
### Methods:
* Multivariate Statistical Analysis: Constructed a synthetic efficiency index based on stimulants and destimulants (equal weight framework with robustness checks).
* Econometric Approach: Conducted a comparative analysis with a control group (reference railway line no. 68).
* Statistical Testing: Performed normality checks (Shapiro-Wilk test) and non-parametric group comparisons (Mann-Whitney U test / Wilcoxon tests) using R and Excel.
### Result: Quantified the net performance uplift of PKA stations over the control group, demonstrating statistically great improvements in passenger turnover. (Presented at the NAWNE 2026 conference).

---

### Ewaluacja efektywności przystanków osobowych w kontekście wdrożenia Podkarpackiej Kolei Aglomeracyjnej (PKA) / Evaluation of Passenger Stop Efficiency in the Context of the Subcarpathian Metropolitan Railway (PKA) Implementation

Projekt badawczy poświęcony analizie zmian na stacjach kolejowych na Podkarpaciu (ze szczególnym uwzględnieniem tras PKA oraz odcinka referencyjnego).

*A research project dedicated to analyzing changes in railway stations in the Subcarpathian Voivodeship (with a particular focus on PKA routes and a reference section).*

---

## Zawartość repozytorium / Repository Contents

1. **`analiza_PKA.R`** - skrypt w języku R odpowiedzialny za przetwarzanie danych, normalizację zmiennych (unitaryzację) oraz obliczanie syntetycznego miernika efektywności.  
   *(The R script responsible for data processing, variable normalization (unitary), and calculating the synthetic efficiency measure.)*

2. **`dane_pociag.xlsx`** - arkusz kalkulacyjny zawierający surowe dane statystyczne, zestawienia z portalu UTK, GUS / Spis Powszechny oraz obliczenia pośrednie dla lat 2021 i 2024.  
   *(The spreadsheet containing raw statistical data, compilations from the UTK portal, Statistics Poland / Census, and intermediate calculations for 2021 and 2024.)*

---

## Wykorzystane narzędzia i pakiety / Tools and Packages Used
* **Język R (R Language)**: obsługa struktur danych i modelowanie / *data structure handling and modeling* (`dplyr`, `stringr`, `ggplot2` itp.)
* **Microsoft Excel**: wstępna agregacja danych, macierze i weryfikacja obliczeń / *initial data aggregation, matrices, and calculation verification*.
* **Źródła danych (Data Sources)**: Urząd Transportu Kolejowego (UTK), Główny Urząd Statystyczny / Spis Powszechny (Statistics Poland / Census).
* Reszta źródeł dostępna jest w podrozdziale 'bibliografia' w monografii.

---

## Metodologia w pigułce / Methodology in a Nutshell
* Badanie w pierwszej części opiera się na **analizie porównawczej z grupą kontrolną** (odcinek linii nr 68 jako linia referencyjna) w ujęciu lat 2021 i 2024.  
  *(The study is at first based on a **comparative analysis with a control group** (railway line no. 68 section as a reference line) for the years 2021 and 2024.)*
* Do oceny przystanków skonstruowano **syntetyczny miernik efektywności** z podziałem na stymulanty i destymulanty, przyjmując założenie o równej wadze kryteriów (zgodnie z metodologią wielowymiarowej analizy statystycznej).  
  *(To evaluate the stops, a **synthetic efficiency measure** was constructed with a division into stimulants and destimulants, assuming equal weights for criteria in accordance with multidimensional statistical analysis methodology.)*
* Weryfikacja statystyczna: Wykorzystano testy istotności oraz analizę rozkładu (m.in. test Shapiro-Wilka do badania normalności rozkładu, testy t-Studenta / odpowiedniki nieparametryczne do oceny istotności różnic między grupami).  
  *(Statistical verification: Significance tests and distribution analysis were applied, including the Shapiro-Wilk test for normality and Student's t-tests / non-parametric equivalents to assess the significance of differences between groups.)*
