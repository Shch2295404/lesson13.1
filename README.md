# **Lesson13.1 – Введение в алгоритмы и структуры данных**  

---

## 📌 **Описание проекта**  
В этом проекте реализован **алгоритм проверки строки на палиндром**.  
Алгоритм позволяет определить, читается ли строка одинаково слева направо и справа налево, **игнорируя пробелы и регистр**.  

🔹 **Ключевые аспекты алгоритма:**  
- Работа со строками (**преобразование регистра, удаление пробелов**)  
- Использование структур данных (**строка как массив символов**)  
- Оптимизированное сравнение (**разворот строки срезом `[::-1]`**)  

---

## 📚 **Алгоритм работы функции**  

**1. Приведение строки к нижнему регистру** – это позволяет сравнивать символы без учета заглавных и строчных букв.  
**2. Удаление пробелов** – они не влияют на палиндромность, поэтому удаляются.  
**3. Разворот строки** – используем срез `[::-1]`, который переворачивает строку.  
**4. Сравнение строк** – если исходная и перевернутая строки совпадают, значит, это **палиндром**.  

📌 **Сложность алгоритма**: **O(n)**, где `n` – длина строки.  
- **O(n)** – так как необходимо пройти по всей строке (нормализовать, перевернуть и сравнить).  
- Используется **минимум дополнительной памяти** – только для хранения строки.  

---

## 📂 **Структура проекта**  
```
lesson13.1/
│── main.py          # Функция проверки строки на палиндром
│── README.md        # Документация проекта
└── requirements.txt # Зависимости проекта (если нужны)
```

---

## 🚀 **Запуск программы**  

### **1. Клонирование репозитория**  
```bash
git clone https://github.com/Shch2295404/lesson13.1.git
cd lesson13.1
```

### **2. Запуск кода**  
```bash
python main.py
```

---

## 🛠 **Реализованная функция**  

### **`is_palindrome(s)`**  
📌 **Алгоритм проверки строки на палиндром**  

✅ **Пример использования:**  
```python
from main import is_palindrome

print(is_palindrome("А роза упала на лапу Азора"))  # True
print(is_palindrome("Привет"))  # False
```

---

## 🏆 **Выводы**  
🔹 **Использование строк как структур данных**  
🔹 **Алгоритм оптимизирован по времени и памяти**  
🔹 **Применение срезов `[::-1]` для реверса строк**  
🔹 **Эффективность O(n), так как необходимо пройти по строке один раз**  

---

## ⚙ **Используемые технологии**  
- **Python 3.10+**  
- **Алгоритмы работы со строками**  
- **Структуры данных: строка (как массив символов)**  
