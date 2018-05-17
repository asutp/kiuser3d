Usage:
$ kiuser3d NAME_USER_VARIABLE

This script is for user variable substitution (like KISYS3DMOD)
in user libraries KiCAD. It looks for files in the current directory
(by mask.* kicad.pretty) and in the case of a normal path in the model file name
replaces it with the path you specify when you enter it.
Example:
I described the NAME_USER_VARIABLE in kicad
   KIUSER3DMOD=/mnt/sda2/myKiLib3D
After executing this script line in the files *.kicad_mod containing:
   "(model INDUCTANCE/K20x11x6.wrl"
will look like
   "(model ${KIUSER3DMOD}/INDUCTANCE/K20x11x6.wrl"

Использование:
$ kiuser3d ИМЯ_ПОЛЬЗОВАТЕЛЬСКОЙ_ПЕРЕМЕННОЙ

Этот скрипт для подстановки пользовательской переменной (вроде KISYS3DMOD)
в пользовательские библиотеки KiCAD. Он ищет файлы в текущей директории
(по маске *.kicad.pretty) и в случае обычного пути в имени файла модели
заменяет его на указанный при вводе путь.
Например: 
Я описал ИМЯ_ПОЛЬЗОВАТЕЛЬСКОЙ_ПЕРЕМЕННОЙ в kicad
   KIUSER3DMOD=/mnt/sda2/myKiLib3D
После исполнения этого скрипта строки в файлах *.kicad_mod содержащие
   "(model INDUCTANCE/K20x11x6.wrl"
будут выглядеть как
   "(model ${KIUSER3DMOD}/INDUCTANCE/K20x11x6.wrl"
