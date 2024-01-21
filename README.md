# fifa22

Downloading anaconda:
`https://www.anaconda.com/download`

Updating requirements:
`pip list --format=freeze > requirements.txt`

Pytania na konsulatacje:
  1. [x] Czy nalezy sporządzić wpierw wpływ cech ogólny dla wszystkich zawodników a potem oddzielne zalezne od pozycji i jeszcze jeden dla top 10% zawodników? jak chcemy
  2. [ ] Czy trzy rózne modele oznaczają 3 różne modele odrzucania współczynników czy 3 różne współczynniki(PCA,FA itd)? zależne tylko od PCA - regresja LASSO, klasyfikacja, las losowy
  3. [X] Czy dodać preferowaną stopę jako wartość binarną(prawa-0, lewa-1)? wywalić kolumnę
  4. [x] Co zrobić z wartoścniam NAN w tabelach? usunąć kolumny z wieloma wartościami NAN
  5. [ ] Czy zawodnik powinien miec kilka mozliwych pozycji(np: pomocnik i napastnik) - realizacja remisów w pozycjach
  6. [X] usunąć kolumny, które znacząco wpływają na ocenę klasyfikatora: score, wage_eur, release_clause_eur, international_reputation
  7. co wpływa, że 1/3 nie kwalifikuje się jako top10?
  8. zbiorowy f1 score dla top10 (lasy losowe)
  9. we wnioskach uwzględnić wyniki (regresja lasy losowe)
  10. co dokładnie oznaczają y dla regresji liniowej?
  11. dobrze skomentować wyniki w raporcie
  11. shap values (lasy losowe regresja), wylicza kontrybucję, wyjaśnialność, zobaczyć co jest na wykresach
  12. porównać wszystkie modele pomiędzy sobą


Podział pracy:

Karol:
  - [x] standaryzacja, normalizacja
  - [x] PCA (wizaulizacja pca)
  - [X] wywalić kolumnę prawa-lewa
  - [X] usunąć kolumny, które znacząco wpływają na ocenę klasyfikatora: score, wage_eur, release_clause_eur, international_reputation
  - [X] sprawdzenie wersji mastera, scalanie, usunięcie ewentualnych konfliktów
  - [ ] histogram  value_eur 

Paweł:
  - [x] tabela (usunięcie/modyfikacja NAN)
  - [x] klasyfikacja (ze względu na pozycje)
  - [x] klasyfikacja (top 10% , widełki value_eur)
  

Piotr:
  - [x] podział na pozycje(jedna kolumna)
  - [x] FA
  - [ ] regresja (liniowa oraz elastic)
  - [ ] realizacja remisów w pozycjach / dodanie kategori mid-back, mid-forward

- dodawanie lasów losowych (dla klasyfikacji, regresji)
- rigid regression (porównanie z innymi)
- uporządkowanie dataframów
- sprawdzenie klasyfikacji oraz regresji dla nienaruszonych danych

