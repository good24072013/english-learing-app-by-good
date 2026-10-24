# English Learning App (Android)

Bu, **English Learning Portal** saytının Android tətbiqidir. Tətbiq tam ekranda açılır (ünvan zolağı olmur) və canlı saytı göstərir. Saytda edilən hər yenilik tətbiqdə avtomatik görünür.

## Yükləmək (şagirdlər üçün)

Telefondan bu linkə toxun:

**https://github.com/good24072013/english-learing-app-by-good/releases/tag/v1.0.6**

(`GITHUB_ADIN` və `REPO_ADI` yerinə öz GitHub adını və repo adını yaz.)

1. Fayl yüklənəndən sonra onu aç.
2. Telefon "Bu mənbədən quraşdırmağa icazə ver" soruşsa, icazə ver (Allow).
3. "Quraşdır" (Install) düyməsinə bas.
4. Ana ekranda **English Learning App** ikonu çıxacaq.

Android "zərərli ola bilər" xəbərdarlığı göstərə bilər. Bu, tətbiq Google Play-dən olmadığı üçün çıxır.

Tətbiqi ilk dəfə açanda mikrofon icazəsi soruşula bilər. Danışıq (Speaking) tapşırığı üçün "İcazə ver" seç.

## Quraşdırma (müəllim üçün, bir dəfə)

1. GitHub-da bu faylların hamısı ilə yeni repo yarat (public ola bilər, içində gizli məlumat yoxdur).
2. **Settings → Secrets and variables → Actions** bölməsində iki secret əlavə et: `KEYSTORE_PASSWORD` və `KEYSTORE_BASE64` (dəyərləri `github-secrets-GIZLI.txt` faylında).
3. **Actions → Build Android APK → Run workflow** düyməsinə bas. Təxminən 5-10 dəqiqəyə `.apk` hazır olur və **Releases** bölməsində görünür.

Secret-ləri əlavə etməsən də tətbiq qurulur, amma sonrakı yeniliyi köhnə quraşdırmanın üstünə yükləmək olmur.

## Sayt ünvanı dəyişərsə

`capacitor.config.json` faylında `server.url` sətrini dəyiş və dəyişikliyi GitHub-a yüklə, yeni APK özü qurulacaq.

## Yeni versiya buraxmaq

Tətbiqin görünüşü saytdan gəlir, ona görə sayt yeniliyi üçün yeni APK lazım deyil. APK-nı yalnız ikon, ad və ya ünvan dəyişəndə yenidən qurmaq lazımdır (**Actions → Run workflow**).
