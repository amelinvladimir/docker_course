# Установка Docker на Windows 10

В данной инструкции мы устанавливаем Docker Desktop вместе с wsl2. 
Установка wsl2 не является обязательной, но при его установке вы сможете работать в Windows также как в Linux/MacOS. 
Если вы хотите установить только Docker Desktop без wsl2, то сразу переходите к Этапу 4.

## Этап 1. Проверяем, что включена опция Hyper-V Windows.
Hyper-V для создания виртуальных машин в Windows 10.

[Официальная инструкция от Microsoft.](https://learn.microsoft.com/ru-ru/virtualization/hyper-v-on-windows/quick-start/enable-hyper-v)

#### Шаг 1. Щелкните правой кнопкой мыши кнопку Windows и выберите пункт "Приложения и компоненты".
![image](https://github.com/user-attachments/assets/a0724f2f-2ff0-4fb2-8ec1-767ae7bdc2aa)

#### Шаг 2. Выберите Программы и компоненты справа в разделе связанные параметры.
![image](https://github.com/user-attachments/assets/6b197a51-427b-48a8-8f78-d1793461aa73)

#### Шаг 3. Выберите пункт Включение или отключение компонентов Windows.
![image](https://github.com/user-attachments/assets/1b3f807d-0aef-495a-b449-1aadf7655e6a)

#### Шаг 4. Включите Hyper-V.
Найдите Hyper-V в списке, если он там есть (если Hyper-V в списке нет, то его надо будет установить. Смотри следующий пункт). Если галочка не стоит, то поставьте ее и нажмите кнопку ОК.
![image](https://github.com/user-attachments/assets/43f96ec9-3df6-4173-be45-dc0608381dc7)

## Этап 2. Устанавливаем Hyper-V, если он не установлен (не был найден на предыдущем шаге).

#### Шаг 1. Запустите PowerShell или сеанс CMD от имени администратора.
Введите в строке поиска "Powershell".
В списке найденных приложений нажмите правой кнопкой мэши на "Windows PowerShell".
Выберите пункт "Запуск от имени администратора".

![image](https://github.com/user-attachments/assets/77f3a856-3e22-43e5-8bb5-f3448bee8621)

#### Шаг 2. Запустите команду установки.
````
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All
````

#### Шаг 3. После завершения установки выполните перезагрузку компьютера.

#### Шаг 4. Вернитесь к Этупу 1 "Проверяем, что включена опция Hyper-V Windows".

## Этап 3. Установите wsl2.

[Официальная инструкция от Microsoft.](https://learn.microsoft.com/ru-ru/windows/wsl/install)

#### Шаг 1. Запустите PowerShell или сеанс CMD от имени администратора.
Введите в строке поиска "Powershell".
В списке найденных приложений нажмите правой кнопкой мэши на "Windows PowerShell".
Выберите пункт "Запуск от имени администратора".

![image](https://github.com/user-attachments/assets/77f3a856-3e22-43e5-8bb5-f3448bee8621)

#### Шаг 2. Выполните команду установки

````
wsl --install
````
Эта команда включит функции, необходимые для запуска WSL и установки дистрибутива Ubuntu для Linux. 

#### Шаг 3. Установите Ubuntu.

Выполните команды
````
wsl --list
wsl --install -d Ubuntu-22.04
````

## Этап 4. Установка Windows Terminal и запуск Ubuntu.

#### Шаг 1. Установите Windows Terminal.
Открываем Microsoft Store.

![image](https://github.com/user-attachments/assets/2f15a8ef-9d6d-4a5e-8dd0-04972ce7c9b4)

Вводим в поиске "Windows Terminal".

![image](https://github.com/user-attachments/assets/eafa1c48-8c50-4163-8f77-2ee99bf1977d)

Устанавливаем найденное приложение.

![image](https://github.com/user-attachments/assets/a4eae157-d12f-48bf-870c-9f6dba7f3f94)

Введите в строке поиска "Терминал" и запустите найденное приложение.
![image](https://github.com/user-attachments/assets/5a531d46-490a-4a85-84b4-ab4610f34e09)

#### Шаг 3. Запустите Ubuntu.
Нажимаем на стрелку вниз в списке вкладок и выбираем "Ubuntu".
![image](https://github.com/user-attachments/assets/637653da-1e63-4e56-91e5-95c66e77f472)

Ubuntu запущен и открыто окно терминала :partying_face:
После установки Docker Desktop вы сможете работать в этом окне с Docker также как в Linux.
![image](https://github.com/user-attachments/assets/38c53199-e225-433f-b03c-1f5bcba17ff4)


## Этап 5. Установка и настройка Docker Desktop.

#### Шаг 1. Скачайте дистрибутив по [ссылке](https://www.docker.com/products/docker-desktop/).

#### Шаг 2. Установите Docker Desktop из дистрибутива.

#### Шаг 3. Запустите Docker Desktop.
![image](https://github.com/user-attachments/assets/b4bc9c0b-f9f4-4902-b2f3-f48475247ce1)

#### Шаг 4. Откройте настройки.
Нажимаем на шестеренку в правом верхнем углу.
![image](https://github.com/user-attachments/assets/a79aa22b-1904-47a4-bc66-04076bd09c15)

#### Шаг 5. Поставьте галочку в разделе "General" в пункте "Use the WSL2 based engine".
![image](https://github.com/user-attachments/assets/977663d3-d3ad-428e-bdb5-77201b980af9)

#### Шаг 6. Включите интеграцию с wsl2.
В разделе "Resources"->"WSL Integration" ставим галочку в "Ubuntu ..." и нажимаем кнопку "Apply & restart".
![image](https://github.com/user-attachments/assets/e887fd45-24b7-492d-8fc2-7decea524113)

# Установка Docker и wsl 2 на Windows 10 успешно завершена :partying_face:
