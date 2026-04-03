
# DECISIONS DE NETTOYAGE

## 1. Doublons
- Suppression basée sur transaction_id
- Conservation de la première occurrence

## 2. Types
- date_transaction convertie en datetime
- montant et solde_avant convertis en float

## 3. Valeurs manquantes
- Numériques : imputation par médiane
- Catégorielles : imputation par mode

## 4. Valeurs aberrantes
- Détection via IQR
- Conservation avec flag is_anomaly
- Pas de suppression pour éviter perte d'information

## 5. Normalisation
- devise → uppercase
- segment_client → format uniforme
- nettoyage des espaces

## 6. Feature engineering
- Variables temporelles
- Score de risque client
- Agrégations par client
- Taux de rejet par agence
