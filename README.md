# fifa22

Downloading anaconda:
`https://www.anaconda.com/download`

Updating requirements:
`pip list --format=freeze > requirements.txt`

Pytania na konsulatacje:
  1. [x] Czy nalezy sporządzić wpierw wpływ cech ogólny dla wszystkich zawodników a potem oddzielne zalezne od pozycji i jeszcze jeden dla top 10% zawodników? jak chcemy
  2. [ ] Czy trzy rózne modele oznaczają 3 różne modele odrzucania współczynników czy 3 różne współczynniki(PCA,FA itd)? zależne tylko od PCA - regresja LASSO, klasyfikacja, las losowy
  3. [ ] Czy dodać preferowaną stopę jako wartość binarną(prawa-0, lewa-1)? wywalić kolumnę
  4. [x] Co zrobić z wartoścniam NAN w tabelach? usunąć kolumny z wieloma wartościami NAN
  5. [ ] Czy zawodnik powinien miec kilka mozliwych pozycji(np: pomocnik i napastnik) - realizacja remisów w pozycjach
  6. [ ] usunąć kolumny, które znacząco wpływają na ocenę klasyfikatora: score, wage_eur, release_clause_eur, international_reputation


Podział pracy:

Karol:
  - [x] standaryzacja, normalizacja
  - [x] PCA (wizaulizacja pca)
  - [ ] wywalić kolumnę prawa-lewa
  - [ ] usunąć kolumny, które znacząco wpływają na ocenę klasyfikatora: score, wage_eur, release_clause_eur, international_reputation
  - [ ] sprawdzenie wersji mastera, scalanie, usunięcie ewentualnych konfliktów
  

Paweł:
  - [x] tabela (usunięcie/modyfikacja NAN)
  - [x] klasyfikacja
  

Piotr:
  - [x] podział na pozycje(jedna kolumna)
  - [x] FA
  - [ ] regresja LASSO
  - [ ] realizacja remisów w pozycjach
