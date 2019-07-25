# Инструкция по таймингу для самых маленьких

Цель статьи – быстро научить вас правильно таймить. Нет, тайминг у HorribleSubs не правильный. Нет, его нельзя оставлять как есть. Он неприятен глазу даже если вы очень поднатужтесь, чтобы это не замечать. А теперь как делать правильно.
Нам нужно:
-   SCXvid.exe;
-   Generate_Keyframes.bat;
-   ffmpeg.exe;
-   aegisub;
-   прямые руки.

### Подготовка к таймингу
[Скачайте](https://drive.google.com/open?id=169OWVisabga_BajkviAL_pUc7F-m1lr0) SCXvid.exe и ffmpeg.exe и положите их в C:/Windows. Нет, компьютер не взорвется. Затем, Generate_Keyframes.bat положите в папку с видео, которое хотите таймить. Перетяните видео на .bat файл. Появится чёрное окошко:![](https://lh5.googleusercontent.com/oLTpITRse6NYlCYwc968sLLWWSibdwQjsKi5-VGDkjmuAgBkxSst4rK1H-Y7ROXG-Y9CI2KusxqMuGIg9xtlHBqKfvgdOgjc5RwRpiaUGMiSNYHB9H5K25nFxi5-dyg8OR9orVYr)Нет, ваш компьютер не взорвется. Когда файл доработает, вы увидите вот это:
![](https://lh6.googleusercontent.com/U7Gf5JG8WWOnnQwIEKmrQC1ar4rYylY40-LkH2nUQzz30IcD9gsM0dx3xtYGH_xYGU2KeBwPVsAAbiUpsQVj_0HzYlrXpcvQoUpK2ggz-ZA4WkdAli_4gEOM7te7qMgNwP6G_iyQ)
В папке с видео появился файл \*имявидео\*_fixed.mkv_keyframes.txt.
![](https://lh5.googleusercontent.com/2FlJVEhOHOtgWsbbtHgrcJ-qDaFu5I0mLZ2y7muBRZe-Neu6OK02WdfwRqrBBpl0m4XLBXa3lKZbG72Ug5FxFg4oGyzGTfUO99jgC3bWdIhXrP1G-3wkBWPqfT5Cwt3RA2ZMfmrj)
Замечательно. Открываем аэгисаб, грузим субтитры и видео. Затем жмём Видео - открыть файл ключ-кадров. Выбираем файл, который мы только что получили.
  
Если вы сделали все правильно, розовые полоски на аудиодорожке сменили свое расположение. Теперь они [чаще всего] указывают на место, где происходит смена кадра.
![](https://lh6.googleusercontent.com/KRx0aD06f2OJ1lpeNxyDccmkjI4vXTx5IPcJttiVEYHBA9YcHWyYEuNH_GOvnwnbT88AhMl56iHtLiAljcAJLA2Z1zokoFr0lPRTLJDtjx4BxmlXKeq_TpXXQzjVGAgluixU-mty)Переключите режим отображения аудиодорожки на спектрограмму. Потягав ползунки сбоку, вы сможете отстроить её так, чтобы видно было только речь персонажей без посторонних шумов. Включается она кнопкой под аудиодорожкой:![](https://lh4.googleusercontent.com/Qo-5LtUIstzNYkRgqabuAJfVG-hBUa4_uUU26aXrL0yRRTVGEie_xAGFkUYxTtTmQ8Q_SyxIIKOVg3zB8nUiQ2L0FqLTK6NMDMJ66WZIifrgNxtU8G83-pBqO_2v43xa-2m3WQYV)
## Тайминг
Остаётся лишь затаймить. Дело техники. Работайте с аудиодорожкой. Рекомендации:
-   Строка субтитра должна начинаться примерно за 80 мс до того, как начинает говорить сам персонаж.
-   Строка субтитра должна заканчиваться через 300-600 мс после того, как персонаж закончит говорить.

Как это выглядит на спектрограмме:
![](https://lh5.googleusercontent.com/59K30JvNrD4DZoP30C8PQzySl4cWu__qb9yitPLxQuYob-RVrCed_Y8ZRyygLyHfd4wltcFrChwUC_5gJCwnD1S2vUsj3sbfF-lEQKq_LFvrnvv7UKVFQjo-DNgj5KZ0139hl6nE)
Теперь о крайних случаях. Мы не зря подготовили наши розовые полоски. Дело в том, что если очень быстро после смены кадра начинается/заканчивается строка - это плохо. Перед сменой кадра - тоже плохо. Нужно подтягивать к началу кадра. Рекомендации:

-   Если персонаж заканчивает говорить меньше, чем за 400 миллисекунд до смены кадра - смело тянем конец строки к ключ-кадру.![](https://lh6.googleusercontent.com/2amqKrt6V3_fQfSQ5rnsvAXrPu3DOPjHuWwReXjVeQPcSNMILag7yEs8EZmjQAMdr3bddoNDD7AmpVJKE33FoefmjmEbszcquZudOHTfORaA_bfhYkdMpOpVy5VjmLJYQ_kz5YmB)
-   Если персонаж начинает говорить в промежутке до 300мс с начала кадра, тянуть строку к началу кадра.   ![](https://lh6.googleusercontent.com/P4_4GJlWAywM468Y-0lwElontYNuUJ-h0ojaeZYSXu2LNnkT75ieYBsrDXnL6hP_jVm5L7vZS113swh2TZSHpt9abYytOUsvD3u73AjIqN2Gg1KMH2oO7WQp5fmXtqMz3OrizGqU)
-   Если вдруг персонаж после смены кадра говорит всего один слог, заканчивайте строку на ключ-кадре. Зритель не заметит, что хвостик проговаривается, когда субтитры пропали.
![](https://lh4.googleusercontent.com/qxKZ-iGKnLlah97tRvgcVKYg90XMXGaSKEcOWQU6SRZVoUDAZRgv1BZ8kdY7NxBKGsAi2gYH8hBkMaR9gnne4CrvOdviVbr8w2_iQdom3Rn6DdwVV331dmtGdyVIytuPwq4aagOh)
-   Если персонаж начинает говорить за 100 миллисекунд до смены кадра, то, в отличие от прошлого случая, начинать нужно не с ключ-кадра, а с того момента, когда начинает говорить персонаж. Зритель заметит, что голос уже появился, а сабов ещё нет.![](https://lh3.googleusercontent.com/jB6Wz9Q7dZs3_i9N1iWhA6DlLii3NMCSMBIBSZah04doGjUhO5yPno8wN_mQh9UK7aNl1NowlExoM66xkUdEWyaaeCItkRx8n-jKG99sa2ArS6khfTYi9mX9r1yXh9_jKM39_SWf)

Предлагаю также ознакомиться с видео-примерами работы с таймингом.

-   [Видео 1](https://yadi.sk/i/jXA_TcPV3MbpDz)
    
-   [Видео 2](https://yadi.sk/i/tQrobHiC3MbpEk)
