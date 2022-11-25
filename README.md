# git
## Створення проекту (
репозиторія = repository)

### 1.На сторінці github створіть новий репозиторій і скопіюйте посилання на нього, натиснувши кнопку `Clone or download`. Посилання виглядає так:

```
https://github.com/ilyavf/tx-builder.git
```

### 2.Відкрийте термінал і склонуйте репозиторій таким чином:
```cmd
$ cd ~/dev
$ git clone https://github.com/ilyavf/tx-builder.git
$ cd tx-builder
```

Команда створить нову папку (якщо такої немає в поточній директорії) на ім'я проекту, в даному прикладі `tx-builder`.

3.Відкрийте проект у вашому улюбленому IDE.

#Робота з проектом

# Перегляд поточних змін у терміналі

## Перейдіть до папки з вашим проектом, наприклад:
```
cd ~/dev/tx-builder
```

### 1. Список змінених файлів:
```
$ git status
```

### 2.Перегляд поточних змін:
```
$ git diff
```

## Збереження поточних змін

### 1.Збереження у локальному репозиторії:
```
$ git commit -am "I made some changes. Put meaningful comment describing your changes"
```

### 2.  Відвантаження на віддалений репозиторій (github):
```
$ git push
```
- `git help` вбудована допомога git зі списком усіх доступних git-команд. Вихід із режиму перегляду - клавіша `q`.
- `git help <command>` допомога за окремими командами, наприклад: `git help status`
- `git clone <link to you repo>` копіювання віддаленого репозиторію на локальний диск (у поточній директорії буде створено папку за назвою проекту
- `git status` список файлів із поточними змінами
- `git diff` перегляд всіх поточних змін
- `git diff my-file.html` перегляд змін конкретного файлу
- `git commit -am "my comment about changes"`
- `git push` відвантаження коммітів на віддалений репозиторій
- `git log -5` перегляд останніх 5 коммітів
- `git log -1 -p` перегляд змін останнього комміту
- `git log -5 --name-status` перегляд останніх 5 коммітів із переліком змінених файлів
- `git log -1 -p f64b35` перегляд змін комміту з id `f64b35d28eaed0c127d07de66708d3f33a44d3f7` (досить 1х 5-6 символів)

### Прапори можна комбінувати, наприклад:
```
$ git log -1 --name-status f64b35
$ git log -5 -p
```
