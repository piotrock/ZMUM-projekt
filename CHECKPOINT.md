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

