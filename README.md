### Задание 1. Создать Deployment и обеспечить доступ к репликам приложения из другого Pod

1. Создать Deployment приложения, состоящего из двух контейнеров — nginx и multitool. Решить возникшую ошибку.
<img width="921" height="112" alt="image" src="https://github.com/user-attachments/assets/5e276b19-9dde-44a8-9d6e-fd8c172ad024" />

2. После запуска увеличить количество реплик работающего приложения до 2.
3. Продемонстрировать количество подов до и после масштабирования.
<img width="1088" height="139" alt="image" src="https://github.com/user-attachments/assets/d3d779d6-1ca3-479c-bf5b-55d3b1d6f2d6" />
4. Создать Service, который обеспечит доступ до реплик приложений из п.1.
5. Создать отдельный Pod с приложением multitool и убедиться с помощью `curl`, что из пода есть доступ до приложений из п.1.
<img width="831" height="121" alt="image" src="https://github.com/user-attachments/assets/fca675a8-06ad-4587-88b9-5c06bb872167" />
<img width="1054" height="693" alt="image" src="https://github.com/user-attachments/assets/d6ca503d-fb17-488f-83dd-9c4cd492e747" />

------

### Задание 2. Создать Deployment и обеспечить старт основного контейнера при выполнении условий

1. Создать Deployment приложения nginx и обеспечить старт контейнера только после того, как будет запущен сервис этого приложения.
2. Убедиться, что nginx не стартует. В качестве Init-контейнера взять busybox.
<img width="981" height="118" alt="image" src="https://github.com/user-attachments/assets/fccdf597-98be-4d88-8b91-9f7eb15d7c4a" />
3. Создать и запустить Service. Убедиться, что Init запустился.
4. Продемонстрировать состояние пода до и после запуска сервиса.
<img width="961" height="238" alt="image" src="https://github.com/user-attachments/assets/dbc5a9a4-d571-41e2-8b6a-26628dc522f8" />
