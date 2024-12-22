# Workshop_3
Отчет по лабораторной работе #3 выполнил(а):

Костерин Дмитрий Николаевич
АТ-05, НМТ-230802 Отметка о выполнении заданий (заполняется студентом):
Задание	Выполнение	Баллы
Задание 1	*	
Задание 2	*	
Задание 3	*	
знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:

к.т.н., доцент Денисов Д.В.
к.э.н., доцент Панов М.А.
ст. преп., Фадеев В.О.
Цель работы
Разработать оптимальный баланс нанесения урона оружием для игры Save RTF

Задание 1
###Задание 1. Расширьте варианты доступного оружия в игре. Используйте шаблон таблицы для визуализации оружия игры Save RTF.
![image](https://github.com/user-attachments/assets/f771db8b-8406-4602-aa67-ebf7febb980c)





Задание 2
###Задание 2. Визуализируйте параметры оружия в таблице.Используйте шаблон таблицы для визуализации оружия игры Save RTF. Постройте примеры для следующих математических величин (см. пример в презентации):

Среднеквадратическое отклонение
Разброс урона оружия
Вариативность времени отклика игрока
![image](https://github.com/user-attachments/assets/230d532d-3a82-4304-828b-4afd709aa784)
Анализ времени отклика игрока проводил на статистическом наборе данных.

reaction_times = np.random.normal(loc=500, scale=40, size=20)

plt.figure(figsize=(10, 6))
plt.plot(reaction_times, 'o-', color='teal')
plt.axhline(reaction_times.mean(), color='red', linestyle='dashed', label=f'Среднее: {reaction_times.mean():.2f} мс')
plt.fill_between(range(20), reaction_times.mean() - np.std(reaction_times), reaction_times.mean() + np.std(reaction_times), color='lightgreen', alpha=0.3, label=f'СКО: ±{np.std(reaction_times):.2f} мс')
plt.legend()
plt.title('Время реакции игрока')
plt.xlabel('Событие')
plt.ylabel('Время (мс)')
plt.show()

Задание 3
###Задание 3. Решение в 80+ баллов должно визуализировать данные из google-таблицы, и с помощью Python передавать переменные в проект Unity. В Python данные также должны быть визуализированы.
![image](https://github.com/user-attachments/assets/dc285c5d-22f5-4268-967d-acf86df3bf5e)




Выводы:
Расширил варианты доступного оружия в игре. Визуализировал параметры оружия в таблице. Перенес данные в Unity.

Powered by
BigDigital Team: Denisov | Fadeev | Panov
