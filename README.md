# Самоконтроль выполненения задания

1. Где расположен файл с `some_fact` из второго пункта задания?  
__group_vars/all/examp.yml__
2. Какая команда нужна для запуска вашего `playbook` на окружении `test.yml`?  
__ansible-playbook site.yml -i inventory/test.yml__
3. Какой командой можно зашифровать файл?  
__ansible-vault encrypt__
4. Какой командой можно расшифровать файл?  
__ansible-vault decrypt__
5. Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?  
__если есть пароль, запустить команду `ansible-vault view %encrypted-file-name%` и ввести пароль__
6. Как выглядит команда запуска `playbook`, если переменные зашифрованы?  
__ansible-playbook -i inventory/prod.yml site.yml --ask-vault-pass__
7. Как называется модуль подключения к host на windows?  
__ansible.builtin.winrm__
8. Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh  
__ansible-doc -t connection -l__
9. Какой параметр из модуля подключения `ssh` необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?  
__remote_user__
