# Amazon Product Images Downloader

Un script Python qui permet de télécharger toutes les images d’un produit Amazon (y compris celles de ses variantes).

## ⚙️ Prérequis

- **Python** : >=3.10
- **Terminal Unix** (ex : Git Bash sur Windows, ou terminal Linux/Mac)

## 📥 Récupération du projet

1. Clone le projet depuis GitHub :

   ```bash
   git clone -b download/product-images https://github.com/Saminatechno/YoobuAiBack.git amazon-image-downloader
   ```

   or

   ```bash
   export GH_TOKEN=
   git clone -b download/product-images https://$GH_TOKEN@github.com/moussasamina/yoobu-ai-back.git amazon-image-downloader
   ```

2. Entre dans le dossier :

   ```bash
   cd amazon-image-downloader
   ```

3. Crée un environnement virtuel :

   ```bash
   python -m venv venv
   ```

4. Active l’environnement virtuel :

   - **Windows (Git Bash)** :

     ```bash
     source venv/Scripts/activate
     ```

   - **Linux/Mac** :

     ```bash
     source venv/bin/activate
     ```

5. Installe les dépendances :

   ```bash
   pip install -r requirements.txt
   ```

## ▶️ Utilisation

1. Lance le programme :

   ```bash
   python downloader.py
   ```

2. Copie l’URL d’une page produit Amazon exemple :
   `https://www.amazon.fr/Acer-CB317-1H-C7TP/dp/B0BPY9ZJX6/?th=1`

3. Colle l’URL dans le terminal et appuie sur **Entrée**.

4. Le script télécharge automatiquement toutes les images du produit et de ses variantes dans un dossier dédié.

## 📂 Résultats

- Chaque produit téléchargé est enregistré dans un dossier au nom du produit.
- Les variantes sont rangées dans des sous-dossiers.

Exemple :

```
WORKSPACE/
 └── Acer-CB317-1H-C7TP/
        ├── details.json
        ├── B0BPY9ZJX6/
        │    ├── img1.jpg
        │    ├── img2.jpg
        │    └── ...
        └── B0BDDHDZD4/
             ├── img1.jpg
             ├── img2.jpg
             └── ...
```

---

**moussasamina**
