
# Образование и опыт:
###  1999 - 2003
Сахалинское училище искусств

Инструментальное исполнительство (скрипка).


- Параллельно изучал звукорежиссуру и практиковался в работе с оборудованием студии звукозаписи.


- Программировал расположения звуков во времени и пространстве при помощи аппаратных секвенсоров.

---
###  2003 - 2005
Новосибирский музыкальный колледж

Инструментальное исполнительство (скрипка).
- Параллельно с обучением хорошо освоил стек программного обеспечения для production и post-production мультимедиа
(Cubase, Nuendo, Logic, WavLab, SoundForge, Vegas Pro, Adobe Premiere)


- Программировал паттерны для секвенсоров.

---
###  2005 - 2011 
Новосибирская Государственная Консерватория-академия им. Глинки
- Параллельно с обучением читал лекции по информатике и преподавал цифровую звукорежиссуру.


- Обслуживал локальную компьютерную сеть отдела ЦМИ (цифровых музыкальных инструментов) ДШИ№7 им.Новикова.


- Оптимизировал системы управления базами данных библиотек NI-Kontakt


- Автоматизировал процессы интеграции семпловых библиотек и конвертации медиа данных с целью увеличения производительности.


- При помощи DAW (Digital Audio Workstation) и сопутствующего стека технологий создавал музыкальные композиции широкого спектра жанров.


- Изучал web-разработку (HTML, JavaScript).
  - Создал сайт-визитку для музыкального коллектива.

---
###  2011 - 2013
- Модифицировал код скриптов VSTi NI-Kontakt

  (SDK NI-Kontakt)


- Занимался звукозаписью, сведением и мастерингом.

  (Cubase, VST, VSTi)


- Монтировал и обрабатывал видео.

  (Adobe Premiere, Vegas, DaVinci, ffmpeg, batch scripting)


- Автоматизировал процессы резервного копирования данных.
  
  (batch scripting)

---
###  2013 - 2015
- Автоматизировал процессы бухгалтерского и складского учета ММО гильдии составом более 500 игроков. 
  
  (Google Spreadsheets, Google Forms, SQL)

 
- Создал интернет-магазин с игровыми товарами

  (PrestaShop)


- Автоматизировал процесс импорта товаров в базу данных магазина из Google Spreadsheets.

  (PHP, Google Spreadsheets, Google API)


- Автоматизировал сбор и обработку различной информации от пользователей.

    (PHP + MySQL).

[![dlVideo.png](https://github.com/symphograph/resume/blob/master/img/dlVideo.png)](https://youtu.be/wEt0Q3MnoCw)


---
###  2015 - 2017

- Разработал первую версию сайта [<b>DeadLegion</b>](https://dllib.ru) для игроков MMO ArcheAge 

  (PHP, MySQL, jQuery) 

    [Репозиторий в Githab](https://github.com/symphograph/dllib)
    
    Сайт предоставляет рад вычислительных сервисов для игрового процесса и взаимодействия пользователей
  - Основные возможности:
      - Калькуляция себестоимости предметов.
      - Вычисление оптимальной структуры дерева крафта
      - Вычисление оптимальной логистики.
      - Симуляция действий, результат которых имеет определенную вероятность.
      - Получение и обработка данных от пользователей
    

- Сотрудничал с компанией Animacord LTD (Проект: "Маша и Медведь")
  - Создал аранжировки и фонограммы для мюзикла "Маша и Медведь"

    (Cubase, VST, VSTi)


- Изучал интерфейс и API DAW Reaper.
---
###  2017 - 2020

- #### Разработал первую версию проекта [<b>SymphoStaff</b>](https://github.com/symphograph/SymphoStaff)
   CRM для автоматизации бизнес-процессов камерных и симфонических оркестров

   (PHP, MySQL, jQuery, Vue)


- Разрабатывал скрипты для DAW Reaper
  
  (Lua, Python)

  Пример кода:

    ```lua
    
    local function hideCoupledAudioTracks()
      -- Iterate through all tracks in reverse order
      for i = reaper.CountTracks(0) - 1, 0, -1 do
        local track = reaper.GetTrack(0, i)
        if track then
          local trackGUID = reaper.GetTrackGUID(track)
          local isCoupled = reaper.GetProjExtState(0, 'levitanus_inst_track_audio', trackGUID)
    
          if isCoupled == '1' then
            reaper.SetMediaTrackInfo_Value(track, 'B_SHOWINTCP', 0)
          end
        end
      end
    end
    
    -- Prevent UI refresh during the operation
    reaper.PreventUIRefresh(1)
    hideCoupledAudioTracks()
    reaper.PreventUIRefresh(-1)
    
    ```



---

### 2020 - 2021 
- Разработал приложение автоматизирующее заполнение отчетов о нагрузке для преподавателей ТГИК (Тюмень)

  (PHP, HTML)

- Разработал уровень игрового платформера.

  (Unity, C#)

- Продолжал работу над проектом [<b>SymphoStaff</b>](https://github.com/symphograph/SymphoStaff)

---

###  2021 - н.в.

- Разработал библиотеку [<b>Bicycle</b>](https://github.com/symphograph/bicycle) с обширным набором классов для упрощения разработки.

  (PHP 8.2)

    Содержит классы, трейты и интерфейсы для:
    - работы серверным окружением
    - взаимодействия с базой данных и маппинга
    - генерации и валидации JWT
    - работы с файлами, строками и массивами
    - централизованного перехвата ошибок и их обработки
    - ведения логов в json
    - генерации json ответов для предоставления API
    - реализации логики взаимодействия сервисов
    
    
- Разработал [сервер JWT авторизации](https://github.com/symphograph/authServer).

    (PHP 8.2) 

    Сервер обеспечил взаимодействие между сервисами, размещенными на разных ресурсах.


- Продолжал работу над проектом [<b>SymphoStaff</b>](https://github.com/symphograph/SymphoStaff)


- Разработал новую версию сайта для игроков MMO ArcheAge.

    [Frontend](https://github.com/symphograph/ArcheAgeTools_Frontend), [Backend](https://github.com/symphograph/ArcheAgeTools_API)

---
