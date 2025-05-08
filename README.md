name = input("Введіть ваше ім'я")
users = ['Віталій','Андрій','Софія','Денис','Антон']
passwords = {
    "Віталій" : "123",
    "Андрій" : "234",
    "Софія" : "234",
    "Денис" : "567",
   "Антон" : "345"
}

if name in users:
    print("Вітаю", name)
    password = input("Введіть пароль:")
    if password == passwords[name]:
        print("Пароль правильний")
    else:
        print("Пароль неправильний")
else:
    print(name," Ваше ім'я не знайдено")
    print("Ви хочете зареєструватись?")
    answer = input("Так/Ні")
    if answer == "Ні":
        print("До побачення", name)
    else:
        users.append(name)
print(users)
