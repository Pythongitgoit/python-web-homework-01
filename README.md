# Project Address_book
# Командний проект Python CLI Assistant "курс Python Core". TEAM_10

## [Презентація проекту](https://docs.google.com/presentation/d/1-O-7II6YCZ0ygWs47Ze4AorIQfSM5ccVOKKWGod-yjg/edit#slide=id.g10f42b85138_2_1005)

![Logo](https://github.com/VolodymyrPruhlo/Team_10_CP/blob/dev/Documentation/team_10.jpg)

## Table of Contents

- [Особливості](#Особливості)
- [Usage](#usage)
- [Commands](#commands)
- [Examples](#examples)
- [Installation](#installation)
- [License](#license)

## Особливості

Ваш особистий асистент сприятиме зберіганню списку ваших контактів (телефон, електронна пошта, дата народження, адреса), створенню нотаток та організації файлів у зазначеній директорії. При додаванні або редагуванні інформації буде автоматично перевірятися правильність введення номеру телефону, електронної пошти та дати народження.

За вашим окремим запитом асистент може виводити список контактів, у яких день народження припадає на зазначений вами період днів.

При створенні нотаток можливо додавати ключові слова, за якими можна проводити сортування та пошук. Сортування файлів у папці здійснюється за типами файлів: аудіо, відео, документи, зображення, архіви, інше. Команда "help" показує усі доступні команди для користувача .

## Usage
Adressbook - зберігає контакти у наступному виді:

    Contact name: John Doe, Email: john@example.com, Phone: 1234567890, Address: City, Street, 123, Birthday: 1990-01-01
    Contact name: Alice Smith, Email: alice@example.com, Phone: 9876543210, Address: Town, Avenue, 456, Birthday: 1985-05-15
    Contact name: Bob Johnson, Email: bob@example.com, Phone: 5551234567, Address: Village, Lane, 789, Birthday: 1978-08-20
    Contact name: Eva Davis, Email: eva@example.com, Phone: 1112223333, Address: Suburb, Park, 101, Birthday: 1992-03-10
    Contact name: Michael Brown, Email: michael@example.com, Phone: 9998887777, Address: Rural, Meadow, 505, Birthday: 1980-06-25      
    Contact name: Sophie White, Email: sophie@example.com, Phone: 4445556666, Address: Island, Beach, 222, Birthday: 1995-11-05

“Асистент” вміє працювати з нотатками + теги:

    List of all notes:
    1. Text: Meeting at 2 PM   
       Tags: work, meeting     
    2. Text: Grocery shopping  
       Tags: personal, shopping
    3. Text: Code review       
       Tags: work, development 
    4. Text: Book club meeting 
       Tags: personal, reading 
    5. Text: Project deadline  
       Tags: work, deadline
   
“Асистент” - сортує файли у зазначеній папці за такими категоріями:

    "Audio": [".mp3", ".ogg", ".wav", ".amr"]
     
    "Documents": [".docx", ".doc", ".txt", ".pdf", ".xlsx", ".pptx"],
    
    "Video": [".avi", ".mp4", ".mov", ".mkv"],

    "Image": [".jpeg", ".png", .jpg", ".svg"],

    "Archive": [".zip",".gz", ".tar"]
 
    "Unknown":[]



## Команди 

| Command Syntax        | Description                                                                                                                                                                                                              |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| add                   | "Додати контакт: Ця команда дозволяє вам додати новий контакт до адресної книги. Ви вводите ім'я, номер телефону, електронну пошту (за бажанням), адресу (якщо є) та дату народження (за бажанням) для нового контакту." |
| search {name}         | "Пошук контакту: Ця команда дозволяє вам знайти контакти за ключовим словом. Ви вводите ключове слово, і програма виводить контакти, які містять це слово в імені, телефоні, електронній пошті або адресі."              |
| delete                | "Видалити контакт: Ця команда дозволяє вам видалити контакт з адресної книги. Ви вводите ім'я контакту, який потрібно видалити."                                                                                         |
| add note              | "Додати нотатку: Ця команда дозволяє вам додати нову нотатку до своїх нотаток. Ви вводите текст нотатки та теги (якщо є)."                                                                                               |
| search note {keyword} | "Пошук нотатки: Ця команда дозволяє вам знайти нотатки за ключовим словом. Ви вводите ключове слово, і програма виводить нотатки, які містять це слово в тексті."                                                        |
| sort                  | "Сортування нотаток за тегами: Ця команда сортує ваші нотатки за тегами. Ви вводите тег, і програма виводить всі нотатки з цим тегом, впорядковані за ним."                                                              |
| sort folder           | "Ця команда сортує файли в папці за розширеннями, видаляє пусті папки."                                                                                                                                                  |
| hello                 | "Вивести привітання: Ця команда виводить привітання від бота."                                                                                                                                                           |
| close                 | "Завершити роботу: Ця команда завершує роботу програми та виводить прощання."                                                                                                                                            |
| clear                 | "Видалення данних: Ця команда видаляє всі збережені данні в нотатках та адресної книзі."                                                                                                                                 |
| change                | "Редагування контакту: Ця команда дозволяє змінити будь-яке поле контакту."                                                                                                                                              |
| all                   | "Вивід всіх наявних контактів: ця команда виводить список всіх контактів."                                                                                                                                               |
| all notes             | "Вивід всіх наявних нотатків: ця команда виводить список всіх нотаток."                                                                                                                                                  |
| change note           | "Редагування нотатків: ця команда дозволяє редагувати нотатки і теги."                                                                                                                                                   |
| delete note           | "Видалення нотатки: ця команда видаляє нотатку"                                                                                                                                                                          |
| help                  | "Список всіх команд"                                                                                                                                                                                                     |


## Examples
 
For more details and examples, please refer to the [documentation](./Documentation/).

## Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/python-cli-assistant.git
cd python-cli-assistant
```

2. Install dependancies:

```bash
pip install -r requirements.txt
```

3. Run the Python CLI Assistant:

```bash
python assistant.py
```

## License

MIT License.

## Contributors

- [Vova ](https://github.com/VolodymyrPruhlo)
- [Igor](https://github.com/Pythongitgoit)
- [Sergiy](https://github.com/SobkoSergiy)
- [Taras](https://github.com/)
- [Max](https://github.com/)
