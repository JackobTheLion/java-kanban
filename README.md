# java-kanban
Repository for homework project.

# Трекер задач
### Простейший трекер задач, содержащий три типа задач:
* задача
* эпик задача (задача состоящая из подзадач)
* подзадача

#### При этом: 
* Для каждой подзадачи известно, в рамках какого эпика она выполняется.
* Каждый эпик знает, какие подзадачи в него входят.
* Завершение всех подзадач эпика считается завершением эпика.

#### Каждая задача имеет:
1. Имя
2. Описание
3. Уникальный ID
4. Cтатус:
   1. NEW
   2. IN_PROGRESS
   3. DONE

#### Для задач и подзадач статус определяет пользователь, для эпиков рассчитиывается автоматически по следующим условиям:
* если у эпика нет подзадач или все они имеют статус NEW, то статус должен быть NEW.
* если все подзадачи имеют статус DONE, то и эпик считается завершённым — со статусом DONE.
* во всех остальных случаях статус должен быть IN_PROGRESS.