# Image Recommendation System 📸

A user-preference image recommendation system implemented in Python.  
Combines image metadata, feature extraction, clustering and simple ML pipelines to recommend images based on user preferences and content similarity.

## Features 🔍
- Read and parse image files and EXIF metadata.
- Image feature extraction and preprocessing (OpenCV, PIL).
- Semantic enrichment via SPARQL queries.
- Dominant colors extration and analysis
- Clustering (KMeans) and cluster evaluation (silhouette score).
- User preference encoding and recommendation pipeline (scikit-learn).
- Interactive exploration using `ipywidgets` (not available on GitHub).

## How it Works 🧩
1. Ingestion: read images and EXIF metadata using Pillow and ExifTags.
2. Cleaning & normalization: normalize text (unicodedata / unidecode), clean paths/URLs.
3. Feature extraction: use OpenCV + simple descriptors or metadata-derived features.
4. Dimensionality & scaling: StandardScaler / custom encodings for numerical features.
5. Clustering & evaluation: KMeans to find image groups, silhouette score for quality.
6. User preferences: encode preferences (one-hot / MultiLabelBinarizer / OneHotEncoder) and combine with content features.
7. Recommendation: simple supervised or similarity-based ranking (SVM and nearest-cluster matching).
8. Interactive UI: use ipywidgets (GridspecLayout, Image, interact) to display results and let users tweak preferences.

## Contributing 🤝
Feel free to fork this repo, improve the code, or experiment with other activation functions and learning rates!

## License 📄
This project is under MIT license.
