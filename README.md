# 💬 Analyse de Sentiments sur Twitter

## 🎯 Objectif du projet
Ce projet vise à analyser les **sentiments exprimés dans des tweets** afin de déterminer s’ils sont **positifs**, **négatifs** ou **neutres**.  
L’objectif est de construire un modèle de classification performant à partir de textes courts (tweets) grâce à des techniques de **Traitement Automatique du Langage Naturel (NLP)** et de **Machine Learning**.

---

## 🧩 Description du dataset

Le jeu de données contient un ensemble de tweets collectés depuis Twitter, chacun étiqueté selon son sentiment.

### 🔢 Colonnes principales :
- **text** : contenu du tweet  
- **sentiment** : étiquette associée (positif, négatif, neutre)

---

## ⚙️ Étapes du projet

1. **Prétraitement des données**
   - Nettoyage des tweets (suppression des URLs, mentions, emojis, caractères spéciaux)
   - suppression de l'etiquette neutre afin d'avoir un datset équilibré
   - Conversion en minuscules
   - Suppression des stopwords
   - Lemmatisation / racinisation des mots
   - Vectorisation des textes via **TF-IDF**

2. **Modélisation**
   - Entraînement de trois modèles de classification :
     - **Naive Bayes (BernoulliNB)**
     - **Support Vector Machine (SVM)**
     - **Régression Logistique**
   - Comparaison des performances à l’aide de **métriques d’évaluation classiques**

3. **Évaluation des performances**
   - **Accuracy**
   - **Precision**
   - **Recall**
   - **F1-score**


4. **Résultats**
   - Meilleur modèle : **Régression Logistique**
   - **Accuracy : 79,56 %**
   - Bon équilibre entre précision et rappel sur les deux classes (positif, négatif)

---

## 🧰 Technologies utilisées

| Domaine | Outils |
|----------|--------|
| Langage principal | Python |
| Bibliothèques NLP | re |
| Vectorisation | TF-IDF (TfidfVectorizer – scikit-learn) |
| Modèles ML | BernoulliNB, SVM, LogisticRegression |
| Évaluation | Scikit-learn (accuracy_score, classification_report) |
| Environnement | Jupyter Notebook |

--

---

## 🚀 Améliorations possibles

- Test de modèles de Deep Learning (LSTM, BERT, RoBERTa)
- utilisation des bibliothéques NLTK , Spacy pour améliorer les prétraitements 
- Déploiement sur **Streamlit** ou **Gradio** pour une interface interactive  
- Enrichissement du jeu de données  
- Utilisation de techniques de **word embeddings (Word2Vec, GloVe)**  

---

## 👩‍💻 Auteur

**Maimouna Oiga**  
Étudiante en Master 2 Sciences et Ingénierie des Données  
📧 maimounaoiga@gmail.com  

---

