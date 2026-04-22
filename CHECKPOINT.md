# Checkpoint

## Cel
Czy redukcja wymiarowości poprawia wyniki klasyfikacji dla danych wysokowymiarowych oraz które metody najlepiej zachowują strukturę klas?
Czy metody nieliniowe (t-SNE, UMAP) dają lepszą separację klas niż liniowe (PCA)?
Czy LDA jako metoda nadzorowana daje przewagę w zadaniach klasyfikacji?

## Metryki
- Accuracy oraz AUC dla klasyfikatorów opartych na danych w zredukowanym wymiarze.
- Silhouette score i trustworthiness - dla wizualizacji i oceny separacji klas w wysokowymiarowej oraz zredukowanej przestrzeni.

## Baseline
Klasyfikator bez redukcji wymiarowości (Logistic Regression / SVM)

## Plan testowania

Wykorzystane zostaną poniższe metody redukcji wymiarowości:

### Metody liniowe
- PCA 
- MDS 
### Metody nieliniowe
- t-SNE
- UMAP
- Kernel PCA
### Metoda nadzorowana
- LDA


W projekcie pokazane zostanie jak poszczególne metody redukcji wymiarowości wpływają na proces klasyfikacji.   
  
## Dane
Dane zostaną pobrane z bibliotek scikit-learn lub publicznych repozytoriów (np. MNIST).

W celach testowych zostaną wykorzystane poniższe zbiory danych:
- Pima Indians Diabetes
- South German Credit
- EMNIST
- Breast Cancer Wisconsin

## Podział pracy

Etap 1 – dane i preprocessing

Mikołaj:

Wybrane i pobrane zostaną datasety (np. z scikit-learn).
Przeprowadzona zostanie wstępna analiza danych (liczba cech, klasy, rozkłady).
Następnie stworzony zostanie klasyczny pipeline w ML:
- czyszczenie danych
- normalizacja / standaryzacja

Piotrek – walidacja poprawności danych
Kasia – przygotowanie podziału train/test

Etap 2 – redukcja wymiarowości

Piotrek:

Zaimplementowane zostaną wymienione w planie testowania metody:
- PCA, MDS
- t-SNE, UMAP
- LDA
Dobór liczby wymiarów (np. 2D do wizualizacji + kilka wariantów)

Mikołaj – integracja z pipeline’em danych
Kasia – generowanie wizualizacji (2D wykresy)


Etap 3 – klasyfikacja i ewaluacja

Kasia:

Implementacja klasyfikatorów oraz 
porównanie:
bez redukcji (baseline)
z redukcją
obliczenie accuracy

Mikołaj – przygotowanie danych wejściowych do modeli
Piotrek – analiza wyników i porównania między metodami

Na każdym etapie:

Wszyscy uczestniczą w decyzjach (np. wybór parametrów),
każdy robi code review fragmentów innych osób.
Ostatecznie, wspólnie przygotowany zostanie raport końcowy.
