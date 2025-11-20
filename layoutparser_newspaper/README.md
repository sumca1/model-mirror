# layoutparser_newspaper

מודל שהורד אוטומטי דרך GitHub Actions

## מידע
- **גודל כולל**: 315MiB
- **מספר חלקים**: 4
- **גודל כל חלק**: ~95MB
- **URL מקורי**: https://www.dropbox.com/s/8v4uqmz1at9v72a/model_final.pth?dl=1
- **תאריך הורדה**: Thu Nov 20 14:24:53 UTC 2025

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
git sparse-checkout set layoutparser_newspaper

# איחוד
cd layoutparser_newspaper
python merge.py
```

## או עם wget

```bash
# הורדת כל החלקים
BASE_URL="https://raw.githubusercontent.com/sumca1/model-mirror/main/layoutparser_newspaper"

wget $BASE_URL/config.yml
wget $BASE_URL/merge.py

# הורדת החלקים (התאם את המספר)
for i in {00..03}; do
  wget "$BASE_URL/model_final.pth.${i}.part"
done

# איחוד
python merge.py
```
