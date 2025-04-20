### **1. Назначение**

Файл `.gitignore` исключает из отслеживания:

- 🗄️ Служебные файлы (например, `.DS_Store`, `.idea/`)

- 🛠️ Артефакты сборки (`node_modules/`, `*.log`)

- 🔒 Конфиденциальные данные (ключи, пароли)


### **2. Примеры**

#### **Синтаксис .gitignore**
```plaintext
# Игнорировать все файлы .log  
*.log  

# Исключить папку сборки  
/build/  

# Но включить конкретный файл  
!build/important.config  
```
#### **Глобальный .gitignore**
```bash
# Создать глобальный ignore-файл  
git config --global core.excludesfile ~/.gitignore_global  
```
### **3. Важно**

- ❗ Уже добавленные в Git файлы нужно удалять вручную:

```bash
git rm --cached file.txt  
```

- 🔄 Шаблоны для языков: [github/gitignore](https://github.com/github/gitignore).