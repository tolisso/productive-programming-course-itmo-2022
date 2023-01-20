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
