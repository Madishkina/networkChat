# networkChat
Курсовой проект "Сетевой чат"

Описание.
Проект позволяет реализовать обмен текстовыми сообщениями по сети с помощью консоли (терминала) между двумя и более пользователями. 

Сервер чата, должно ожидать подключения пользователей. В бесконечном цикле while(true) сервер ждет новые подключения и добавляет их в коллекцию. 
При получении сообщения от любого клиента, сервер отправляет его остальным клиентам, включая отправителя.    

Второе приложение - клиент чата, подключается к серверу чата и осуществляет доставку и получение новых сообщений.
В классе клиента реализовано два потоков – один слушает новые сообщения от сервера и печатает их в консоль, 
второй читает вывод из консоли и отправляет серверу.

Все сообщения должны записываются в file.txt и дополняется при каждом запуске, а также при отправленном или полученном сообщении. 
Выход из чата осуществляется по команде /exit.
Установка порта и ip осуществляется через редактирование файла settings.txt
