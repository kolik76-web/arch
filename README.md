                 ##############################################
                              
                         **ArchLinux Fast Install v2.4.0**
                         
                  ##############################################
                          
**Описание**

Этот скрипт не задумывался, как обычный установочный с большим выбором DE, разметкой диска и т.д. И он не предназначен для новичков. Он предназначен для тех, кто ставил ArchLinux руками и понимает, что и для чего нужна каждая команда.

Его цель - это моментальное разворачиванеи системы со всеми конфигами. Смысл в том что, все изменения вы делаете предварительно в самом скрипте и получаете возможность быстрой установки ArchLinux с вашими личными настройками (при условии, что вы его изменили под себя, в противном случае с моими настройками).

Cкрипт основан на моем чек листе ручной установке ArchLinux https://vk.cc/7JTg6U Этот скрипт работает с UEFI. Для работы с Legasy/BIOS используйте предыдущий скрипт https://github.com/ordanax/arch2018

Cостоит из 3 частей.

1-й и 2-й - это базовая установка Arch Linux c XFCE/i3wm

3-й - мой конфиг системы. Подключение AUR, кастомизация XFCE/i3wm, установка нужных программ, авто вход и т.д.

**Установка**

Скачать и записать на флешку ISO образ Arch Linux https://www.archlinux.org/download/

Скачать и запустить скрипт командой:

```
pacman -Syy
pacman -S wget
wget git.io/archuefi_1.sh && sh archuefi_1.sh
```
или просто

```
curl -OL git.io/archuefi_1.sh && sh archuefi_1.sh
```
Запустится установка минимальной системы. 2-я часть ставится автоматически и это базовая установка ArchLinux без программ.

3-я часть не обязательная. Она устанавливает программы, AUR (yay), мои конфиги XFCE/i3wm. Предварительно установите wget командой:

```
sudo pacman -S wget
```
Установка 3-й части производится из терминала командой:

```
wget git.io/archuefi_3.sh && sh archuefi_3.sh
```
