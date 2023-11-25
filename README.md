# TOIB-PR-4 Vasiljew Grigoriy Maksimovich BBMO-02-23

1. Создаем 2 виртуальные машины на базе ОС Debian 12 и обеспечиваем между ними сетевой обмен

   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/1.JPG)

   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/2.JPG)

   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/3.JPG)
   
2. Включаем на 1-ой (сервере) из ВМ передачу логов по протоколу rsyslog на 2-ую ВМ (клиент)
   
   **Устанавливаем и настраиваем rsyslog на сервере и клиенте**

   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/4.JPG)

   **Проверяем работоспособность rsyslog на сервере и клиенте**

   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/5.JPG)

   **Включаем UDP и TCP соединение**

   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/6.JPG)

   **Устанавливаем правила на сервере**
   
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/7.JPG)

   **Установливаем правила на клиенте**
   
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/8.JPG)

   **Проверяем получения логов на сервере**
   
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/9.JPG)

   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/10.JPG)

3. Устанавливаем и настраиваем получение логов на сервере с использованием Loki
   
   **Установливаем и редактируем compose-файл на сервере**
 
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/11.JPG)
   
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/12.JPG)

   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/12.2.JPG)
   
   **Запускаем Loki**
 
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/13.JPG)
   
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/13.2.JPG)

   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/13.2.JPG)
   
   **Редактируем promtail на клиенте**
 
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/14.JPG)

   **Редактируем compose-файл для promtail**
 
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/15.JPG)
  
   **Запускаем promtail на клиенте**
 
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/16.JPG)

   **Просматриваем логи клиента в Grafana**
 
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/17.JPG)

   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/18.JPG)
 
 5. Устанавливаем и настроиваем получение логов на сервере с использованием Signoz

   _Установка Signoz по инструкции с сайта: https://signoz.io/docs/install/docker/#install-signoz-using-docker-compose_

   **Запускаем Signoz**
   
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/19.JPG)
   
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/20.JPG)
   
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/21.JPG)
   
   **Редактируем конфигурации на клиенте для отправки данных в Signoz**
   
   _Установка приложения sample-nodejs-app согласно инструкции с сайта: https://github.com/SigNoz/sample-nodejs-app/_
   
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/22.JPG)
   
   **Проверяем получение логов в Signoz**
   
   ![image](https://github.com/Archangel15520/toib3/blob/main/Screenshot/23.JPG)
   
