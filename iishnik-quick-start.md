# Краткий курс молодого ИИшника

(специально для b17)

## Предупреждения и отмазки

**Внимание**: использование chatGPT может вызвать нарушения мышления, но это не точно. Хотя в недавнем исследовании американцы выяснили, что они от этого тупеют https://www.brainonllm.com/ . Если вы в себе уверены (по Даннингу-Крюгеру), бояться нечего.

**Ахтунг:** хотя компании говорят что ваши данные надежно защищены, отправлять в чатик личные документы всё же не нужно.

**Главное правило: У LLM и ветра не спрашивай совета: оба скажут в ответ - что да, то и нет © J.R.R.Tolkien**

## Урок 1. Матчасть

- Как искусственные нейросети «думают» и что можно сказать об их знании. https://www.b17.ru/blog/530871/
- Антропоморфизация искусственного интеллекта: психологические эффекты, риски зависимости https://www.b17.ru/article/684538/
- Психология машин - https://www.b17.ru/blog/530624/

### Визуализации:

- https://ig.ft.com/generative-ai/
- https://bbycroft.net/llm
- https://poloclub.github.io/transformer-explainer/


**Домашнее задание:** расскажите о прочитанном своей бабушке так, чтобы она тоже поняла и была в глубоко в теме.

-----

## Урок 2. Набрасывание на ИИ-вентилятор

_Аксиома Кана. Если ничто другое не помогает, прочтите, наконец, инструкцию!_

- Руководство по промпт-инжинирингу: https://promptingguide.ai/ru
- Введение в промпт-инжиниринг НИУ ВШЭ: https://academika.ru/course/hse-prompt-engineering/
- От Сбера: https://developers.sber.ru/docs/ru/gigachat/prompts-hub/prompt-engineering

AI-Prompt-Writing-Teacher: https://gitflic.ru/project/sdsmirnov/ai-therapy-prompts/blob/?file=AI-Prompt-Writing-Teacher.md

**Проверка качества запроса:** Покажите ваш запрос тому, кто имеет минимальное представление о задаче, и попросите его следовать инструкциям. Если ему непонятно, то ИИ, вероятно, тоже будет сложно.


**Домашнее задание:**

- Составьте промпт для получения инструкций о том, как составлять промпты.
- Расскажите своему коту, что нового вы узнали. Спросите его совета, и дайте ему жрадло в благодарность.


-----

## Урок 3. Вредные советы для непрактичного использования

_"Было бы величайшей ошибкой думать" В.И.Ленин, ПСС, т.41, с.55._

1. chatGPT и подобные хороши как Википедия на максималках, или как переводчики, или для обобщения и помощи в структурировании/конспектировании текстов - т.е. когда используются именно как тупой инструмент.

2. Чтобы получить качественный ответ, ваш запрос уже должен содержать большую его часть, и вы уже должны хорошо разбираться в предметной области. Т.е. чем больше вы сами эксперт, тем менее вам нужен ИИ, но когда нужен - пользы больше.

3. Задавайте роли, например: _“Ты Вася-психолог гуманистического направления, который будет задавать мне вопросы, чтобы я разобрался в своей проблеме с тревожностью. Да, ты ещё и наглый гопник.”_
Ещё пример : https://www.b17.ru/article/683012/
AI-Not-Therapist: https://gist.github.com/SDSmirnov/19baebc12aa008c5ab2061e3615882f3

4. Делайте запросы на критику вашего мнения, типа _"Теперь включай режим предельно жесткой критики, с чёрно-белым мышлением. Что скажешь о моей идее? А о своём предыдущем ответе? ОК, возвращаемся к конструктивному режиму"_ или _"Рассмотри это в роли Адвоката Дьявола", "в роли злого эксперта"_ и т.д.

5. Сохраняйте понимание: когда LLM генерирует текст, она опирается на внутреннюю модель контекста, который она получила до текущего момента. Проблема возникает, потому что **LLM интерпретирует этот контекст так, будто пользователь полностью усвоил, понял и принял каждое сгенерированное предложение**. Это очень неявное, но фундаментальное ограничение. Из-за этого возможно кумулятивное накопление ошибок.

6. Эффективный объем чата для конкретной проблемы - **до 30-50 реплик** с каждой стороны. Далее начинается дрифт контекста, "забывание", пользователь помнит больше чем модель. Пробелы в контексте модель может начать заполнять галлюцинациями. Просите модель составить конспект для нового чата, сохраняйте конспект или весь журнал.

7. Просите меньше врать (хоть это почти бесполезно): _"Если ты не уверен на 100%, просто скажи 'я не знаю'. Не выдумывай. Отвечай только на основе проверенных фактов. Ссылайся на источник, а если не можешь — скажи 'не знаю'"_

8. Не доверяйте никому (мне тоже): хотя ответы от одного ИИ можно перепроверить в другом ИИ - из chatGPT в deepseek/Grok для взаимокомпенсации галлюцинаций, все значимые результаты уточняйте по оригиналам публикаций/документации. Ответственность за применение ответов от чатика в реальной жизни - только ваша. А у чатика - лапки.

9. Если ответ вам непонятен, неполон, ошибочен - исправляйте запрос или указывайте на ошибку сразу. Или начинайте чат заново. Если через 10 минут вы не можете вспомнить, что вам ответил чатик - значит оно вам и не надо было.

Ещё практические советы: https://habr.com/ru/articles/921136/

Помните, что ИИ (_“искусственный идиот”_) - это только сложный вероятностно-статистичекий алгоритм, и близко не человеский разум. Он даёт только **опасную иллюзию понимания**. А ответы от человека отражает именно его _понимание_. Ответ от нейронки - отражает только _соответствие паттерна_ с запросом и контекстом.

**Пока ИИ не знает как пахнет его кровь, бесконечно он далёк от человека.**


_//proudly made with sarcasm//_