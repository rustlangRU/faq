# FAQ

## Как установить Rust?

Официально рекомендуемый способ установки — [rustup.rs](https://rustup.rs).

## Какую версию использовать: stable, beta, nightly?

Для новичков лучше всего подойдет последняя `stable` версия.

## Что почитать по Rust?

Начинать лучше всего с [официальной книги](https://doc.rust-lang.org/book/index.html).

## Какой IDE пользоваться для Rust?

Есть 2 варианта: 

1) Любимый редактор + [RLS](https://github.com/rust-lang/rls):

   Преимущества: 
    - Не нужно учить другой редактор
    - Официальный проект от разработчиков языка
    - Использует парсер компилятора
    - Работает по Language Server Protocol, который поддерживается большинством современных редакторов


   Недостатки:
    - На данный момент не очень стабилен и не всегда правильно работает
    - Нетривиальная настройка в некоторых редакторах

2) [IntelliJ Rust](https://intellij-rust.github.io):

   Преимущества:
    - Собственный парсер специально заточенный для IDE
    - Использует инфраструктуру IntelliJ IDEA
    - Знаком пользователям IDEA, CLion, Rider и тд 
    - Разработчик плагина сидит в [чате](https://t.me/rustlang_ru), можно сообщать о проблемах
    
    
   Недостатки:
    - Потребление ресурсов
    - Неполная поддержка языка

## Как дебажить Rust?

Любой дебаггер для C/C++ работает с Rust. В CLion есть поддержка дебаггера в GUI.

## А кто-нибудь пользуется Rust в продакшене?

Да, вот [список пользователей](https://www.rust-lang.org/production/users).

## А вакансии по Rust есть?

Да, есть, хотя и не много. [Чат для обсуждения вакансий](https://t.me/rust_jobs)

## Не могу установить rustfmt, clippy на Rust 1.31

```
rustup self update
rustup toolchain uninstall stable
rustup toolchain install stable
```

## Как уменьшить размер бинаря?

- [How to minimize Rust binary size](https://github.com/johnthagen/min-sized-rust)
- [Why is a rust executable large](https://lifthrasiir.github.io/rustlog/why-is-a-rust-executable-large.html) и [перевод](https://habr.com/en/post/305246/), [тот же перевод только на хабре](https://rustycrate.ru/%D0%BE%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/2016/07/07/why-big-bin.html)
