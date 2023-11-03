# fifa22

Downloading anaconda:
`https://www.anaconda.com/download`

Updating requirements:
`pip list --format=freeze > requirements.txt`

Pytania na konsulatacje:
  1. Czy nalezy sporządzić wpierw wpływ cech ogólny dla wszystkich zawodników a potem oddzielne zalezne od pozycji i jeszcze jeden dla top 10% zawodników?
  2. Czy trzy rózne modele oznaczają 3 różne modele odrzucania współczynników czy 3 różne współczynniki(PCA,FA itd)?
  3. Czy dodać preferowaną stopę jako wartość binarną(prawa-0, lewa-1)?
  4. Co zrobić z wartoścniam NAN w tabelach?
  5. Czy zawodnik powinien miec kilka mozliwych pozycji(np: pomocnik i napastnik)


Podział pracy:

Karol:
  - standaryzacja, normalizacja
  - PCA (wizaulizacja pca)

Paweł:
  - tabela (usunięcie/modyfikacja NAN, )

Piotr:
  - podział na pozycje(jedna kolumna)
  - FA
