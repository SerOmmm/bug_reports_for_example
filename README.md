**Примеры баг-репортов**

<details>
<summary>BG-001: Клик на лого "SK Участник" в подвале главной страницы «xPress» перенаправляет на главную страницу "Сколково".</summary>

***

**Шаги воспроизведения**:
1.	Открыть главную страницу https://express.ms/
2.	Проскроллить страницу до подвала сайта
3.	Нажать на лого "SK Участник"

**ОР**: Клик на лого "SK Участник" перенаправляет на карточку компании "xPress"  на сайте "Сколково", в HTML-разметке указана ссылка https://navigator.sk.ru/orn/1123784
``` 
<a href="https://navigator.sk.ru/orn/1123784" target="_blank" title="Cколково"></a>
```

**ФР**: Клик на лого "SK Участник" перенаправляет на главную страницу "Сколково", в HTML-разметке указана неверная ссылка https://sk.ru/
``` 
<a href="https://sk.ru/" target="_blank" title="Cколково"></a>
```

![Screenshot](https://github.com/SerOmmm/bug_reports_for_example/blob/main/Screenshot_3.png)

**Окружение**: 
PC (Windows 10), Chrome 120.0.6099.225, разрешение 1920х1080 <br>
Xiaomi Redmi 11 Pro 5G (Android 13), Chrome mobile  120.0.6099.230, разрешение 1080x2400

**Серьезность**: Minor <br>
**Приоритет**: Medium

***

</details>

