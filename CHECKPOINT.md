# Checkpoint

## Cel
Czy redukcja wymiarowości poprawia wyniki klasyfikacji dla danych wysokowymiarowych oraz które metody najlepiej zachowują strukturę klas?
Czy metody nieliniowe (t-SNE, UMAP) dają lepszą separację klas niż liniowe (PCA)?
Czy LDA jako metoda nadzorowana daje przewagę w zadaniach klasyfikacji?

## Metryki
accuracy - dla danych; 
silhouette score i trustworthiness - dla wizualizacji.

## Baseline
klasyfikator bez redukcji wymiarowości (Logistic Regression / SVM)

## Plan testowania
### Metody liniowe
PCA + klasyfikator
MDS + klasyfikator

### Metody nieliniowe
t-SNE + klasyfikator 
UMAP + klasyfikator
### Metoda nadzorowana
LDA + klasyfikator

## Dane
Dane zostaną pobrane z bibliotek scikit-learn lub publicznych repozytoriów (np. MNIST).
