# Причины и признаки сложного кода (лекция 8)

Правило: исбавляйтесь от нопределенности в коде как можно раньше

```c++
for (pair<string, int> p: getInfo()) {
    // надо сразу пояснять кодом, что такое first, 
    // а что такое second в p
    string attribute = p.first;
    int value = p.second;
    ...
} 
```

```java
// старайтесь сразу избавляться от optional и nullable переменных
Optional<Long> studentIdOpt = getStudentId();

if (studentIdOpt.isPresent()) {
    long studentId = studentIdOpt.get();
    ...
} else {
    ...
}
```

```java
// если пользуетесь массовой апи для нахождения одного конкретного элемента
// то сразу вытаскивайте его из списка
List<String> teamNameInList = getTeamNamesByIds(singletonList(1L));

if (teamNameInList.size() == 1) {
    String teamName = teamNameInList.get(0);
    ...
} else {
    throw new RuntimeException();
}
```

Чем более знание локально, тем легче система. Например, если вы используете неочевидную аббревиатуру в одном файле, система выходит проще, чем если бы вы её использовали во всем модуле/проекте

Локальность знаний облегчает понимание и снижает риски при внесении правок в код

