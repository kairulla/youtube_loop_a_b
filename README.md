[original source][1]

# Как зациклить кусок видео на Youtube <br> без установки расширений для браузера

1. откройте web console браузера
```
Ctrl-Shift-K (в Firefox)

Ctrl+Shift+J (в Chrome)
```
2. вставьте следующий код в консоль:
```
var
a;
b;
v = $(".video-stream");
v.addEventListener('timeupdate', function() {
    if (Math.round(v.currentTime) == b) {
        v.currentTime = a;
        }});
```
3. нажмите Enter и вставьте ещё вот это вместе с кавычками:
```
"allow pasting"
```
4. потом нужно задать значения в секундах <br>
    *начальная позиция:
```
a=10
```

    *конечная позиция:
```
b=30
```
5. Нажать Enter


чтобы все отменить - просто перегрузите страницу

зы: чтобы зациклить целиком, нажмите правую кнопулю на видео (вдруг кто не в курсе)

всем удачи


<!-- Мои ссылки -->
[1]: https://pikabu.ru/story/kak_zatsiklit_kusok_video_na_youtube_5736593
