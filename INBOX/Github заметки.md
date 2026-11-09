Здесь хранятся команды для Git которые помогают работу с некоторыми элементами 




# 1. Разрешить длинные пути в Windows (делается 1 раз для всей системы)
git config --global core.longpaths true

# 2. Отключить предупреждения о переносах строк (только для текущей папки Obsidian)
git config --local core.autocrlf false
git config --local core.safecrlf false

# 3. Если коммит "сломался" и выдал ошибку, отменяем его (твои файлы на диске НЕ удалятся!)
git reset HEAD~1

# 4. Добавляем все файлы заново и создаём чистый коммит
git add .
git commit -m "fix: normalize line endings and long paths"