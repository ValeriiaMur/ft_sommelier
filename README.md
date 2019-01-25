# ft_sommelier

# Jupyter Notebook
Создаем директорию 

```
/tmp/"_docker"
```

В домашней директории запускаем:
ln -s "/tmp/"$USER""_docker/"" .docker
cp -R ~/.docker "/tmp/"$USER""_docker/""
rm -rf ~/.docker
ln -s "/tmp/"$USER""_docker/"" .docker
Скачиваем resources
Вводим команду для создания образа
docker build -t ft_sommelier .
Создаем папку, в которую будут сохраняться файлы, созданные через Jupyter Notebook
Запускаем образ, указав папку, где будут сохраняться файлы
docker run -it -p 8888:8888 -v <директория>:/notebooks ft_sommelier
переходим localhost:8888/?token=...
