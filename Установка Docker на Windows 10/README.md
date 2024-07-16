# Установка Docker на Windows 10

## Этап 1. Проверяем, что включена опция Hyper-V Windows 
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

## Этап 2. Устанавливаем wsl2.

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
