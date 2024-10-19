
|                          |                                       Заметка                                        |
| :----------------------: | :----------------------------------------------------------------------------------: |
|       Курсач TODO        |                                       [[TODO]]                                       |
| Структура Курсача и ВКР  |                             [[Структура Курсача и ВКР]]                              |
|      Мудрости жизни      |                                    [[Осознание]]                                     |
| Что-то про писательство  |                              [[Принципы писательства]]                               |
|    Подготовка к дему     |                                   [[План + время]]                                   |
| шпаргалка по API ASP.NET |                             [[Шпаргалка по ASP.NET API]]                             |
| ***Синтаксис Обсидиан*** | [Синтаксис](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax) |
|  ***Гайд на DataView***  |  [Гайд](https://blacksmithgu.github.io/obsidian-dataview/annotation/add-metadata/)   |
|      Типы диаграмм       |                                  [[Типы диаграмм]]                                   |


```dataviewjs
const today = DateTime.now()
const endOfYear = {
    year: today.year,
    month: 12,
    day: 31
}

const lifespan = { year: 80 } 
const birthday = DateTime.fromObject({
    year: 2005,
    month: 2,
    day: 6
});
const deathday = birthday.plus(lifespan)

function progress(type) {
    let value;
    
    switch(type) {
        case "lifespan": 
            value = (today.year - birthday.year) / lifespan.year * 100;
            break;
        case "year":
            value = today.month / 12 * 100
            break;
        case "month":
            value = today.day / today.daysInMonth * 100
            break;
        case "day":
            value = today.hour / 24 * 100
            break;
    }
    return `<progress value="${parseInt(value)}" max="100"></progress> | ${parseInt(value)} %`
}


dv.span(`
|  | Прогресс  | Процент |
| --- | --- |:---:|
| **Год** | ${progress("year")}
| **Месяц**| ${progress("month")}
| **День**| ${progress("day")}
`)
```

