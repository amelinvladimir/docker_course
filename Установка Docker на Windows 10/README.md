# Установка Docker на Windows 10

## Этап 1. Проверяем, что включена опция Hyper-V Windows 
Hyper-V для создания виртуальных машин в Windows 10.

[Официальная инструкция от Microsoft.](https://learn.microsoft.com/ru-ru/virtualization/hyper-v-on-windows/quick-start/enable-hyper-v)

#### Шаг 1. Щелкните правой кнопкой мыши кнопку Windows и выберите пункт "Приложения и компоненты".
![image](https://github.com/user-attachments/assets/9d9ab88f-0b12-4b2c-9f66-28bd10ab1a1e)

#### Шаг 2. Выберите Программы и компоненты справа в разделе связанные параметры.
![image](https://github.com/user-attachments/assets/3bab9492-666b-46a3-a6d4-87e6a8b5e888)

#### Шаг 3. Выберите пункт Включение или отключение компонентов Windows.
![image](https://github.com/user-attachments/assets/d92dbd92-93f2-465a-95c9-fafd651b3f72)

#### Шаг 4. Включите Hyper-V.
Найдите Hyper-V в списке, если он там есть (если Hyper-V в списке нет, то его надо будет установить. Смотри следующий пункт). Если галочка не стоит, то поставьте ее и нажмите кнопку ОК.
![image](https://github.com/user-attachments/assets/d298a891-64f9-40b8-bbdf-1b47e7fae4d5)

## Этап 2. Устанавливаем Hyper-V, если он не установлен (не был найден на предыдущем шаге).

#### Шаг 1. Запустите PowerShell или сеанс CMD от имени администратора.
Введите в строке поиска "Powershell".
В списке найденных приложений нажмите правой кнопкой мэши на "Windows PowerShell".
Выберите пункт "Запуск от имени администратора".


