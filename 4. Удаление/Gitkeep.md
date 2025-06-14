### 1. Назначение

Git не отслеживает пустые папки. `.gitkeep` — это:

- 📌 Пустой файл-маркер для сохранения структуры проекта

- 🔧 Альтернатива — `.gitignore` с исключением (`!*/`)

---
### 2. Примеры

#### Создание пустой папки

```bash
mkdir logs  
touch logs/.gitkeep  # Теперь папка будет в репозитории  
```
#### Игнорирование всего, кроме .gitkeep

```plaintext
# В .gitignore папки `logs`:  
logs/*  
!logs/.gitkeep  

```
### 3. Важно

- 🔄 `.gitkeep` — неофициальное соглашение, технически подойдет любой файл.