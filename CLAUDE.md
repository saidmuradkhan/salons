# Salons

Gözəllik salonları və bərbərxanalar üçün AI qəbul köməkçisi. Bu repo **publicdir**.

## Biznes sənədləri

Plan, gecə işi qaydaları, rəqib analizi və hesabatlar `biznes/` qovluğundadır. O, ayrıca **private**
repodur və bu repoda gitignore-dadır. Qovluq varsa, işə başlamazdan əvvəl `biznes/CLAUDE.md`-ni oxu.

Oradakı məzmunu (qiymətlər, strategiya, rəqib analizi, mesaj şablonları) bu repoya köçürmə:
nə fayl kimi, nə kod şərhində, nə README-də, nə də commit mesajında.

## Gizli məlumatlar

- Açarlar, tokenlər və parollar yalnız `.env`-də olur. Kodda yalnız `.env.example`-da boş dəyərlə görünür.
- Salonların telefonu, adları və müştəri məlumatları yalnız `data/`-da olur. `.env` və `data/` commit olunmur.
- Commit-dən əvvəl `git diff --cached`-də açar, token və ya telefon nömrəsi olmadığını yoxla.
- Commit mesajlarında Claude və ya AI qeydi olmasın (`Co-Authored-By` və s. yoxdur).

## Kod üslubu

- TypeScript, strict rejim. Node.js 22.
- Testlər vitest ilə.
- İstifadəçiyə görünən mətnlər Azərbaycan və rus dilində.
