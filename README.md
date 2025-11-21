# OrdoVerif – Vérification d’ordonnances (Python + Flask)

Application web légère qui :
- scanne une ordonnance (image ou PDF) ;
- extrait le numéro RPPS du médecin ;
- vérifie sa validité via la base publique ARS ;
- détecte la présence d’un cachet / date ;
- retourne **VRAI** ou **FAUX** avec un rapport détaillé.

&gt; ⚠️ Usage pédagogique – agrément CNIL / ANSM nécessaire pour la production.

---

## Installation locale

### Prérequis
- Python 3.9+
- Tesseract OCR + langue française
- poppler-utils (pour pdf2image)

Ubuntu / Debian
```bash
sudo apt update
sudo apt install tesseract-ocr tesseract-ocr-fra poppler-utils
