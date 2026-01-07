**1.Выведите содержимое fstab. Что хранится в fstab?**
/etc/fstab — это файл конфигурации, содержащий информацию о файловых системах, которые монтируются автоматически при загрузке системы.
<img width="968" height="144" alt="image" src="https://github.com/user-attachments/assets/a0b401b8-e127-4af0-ac54-e8762566e1d2" />

**2.Добавьте в виртуальную машину ещё один диск**
Через интерфейс UTM был добавлен новый виртуальный диск.

**3.Узнайте как ситема видит ваш диск - выведите информацию о блочных устройствах**

Команда lsblk показала доступные диски в системе. Новый диск определился как /dev/vdb.

<img width="418" height="164" alt="image" src="https://github.com/user-attachments/assets/b2681811-d2fc-4191-bb41-e6702f9c09f3" />

**4.С помощью полученной информации создайте на диске таблицу разделов и фаловую систему ext4**

Создана таблица разделов GPT.Создан раздел на весь диск.Создана файловая система ext4.

<img width="654" height="498" alt="image" src="https://github.com/user-attachments/assets/638249c4-8856-4480-91d0-75abb56ec1e2" />

**5.Примонитруте диск в каталог /mnt**

<img width="678" height="146" alt="image" src="https://github.com/user-attachments/assets/b8018f86-e75f-4d2c-b450-f329e2cae13c" />

**6.Зайдите в каталог и создайте там файлы**

<img width="404" height="81" alt="image" src="https://github.com/user-attachments/assets/73aaecfe-33e9-41f4-a85c-49d5ee39ed31" />

**7.Отмонтируйте диск и проверье остались ли файлы**

Отмонтирую с помощью umount, затем снова примонтирую и проверю файлы

<img width="423" height="98" alt="image" src="https://github.com/user-attachments/assets/9d62027e-6189-43fd-97fe-eb6a8e1606ae" />

**8.Сделайте так чтобы диск автоматически подключался при загрузке систем ( добавьте информацию о нём с fstab). 9.Проверьте корретность записанных в fstab данных перед перезагрузкой**

Сначала узнаю UUID раздела с помощью blkid и добавлю его в fstab
<img width="1458" height="258" alt="image" src="https://github.com/user-attachments/assets/485f3cdf-df4e-4e40-8e19-857afe78a00a" />

**10.Перезагрущите систему и убедитесь что диск был подключён к системе**

<img width="630" height="87" alt="image" src="https://github.com/user-attachments/assets/b59e9139-3116-4b98-87e1-c123c831f712" />
<img width="533" height="69" alt="image" src="https://github.com/user-attachments/assets/f89d2e25-c5ba-4bd5-80a4-e76420433a5d" />


