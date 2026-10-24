# rabotki
s = input("Введите строку: ")

print(f"Длина строки: {len(s)}")
print(f"Верхний регистр: {s.upper()}")
print(f"Нижний регистр: {s.lower()}")

if len(s) > 0:
    print(f"Первый символ: {s[0]}")
    print(f"Последний символ: {s[-1]}")
else:
    print("строка пуста")
    print("строка пуста")

print(f"Перевёрнутая строка: {s[::-1]}")

ls = s.split()
print(f"Количество слов: {len(ls)}")

if 'а' in s.lower():
    s_izm = s.replace('а', '*').replace('А', '*')
    print(f"Замена 'а' на '*': {s_izm}")
else:
    print("Буква 'а' не найдена в строке.")

polindrom = s.replace(" ", "").lower()

if polindrom == polindrom[::-1]:
    print("Строка является палиндромом!")
else:
    print("Строка не является палиндромом.")
