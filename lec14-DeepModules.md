# Глубокие модули (лекция 14)

Глубокий модуль (Deep Module) - модуль со огромной функциональностью и простым апи

Shallow Module - модуль который предоставляет мало функционала относительно сложности его апи

> Пример глубокого модуля: Unix File System
>
> ![image](https://user-images.githubusercontent.com/57497898/213894598-35797d4f-ebae-472f-ae82-67a72c6b1476.png)

Shallow Module-и пораждают лишние зависимости и слои, что порождает Obscurity

Зачастую методы Shallow Module-ей можно спокойно заинлайнить. Но как же так, вдруг мы захотим логировать этот метод... You Aren't Gonna Need It.

Принцип YAGNI говорит о том, что для любой вещи, которая вам **возможно** пригодится потом, можно считать что она вам не пригодится.

Small Module - literally маленький модуль
- зачастую удобнее читать
- но те кто используют модуль чаще всего не читают

Проблемы small module-й
- нет уверенности в том что они достаточно глубоки и полезны
- если маленьких модулей много, то количество интерфейсов которые вам нужно знать зашкаливает
- приходится постоянно комбинировать кучу методов, но так очень сложно программировать

