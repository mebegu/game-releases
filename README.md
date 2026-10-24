# game-releases

Oyunların indirilebilir build'lerini **Release** olarak barındırır. Android APK ve
masaüstü paketleri burada yayımlanır.

**Repo ağacı bilerek boştur.** Dosyalar release asset'i olarak durur; böylece repo
boyutuna sayılmazlar ve Pages bütçesinden yemezler. Kaynak kod her oyunun kendi
(private) reposundadır.

Tasarım: [GAMES-PIPELINE.md](https://github.com/mebegu/mebegu.github.io/blob/main/docs/GAMES-PIPELINE.md)

## Tag biçimi

Tek repoda birden fazla oyun olduğu için tag oyun slug'ıyla başlar:

```
bagatelle-v0.3.0
caves-v0.1.2
distinct-v0.2.0
lift-v0.4.0
football-academy-v0.1.0
```

`releases/latest` bu repoda anlamlı değildir — hangi oyun olduğunu bilemez. İndirme
bağlantıları her sürümde tam adresle verilir:

```
https://github.com/mebegu/game-releases/releases/download/bagatelle-v0.3.0/bagatelle-0.3.0.apk
```

## Dosya adlandırma

```
<slug>-<sürüm>.apk          Android
<slug>-<sürüm>-win64.zip    Windows
```
