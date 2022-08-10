# Украшаем систему после установки

## Характеристики
- DE: KDE Plasma: **5.24.6**
- KDE Frameworks: **5.96.0**
- Версия Qt: **5.15.5**
- Systems: Arch/Arch-based distributives


### Установка latte dock:

[Официальный репозиторий](https://github.com/KDE/latte-dock)

*Прежде чем устанавливать первым способом, вам необходимо поставить необходимые зависимости:*
- first step: `sudo pacman -Syu`
- next step: `sudo pacman -S cmake extra-cmake-modules python plasma-framework plasma-desktop plasma-wayland-protocols`

- Способ 1 - Установка и сборка из официального Git репозитория:
- first step: `git clone https://github.com/KDE/latte-dock`
- next step: `cd latte-dock/`
- next step: `sh install.sh`

- Способ 2 - Установка с помощью **pacman**:
`sudo pacman -S latte-dock`

- Способ 3 - Установка с помощью **yay**:
`yay -Sy latte-dock` or `yay latte-dock`

-----------------------------------------------------------------------------------------------------------

# Установка плазмидов в систему:

*Можно установить с помощью графического установщика или через терминал с помощью **yay***

- *Вывести список доступных плазмидов на экран:*
`yay plasma5-applets`


- *Или установить каждый отдельно, или только тот что необходим:*

- Установить latte-sidebar-button:
`yay -S plasma5-applets-latte-sidebar-button`

- Установить uswitch:
`yay -S plasma5-applets-uswitch`

- Установить latte-spacer:
`yay -S plasma5-applets-latte-spacer`

- Установить latte-separator:
`yay -S plasma5-applets-latte-separator`

- Установить kde-arch-update-notifier:
`yay -S plasma5-applets-kde-arch-update-notifier`

- Установить window-title:
`yay -S plasma5-applets-window-title`

- Установить docker:
`yay -S plasma5-applets-docker`

- Установить window-appmenu:
`yay -S plasma5-applets-window-appmenu`

- Установить panon:
`yay -S plasma5-applets-panon`

- Установить window-control:
`yay -S plasma5-applets-active-window-control`

-----------------------------------------------------------------------------------------------------------


# Настройка терминала:

*Переход на **zsh** и использование **ohmyzsh** + установка специальной темы **powerlevel10k** *

ArchWiki: [zsh](https://wiki.archlinux.org/title/Zsh_(%D0%A0%D1%83%D1%81%D1%81%D0%BA%D0%B8%D0%B9))
OhMyZsh: [ohmyzsh](https://ohmyz.sh/)
powerlevel10k: [powerlevel10k](https://github.com/romkatv/powerlevel10k)

- Установка **zsh**
`sudo pacman -Syu zsh`

- Установка **OhMyZSH**:

|Метод|Комманда|
| ----------- | ----------- |
|curl|`sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`|
|wget|`sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`|
|fetch|`sh -c "$(fetch -o - https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`|

*Больше информации по настроке, можно найти на официальной странице [Github](https://github.com/ohmyzsh/ohmyzsh) проекта*

---------------

## Если возможностей ohmyzsh показалось мало, то ставим тему powerlevel10k

*Установка*
- `yay -S --noconfirm zsh-theme-powerlevel10k-git`
- `echo 'source /usr/share/zsh-theme-powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc`

*Далее для детальной настройки и конфигурации можно посетить [страницу проекта](https://github.com/romkatv/powerlevel10k#configuration)*

----------------------------------------------------------------------------------------------------------

# Украшаем систему, ставим иконки


# Papirus
![papirus icon collection](https://raw.githubusercontent.com/PapirusDevelopmentTeam/papirus-icon-theme/master/preview.png)
### [**Papirus**](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme/)

## Установка набора иконок:
*Клонируем репозиторий с иконками*
- `git clone https://github.com/PapirusDevelopmentTeam/papirus-icon-theme.git`
*переходим в папку с иконками*
- `cd papirus-icon-theme`
*устанавливаем иконки*
- `./install.sh` or `sh install.sh`

### 2 способ установки:
`sudo pacman -S papirus-icon-theme` community

### 3 способ установки:
*Используйте сценарии для установки последней версии непосредственно из этого репозитория (независимо от вашего дистрибутива)*

- Корневой каталог (рекомендуется)
`wget -qO- https://git.io/papirus-icon-theme-install | sh`

- Домашний каталог для GTK
`wget -qO- https://git.io/papirus-icon-theme-install | DESTDIR="$HOME/.icons" sh`

- Домашний каталог для KDE
`wget -qO- https://git.io/papirus-icon-theme-install | DESTDIR="$HOME/.local/share/icons" sh`

- Удаление
`wget -qO- https://git.io/papirus-icon-theme-uninstall | sh`

----------------------------------------------------------------------------------------------------------

# Flatery
![Flatery icons](https://raw.githubusercontent.com/cbrnix/Flatery/master/cover.png)
**[Flatery]**(https://github.com/cbrnix/Flatery)

## Установка набора иконок
*Клонируем репозиторий с иконками*
- `git clone https://github.com/cbrnix/Flatery.git`
*переходим в папку с иконками*
- `cd Flatery`
*примечание! у этого набора есть опции, чтобы посмотреть их нужно вызвать справку по устаноке, командой:*
- `./install.sh -h` or `sh install.sh -h`
*устанавливаем иконки*
- `./install.sh` or `sh install.sh`



# Qogir icon theme
### black
![Qogir icon theme black](https://raw.githubusercontent.com/vinceliuice/Qogir-icon-theme/master/preview_01.png)
### white
![Qogir icon theme white](https://raw.githubusercontent.com/vinceliuice/Qogir-icon-theme/master/preview_02.png)
**[Qogir]**(https://github.com/vinceliuice/Qogir-icon-theme)

## Установка набора иконок
*Клонируем репозиторий с иконками*
- `git clone https://github.com/vinceliuice/Qogir-icon-theme`
*переходим в папку с иконками*
- `cd Qogir-icon-theme`
*примечание! у этого набора есть опции, чтобы посмотреть их нужно вызвать справку по устаноке, командой:*
- `./install.sh -h` or `sh install.sh -h`
*устанавливаем иконки*
- использование: `./install.sh [OPTIONS...]`
**OPTIONS:**
  |-d, --dest DIR|Specify theme destination directory (Default: /home/romildo/.local/share/icons)|
  |-n, --name NAME|Specify theme name (Default: Qogir)|
  |-t, --theme VARIANT|Specify theme primary color variant(s) [default|manjaro|ubuntu|all] (Default: all themes)|
  |-c, --color VARIANT|Specify theme color variant(s) [standard|dark|all] (Default: all variants)|
  |-h, --help|Show this help|



# Tela-icon
![Tela-icon](https://images.pling.com/img/00/00/32/24/44/1279924/6b664cbc418fd3837179d322d63db97c8b84.png)
**[Tela-icon]**(https://github.com/vinceliuice/Tela-icon-theme)

## Установка набора иконок
*Клонируем репозиторий с иконками*
- `git clone https://github.com/vinceliuice/Tela-icon-theme.git`
*переходим в папку с иконками*
- `cd Tela-icon-theme`
*примечание! у этого набора есть опции, чтобы посмотреть их нужно вызвать справку по устаноке, командой:*
- `./install.sh -h` or `sh install.sh -h`
*устанавливаем иконки*
- `./install.sh -a` or `sh install.sh -a` -all color version



# Tela-circle
![Tela-circle](https://github.com/vinceliuice/Tela-circle-icon-theme/blob/master/preview.png)
**[Tela-circle]**(https://github.com/vinceliuice/Tela-circle-icon-theme)

## Установка набора иконок
*Клонируем репозиторий с иконками*
- `git clone https://github.com/vinceliuice/Tela-circle-icon-theme.git`
*переходим в папку с иконками*
- `cd Tela-circle-icon-theme`
*примечание! у этого набора есть опции, чтобы посмотреть их нужно вызвать справку по устаноке, командой:*
- `./install.sh -h` or `sh install.sh -h`
*устанавливаем иконки*
- `./install.sh -a` or `sh install.sh -a` -all color version



# Colloid icons
![Colloid icons](https://raw.githubusercontent.com/vinceliuice/Colloid-icon-theme/main/preview.png)
**[Colloid icons]**(https://github.com/vinceliuice/Colloid-icon-theme)

## Установка набора иконок
*Клонируем репозиторий с иконками*
- `git clone https://github.com/vinceliuice/Colloid-icon-theme.git`
*переходим в папку с иконками*
- `cd Colloid-icon-theme`
*примечание! у этого набора есть опции, чтобы посмотреть их нужно вызвать справку по устаноке, командой:*
- `./install.sh -h` or `sh install.sh -h`
*устанавливаем иконки*
- `./install.sh -t all` or `sh install.sh -t all` -all color version


----------------------------------------------------------------------------------------------------------

# Украшаем систему, ставим темы оформления

*Прежде чем устанавливать темы оформления, необходимо установить **Kvantum** движок тем*

### Kvantum

Страница проекта на [Gitgub](https://github.com/tsujan/Kvantum/tree/master/Kvantum)
Больше информации можно найти на странице в [git](https://github.com/tsujan/Kvantum/blob/master/Kvantum/INSTALL.md#arch-based-distributions)

- Установка в Arch-based дистрибутивах:
`sudo pacman -S kvantum-qt5`
------ или ------
`yay -S kvantum-qt5-git`

*Примечение! так же, Kvantum можно собрать из исходников*
Больше инструкций по сборке из исходников можете найти [здесь](https://github.com/tsujan/Kvantum/blob/master/Kvantum/INSTALL.md#installation)


# Темы

## Arc-kde
![Arc-kde](https://raw.githubusercontent.com/PapirusDevelopmentTeam/arc-kde/master/preview.png)
<p align="center">
  <img src="https://raw.githubusercontent.com/PapirusDevelopmentTeam/arc-kde/master/preview.png" alt="Preview Arc-Dark KDE"/>
  <sup><sub>Screenshot Details: Engine: <a href="https://github.com/tsujan/Kvantum/tree/master/Kvantum">Kavntum</a> | Kvantum Theme: Arc Dark | Aurorae decoration: Arc Dark | Plasma Theme: Arc Dark | Icons: <a href="https://github.com/PapirusDevelopmentTeam/papirus-icon-theme">Papirus</a></sub></sup>
</p>
[Arc-kde](https://github.com/PapirusDevelopmentTeam/arc-kde)

- Установка:
`wget -qO- https://raw.githubusercontent.com/PapirusDevelopmentTeam/arc-kde/master/install.sh | sh`
- Удаление:
`wget -qO- https://raw.githubusercontent.com/PapirusDevelopmentTeam/arc-kde/master/install.sh | env uninstall=true sh`

-- Второй способ установки --
*Клонируем репозиторий:*
`git clone https://github.com/PapirusDevelopmentTeam/arc-kde.git`
*Переходим в папку с темой:*
`cd arc-kde`
*Устанавливаем тему:*
`./install.sh` or `sh install.sh`

- Лучше всего использовать эту тему с иконками [Papirus](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme)

*Примечание! Если не получается установить, то пробуем с командой `sudo`*



## Canta
![Canta dark](https://raw.githubusercontent.com/vinceliuice/Canta-kde/master/canta-dark.png)
![Canta light](https://raw.githubusercontent.com/vinceliuice/Canta-kde/master/canta-light.png)
[Canta](https://github.com/vinceliuice/Canta-kde)

### Установка:
*Клонируем репозиторий:*
`git clone https://github.com/vinceliuice/Canta-kde.git`
*Переходим в папку с темой:*
`cd Canta-kde`
*Устанавливаем тему:*
`./install.sh` or `sh install.sh`



## Cherry
![Cherry](https://raw.githubusercontent.com/nullxception/cherry-kde-theme/main/preview-full.png)
[Cherry](https://github.com/nullxception/cherry-kde-theme)

### Установка
*Клонируем репозиторий:*
`git clone https://github.com/nullxception/cherry-kde-theme.git`
*Переходим в папку с темой:*
`cd cherry-kde-theme`
*Устанавливаем тему:*
`./install.sh` or `sh install.sh`
*Удаляем тему:*
`./uninstall.sh` or `sh uninstall.sh`



## Colloid
![Colloid dark](https://github.com/vinceliuice/Colloid-kde/blob/main/Screenshot_dark.png)
![Colloid light](https://github.com/vinceliuice/Colloid-kde/blob/main/Screenshot_light.png)
[Colloid kde](https://github.com/vinceliuice/Colloid-kde)
*Примечание отлично сочитается с иконками [Colloid](https://github.com/vinceliuice/Colloid-icon-theme)*

### Установка
*Клонируем репозиторий:*
`git clone https://github.com/vinceliuice/Colloid-kde.git`
*Переходим в папку с темой:*
`cd Colloid-kde`
*Устанавливаем тему:*
`./install.sh` or `sh install.sh`



## Lace
![Lace](https://raw.githubusercontent.com/yeyushengfan258/Lace-kde/main/View-1.png)
[Lace kde](https://github.com/yeyushengfan258/Lace-kde)

### Установка
*Клонируем репозиторий:*
`git clone https://github.com/yeyushengfan258/Lace-kde.git`
*Переходим в папку с темой:*
`cd Lace-kde`
*Устанавливаем тему:*
`./install.sh` or `sh install.sh`

В проекте есть тема для sddm, но устанавливать её нужно отдельно:
*находясь в папке **Lace-kde** перейдите в папку sddm командой:*
`cd sddm/`
*Установите тему для экрана загрузки, командой:*
`./install.sh` or `sh install.sh` - если надо, то запустите скрипт с помощью *sudo*



## Nephrite
![Nephrite](https://github.com/vinceliuice/Nephrite-kde/blob/main/Screenshot_light.png)
[Nephrite](https://github.com/vinceliuice/Nephrite-kde)

### Установка
*Клонируем репозиторий:*
`git clone https://github.com/vinceliuice/Nephrite-kde.git`
*Переходим в папку с темой:*
`cd Nephrite-kde`
*Устанавливаем тему:*
`./install.sh` or `sh install.sh`

В проекте есть тема для sddm, но устанавливать её нужно отдельно:
*находясь в папке **Nephrite-kde** перейдите в папку sddm командой:*
`cd sddm/`
*Установите тему для экрана загрузки, командой:*
`./install.sh` or `sh install.sh` - если надо, то запустите скрипт с помощью *sudo*



## Orchis
![Orchis](https://github.com/vinceliuice/Orchis-kde/blob/main/plasma/look-and-feel/com.github.vinceliuice.Orchis/contents/previews/fullscreenpreview.jpg)
[Orchis](https://github.com/vinceliuice/Orchis-kde)

### Установка
*Клонируем репозиторий:*
`git clone https://github.com/vinceliuice/Orchis-kde.git`
*Переходим в папку с темой:*
`cd Orchis-kde`
*Устанавливаем тему:*
`./install.sh` or `sh install.sh`

В проекте есть тема для sddm, но устанавливать её нужно отдельно:
*находясь в папке **Orchis-kde** перейдите в папку sddm командой:*
`cd sddm/`
*Установите тему для экрана загрузки, командой:*
`./install.sh` or `sh install.sh` - если надо, то запустите скрипт с помощью *sudo*



## Qogir
![Qogir](https://raw.githubusercontent.com/vinceliuice/Qogir-kde/master/images/preview1.png)
[Qogir](https://github.com/vinceliuice/Qogir-kde)
*Примечание! идеально гармонирует с набором иконок [qogir](https://github.com/vinceliuice/Qogir-icon-theme)*

### Установка
*Клонируем репозиторий:*
`git clone https://github.com/vinceliuice/Qogir-kde.git`
*Переходим в папку с темой:*
`cd Qogir-kde`
*Устанавливаем тему:*
`./install.sh` or `sh install.sh`
*Удаляем тему:*
`./uninstall.sh` or `sh uninstall.sh`

В проекте есть тема для sddm, но устанавливать её нужно отдельно:
*находясь в папке **Qogir-kde** перейдите в папку sddm командой:*
`cd sddm/`
*Установите тему для экрана загрузки, командой:*
`./install.sh` or `sh install.sh` - если надо, то запустите скрипт с помощью *sudo*



## Otto
![Otto](https://user-content.gitlab-static.net/a6ed93e55643d26282a6bab6574b9fc6fef550ba/68747470733a2f2f692e696d6775722e636f6d2f5655374b4d41722e706e67)
[Otto](https://gitlab.com/jomada/otto)
*Примечание! идеально гармонирует с набором иконок [qogir](https://github.com/vinceliuice/Qogir-icon-theme)*

### Установка
*Клонируем репозиторий:*
`git clone https://gitlab.com/jomada/otto.git`
*Переходим в папку с темой:*
`cd otto`
*Устанавливаем тему:*
`./install.sh` or `sh install.sh`
