**1. Установите пакет samba**
<img width="1268" height="814" alt="image" src="https://github.com/user-attachments/assets/ad0da854-4e24-4fcf-b633-ac25a9e0c0a9" />
<img width="1044" height="722" alt="image" src="https://github.com/user-attachments/assets/9e229113-4152-473d-be1f-a43381ba6ebe" />
<img width="809" height="384" alt="image" src="https://github.com/user-attachments/assets/3c150b4f-28c3-4c34-965a-1c9443c7c3eb" />
**2. ЧТо такое побщая папка, зачем оно может быть нужно?**

Общая папка в Samba — это каталог в Linux, к которому можно получить доступ по сети с других компьютеров (Linux, Windows, macOS).
Она используется для обмена файлами, совместной работы, хранения общих документов или резервных копий.

**3. Создайте общую папку без пароля с правами только на чтение файлов**

<img width="489" height="81" alt="image" src="https://github.com/user-attachments/assets/d4f2637f-21d5-458e-8379-5dda398b81f0" />
Добавил в конец файла smb.conf
<img width="285" height="118" alt="image" src="https://github.com/user-attachments/assets/38f17cde-1852-4c5f-bc2a-9329bbdef871" />

**4. Создайте общую папку с паролем с правами на чтение и запись**
<img width="1037" height="830" alt="image" src="https://github.com/user-attachments/assets/328bdbc6-a61f-4460-9964-6e077fdb0807" />

Добавил в конец файла smb.conf
<img width="556" height="219" alt="image" src="https://github.com/user-attachments/assets/d9488b4a-7cf6-4cca-946c-4f326590c6c3" />
перезапустил systemctl restart smb
Доступ по логину и паролю, чтение и запись

**5. Создайте общую папку с доступом для какой-то группы с полными правами**

<img width="932" height="461" alt="image" src="https://github.com/user-attachments/assets/f57c9442-c0c9-46e0-89d9-04763adbf56c" />

Добавил в конец файла smb.conf
<img width="560" height="186" alt="image" src="https://github.com/user-attachments/assets/78998892-85cd-4fb4-8297-d878b3777d62" />
**6. Создайте общую папку в которой у одной группы будет полный доступ, а у другой только доступ на чтение. Третья группа не должна иметь к ней доступа**
<img width="1087" height="821" alt="image" src="https://github.com/user-attachments/assets/85f614bc-329c-48bb-b43c-44b3ed78c008" />

Добавил в конец файла smb.conf

<img width="683" height="230" alt="image" src="https://github.com/user-attachments/assets/b9135df8-eb01-45ca-922f-9c68f114bbe1" />

fullaccess — полный доступ, readonly — только чтение, другие пользователи — доступа нет
