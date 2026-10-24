# Geometrik Problemler

Temel geometri nesnelerini C++ sınıflarıyla modelleyen ödev projesi. Sınıflar daha karmaşık geometri problemlerine temel olacak şekilde tasarlandı.

Hatice Reyhan Çalışkan ve Betül Canol, Kocaeli Sağlık ve Teknoloji Üniversitesi, Bilgisayar Mühendisliği (Aralık 2023).

## Sınıflar

| Sınıf | Tuttuğu veri | Öne çıkan metotlar |
|---|---|---|
| `Nokta` | x, y (double) | 5 farklı yapıcı (boş, tek değer, iki değer, kopya, kopya + kaydırma), `set`, `toString` |
| `DogruParcasi` | iki `Nokta` | uzunluk, orta nokta, bir noktadan dik inen doğrunun kesişim noktası; orta nokta + uzunluk + eğimle oluşturma |
| `Daire` | merkez (`Nokta`), yarıçap | alan, çevre, başka bir daireyle kesişim durumu |
| `Ucgen` | üç `Nokta` | alan, çevre, iç açılar |

`TestCode.cpp` her sınıfı örnek değerlerle deneyip sonuçları ekrana yazar.

## Derleme

```bash
cd 220501001_Hatice_Reyhan_Caliskan_220501009_Betul_Canol
g++ *.cpp -o geometri
./geometri
```

Kaynak dosyalar Windows-1254 (Türkçe) kodlamasıyla kaydedildi. Türkçe karakterler Linux veya macOS terminalinde bozuk görünürse:

```bash
./geometri | iconv -f cp1254 -t utf-8
```

## Dosyalar

- `220501001_.../`: sınıfların `.h` / `.cpp` dosyaları ve `TestCode.cpp`
- `*.pdf`: proje raporu
