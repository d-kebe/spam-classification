# 📱 Classification de Spams SMS par Machine Learning

> Modèle de détection automatique de contenus malveillants dans des SMS, entraîné sur 5 500 messages réels.

---

## 🎯 Objectif

Construire un classifieur capable de distinguer automatiquement un **spam** d'un message légitime (**ham**), en s'appuyant sur des techniques de traitement du langage naturel (NLP) et d'apprentissage automatique.

---

## 📊 Résultats

| Métrique | Score |
|---|---|
| Accuracy | ~97% |
| Précision (spam) | ~99% |
| Recall (spam) | ~92% |
| F1-score (spam) | ~95% |

---

## 🛠️ Stack technique

- **Langage :** Python 3
- **Bibliothèques :** scikit-learn, pandas, numpy, matplotlib, seaborn
- **Algorithme :** Naive Bayes Multinomial
- **Vectorisation :** TF-IDF (5 000 features)

---

## 📁 Structure du projet

```
.
├── spam_classification.ipynb   # Notebook principal
├── SMSSpamCollection           # Dataset (téléchargé automatiquement)
├── distribution.png            # Graphique de distribution des classes
├── confusion_matrix.png        # Matrice de confusion
├── top_words.png               # Mots les plus discriminants
└── README.md
```

---

## 🚀 Lancer le projet

```bash
# 1. Cloner le dépôt
git clone https://github.com/d-kebe/spam-classification
cd spam-classification

# 2. Installer les dépendances
pip install scikit-learn pandas numpy matplotlib seaborn jupyter

# 3. Lancer le notebook
jupyter notebook spam_classification.ipynb
```

> Le dataset est téléchargé automatiquement à la première exécution.

---

## 🔍 Aperçu du pipeline

```
SMS brut
   │
   ▼
Nettoyage du texte (minuscules, ponctuation)
   │
   ▼
Vectorisation TF-IDF
   │
   ▼
Modèle Naive Bayes
   │
   ▼
ham ✅ ou spam 🚨
```

---

## 💡 Pistes d'amélioration

- Tester d'autres algorithmes : SVM, Random Forest, Logistic Regression
- Appliquer une lemmatisation pour normaliser les mots
- Déployer le modèle via une API Flask
- Gérer le déséquilibre des classes avec SMOTE

---

*Projet réalisé dans le cadre d'une démarche d'autoformation en Machine Learning — Djiby KEBE, 2026*
