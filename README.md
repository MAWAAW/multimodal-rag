# Multi-modal RAG Chatbot
Bienvenue dans le Multi-modal RAG Chatbot, une application interactive développée avec Streamlit qui combine les capacités de traitement du langage naturel de OpenAI GPT-4o avec une base de données vectorielle ChromaDB pour fournir des réponses enrichies par des images. Ce chatbot permet aux utilisateurs de poser des questions en contexte d'images, offrant ainsi une expérience utilisateur fluide et informative.

## Fonctionnalités
- Interface Utilisateur Intuitive : Développée avec Streamlit pour une expérience utilisateur rapide et réactive.
- Recherche d'Images Intelligente : Utilise ChromaDB pour indexer et rechercher des images pertinentes basées sur les requêtes des utilisateurs.
- Intégration de GPT-4o : Fournit des réponses contextuelles et précises en utilisant le modèle de langage GPT-4o d'OpenAI.
- Support Multi-modal : Capacité à traiter et intégrer des données textuelles et visuelles pour des réponses enrichies.
- Gestion des Transactions : Assure l'intégrité et la cohérence des données lors des opérations de lecture et d'écriture.

## Utilisation
### Récupérer le projet
```bash
git clone https://github.com/MAWAAW/multimodal-rag.git
cd multimodal-rag
```
### Créer et activer un environnement virtuel
```bash
python -m venv env
```
- Sur Windows :
```bash
env\Scripts\activate
```
- Sur macOS/Linux :
```bash
source env/bin/activate
```

### Installer les dépendances
```bash
pip install -r requirements.txt
```

### Configurer la clé API OpenAI
Remplacer dans le script la ligne la ligne `OPEN_API_KEY = " . . . "` par votre clé API `OPEN_API_KEY = "sk-..."`

### Initialiser la base de données ChromaDB
Le script charge les données dans la base de données ChromaDB lors de l'exécution. Assurez-vous d'avoir un dossier d'images au format jpg/jpeg `data` à la racine du projet prêt à être indexé

### Lancer l'application Streamlit
```bash
streamlit run multimodal-rag.py
```

### Interagir avec le Chatbot
Entrez votre question dans la zone de texte.
Les images pertinentes seront affichées.
Recevez une réponse contextualisée basée sur les images fournies.

## Remerciements
- Merci à l'équipe de Streamlit pour l'interface utilisateur simplifiée.
- Merci à ChromaDB pour la gestion efficace des données vectorielles.
- Merci à LangChain pour les outils puissants de traitement du langage naturel.

## Licence
Ce projet est distribué sous la licence MIT
