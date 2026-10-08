# Turbo Retro

Retroville'de geçen 3D uçan araba yarışı (Android).

APK, her `main` dalına push'ta GitHub Actions ile otomatik derlenir.
Hazır APK: **Releases** bölümündeki en son `TurboRetro.apk`.

Oyunun kendisi: `app/src/main/assets/index.html`

## Kendi müziğini eklemek
`app/src/main/assets/` klasörüne **music.mp3** adıyla bir dosya koy. Oyun varsa onu çalar, yoksa kendi müziğini kullanır.

## Google Play (AAB)
Her derlemede **Releases** bölümüne `TurboRetro.aab` da eklenir. Play Console'a bu dosyayı yükle.
AAB'nin Play'in kabul ettiği anahtarla imzalanması için deponun Settings > Secrets and variables > Actions
bölümüne `KEYSTORE_BASE64` ve `KEYSTORE_PASSWORD` secret'larını ekle (değerler GITHUB-SECRETS.txt dosyasında).
Anahtar dosyasını (.jks) asla depoya yükleme.
