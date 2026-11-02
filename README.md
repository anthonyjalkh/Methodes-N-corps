# Principe de la résolution
## Conditions initiales 
Utilisation de la bibliothèque 'GALPY'

## Conditions aux limites 
- Étape 1 : conditions périodiques
- Étape 2 : condition isolées

## Méthode Particules-Mailles
- Calcul de la densité en utilisant la position des particules
> - NGP (*tests*)
> - CIC : cube homogène d'extension une cellule
> - TSC : pyramide d'extension deux cellules
- Calcul du potentiel via la résolution de l'équation de Poisson
- Calcul du gradient du potentiel pour obtenir le champ gravitationnel
- Calcul de l'interpolation du champ gravitationnel au niveau des particules 
> - Utilisation d'une méthode inverse par rapport à celle employée pour le calcul de la densité
- Intégration des équations du mouvement
> - Euler semi-explicite (*tests*)
> - Leapfrog
> - Kick-Drift-Kick (*possibilité d'utiliser un pas de temps variable*)
