# Node.js File Server — README
 
## Запуск сервера
 
Відкрийте термінал у директорії з файлами проєкту та виконайте команду:
 
```bash
node <назва_файлу>.js <порт>
```
 
**Приклади:**
 
```bash
node file_read.js 3000
node file_write.js 3000
```
 
---
 
## Перевірка через curl
 
### Читання даних (GET)
 
```bash
curl -i http://localhost:3000/data
```
 
### Запис даних (POST)
 
```bash
curl -X POST http://localhost:3000/data \
  -H "Content-Type: application/json" \
  -d '{"name":"Karina","age":19}'
```
