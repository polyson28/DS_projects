# Описание проекта
## Цель
Нам нужно защитить данные клиентов страховой компании с помощью преобразования данных. Необходимо разработать такой метод обработки, чтобы по данным было сложно восстановить персональную информацию, а также обосновать корректность его работы. Нужно защитить данные, чтобы при преобразовании качество моделей машинного обучения не ухудшилось. 

## Используемые инструменты
pandas, numpy, matplotlib, sklearn, линейная алгебра

## Вывод
- В процессе проекта мы доказали следующий факт с помощью методов линейной алгебры:
   - Если уножить признаки на обратимую матрицу, качество линейной регрессии не изменится, при условии, что модель можно обучить заново на новых признаках
- Доказательство выше упомянутого факта натолкнуло нас на следующую мысль: данные клиентов можно защитить домножением на обратимую матрицу Р, сгенерированную рандомным образом. Таким образом, персональные данные клиентов будут преобразованы, а качество регрессии не изменится
- Для моделей, построенных на изначальных и защищенных данных, качество регрессии получилось одинаковым - примерно 0.412
- Таким образом, цель данного проекта была выполнена: персональные данные клиентов были защищены, а качество линейной регрессии на преобразованных данных не изменилось

## Статус проекта
Завершен
