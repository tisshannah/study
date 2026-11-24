## 1
* ![alt text](image-1.png)
* ![alt text](image-3.png)
* ![alt text](image-4.png)
* ![alt text](image-5.png)
* ![alt text](image-6.png)
* ![alt text](image-9.png)
* ![alt text](image-8.png)

## 2
* проделала то же самое с новым интерфейсом enp0s9
* пинг проходит 
* ![alt text](image-10.png)

## 3
* созданы 2 пользователя
* вход работает ![alt text](image-11.png)
* ![alt text](image-12.png)

## 4
* установка ssh 
* ![alt text](image-13.png)
* конфиг файл ssh
* ![alt text](image-16.png) ![alt text](image-15.png)
* файл баннера
* ![alt text](image-14.png)
* ![alt text](image-17.png)
* ![alt text](image-18.png)

## 5
* это веб сервер
* ![alt text](image-19.png)
* это дата
* ![alt text](image-20.png)
* ![alt text](image-21.png)
* ![alt text](image-22.png)
* пинг проходит
* ![alt text](image-23.png)
* то же и на дате
* ![alt text](image-24.png)

## 6
* проверка дисков
* ![alt text](image-25.png)
* создание и форматирование 
* ![alt text](image-26.png)
* ![alt text](image-27.png)
* ![alt text](image-28.png)
* ![alt text](image-29.png)

## 7
* -t nat таблица отвечает за изменение ip в пакетах, в отличие от стандартной F, которая разрешает/блок пакеты. цепочка postrouting - на выходе из сервера. -s == source, источник, правило только для подсети нужной. -o == output, -j masquerade == jump. Заменяет локальный адрес отправителя на текущий ip интерфейса enp0s3 и запоминает соединение для возврата. Есть еще dnat (меняется ip получателя)
* ![alt text](image-30.png)
* сохранить правило и вкл службу в автозагрузку
* ![alt text](image-31.png)
* потом в sysctl.conf разрешить маршрутизацию
* применить настройки
* ![alt text](image-32.png)
* указать шлюз и днс серверы в конфиг файлах
* ![alt text](image-33.png)
* ![alt text](image-34.png)
* флаг -n отключает поиск доменных имен и показыват ip 
* ![alt text](image-35.png) 

## 8
* ![alt text](image-36.png)
* ![alt text](image-37.png)
* ![alt text](image-38.png)
* ![alt text](image-39.png)
* настройка второй машины
* ![alt text](image-40.png)
* ![alt text](image-41.png)

## 9
* ![alt text](image-42.png)
* ![alt text](image-45.png)
* ip
* ![alt text](image-46.png)
* ![alt text](image-47.png)
* resolv.conf
* ![alt text](image-67.png)
* вкл пересылку пакетов и установить шлюз
* ![alt text](image-48.png)
* ![alt text](image-49.png)
* ![alt text](image-50.png)
* ![alt text](image-68.png)
* пишу это в файл options.conf
* ![alt text](image-51.png)
* в файле rfc1912.conf
* ![alt text](image-52.png)
* создание файла прямой зоны
* ![alt text](image-54.png)
* ![alt text](image-55.png)
* создание файла обратной зоны
* ![alt text](image-56.png)
* ![alt text](image-57.png)

* генерация ключа управления rndc
* ![alt text](image-61.png)
* ![alt text](image-64.png)
* ![alt text](image-65.png)
* запускается так
* ![alt text](image-66.png)
* ![alt text](image-69.png)