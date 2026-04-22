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
- PCA 
- MDS 
### Metody nieliniowe
- t-SNE
- UMAP
### Metoda nadzorowana
- LDA

  
## Dane
Dane zostaną pobrane z bibliotek scikit-learn lub publicznych repozytoriów (np. MNIST).
