# ortho_lines_model_ortho_lines.pth

מודל שהורד אוטומטי דרך GitHub Actions

## מידע
- **גודל כולל**: 715MiB
- **מספר חלקים**: 8
- **גודל כל חלק**: ~95MB
- **URL מקורי**: https://huggingface.co/yzamir/ortho-lines/resolve/main/ortho_lines.pth
- **תאריך הורדה**: Thu Nov 20 12:16:27 UTC 2025

## איך להשתמש

1. הורד את כל הקבצים בתיקייה זו
2. הרץ את סקריפט האיחוד:
   ```bash
   python merge.py
   ```
3. הקובץ `model_final.pth` יתקבל

## הורדה מהירה

```bash
# הורדה עם git
git clone --depth 1 --filter=blob:none --sparse \
  https://github.com/sumca1/model-mirror.git
cd model-mirror
git sparse-checkout set ortho_lines_model_ortho_lines.pth

# איחוד
cd ortho_lines_model_ortho_lines.pth
python merge.py
```

## או עם wget

```bash
# הורדת כל החלקים
BASE_URL="https://raw.githubusercontent.com/sumca1/model-mirror/main/ortho_lines_model_ortho_lines.pth"

wget $BASE_URL/config.yml
wget $BASE_URL/merge.py

# הורדת החלקים (התאם את המספר)
for i in {00..07}; do
  wget "$BASE_URL/model_final.pth.${i}.part"
done

# איחוד
python merge.py
```
