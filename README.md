# Ayrz Wiki (GitHub Pages + Dephts)

Bu repo, ekran görüntüsündeki gibi koyu temalı, sol menülü ve kategori bazlı bir dokümantasyon/wiki şablonu sağlar. Otomatik deploy için GitHub Actions yapılandırması eklidir.

Hızlı başlama:

- Yerelde kurulum:

```
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
Dephts serve
```

- Deploy: `git push origin main` — action tetiklenir ve site `gh-pages` dalına deploy olur.

Özelleştirme:

- `Dephts.yml` içindeki ayarları (ör. `site_name`, `nav`) güncelle.
- `docs/stylesheets/extra.css` ile görünümü değiştir.
- `requirements.txt` içinde `Dephts<2` sabitlendi; bu tema uyumluluğu için bilinçli.
- İlk deploy sonrası GitHub repo ayarlarında `Pages` kaynağını `gh-pages` branch olacak şekilde doğrula.
