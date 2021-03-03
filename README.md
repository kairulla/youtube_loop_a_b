[original source][1]

# Как зациклить кусок видео на Youtube <br> без установки расширений для браузера

1. откройте web console браузера (Ctrl-Shift-J в Chrome, Ctrl-Shift-K в Firefox)
2. вставьте следующее: var v = $(".video-stream"); v.addEventListener('timeupdate', function() { if (Math.round(v.currentTime) == 100) v.currentTime = 15; });
первая цифра (в примере 100) - конец отрезка в секундах, вторая (15) - начало (куда прыгнуть)
3. наслаждайтесь :)
чтобы все отменить - просто перегрузите страницу

зы: чтобы зациклить целиком, нажмите правую кнопулю на видео (вдруг кто не в курсе)

всем удачи


<!-- Мои ссылки -->
[1]: https://pikabu.ru/story/kak_zatsiklit_kusok_video_na_youtube_5736593
