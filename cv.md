# Alexey Khirny
## contact info:
- phone number:+375336913620
- Email: lioshakhirny@gmail.com
- instagram: @lioshkaaa
***
## Briefly About Myself:
I am a student of the Polytechnic College. I am studying to become a programmer, I strive to learn something new for myself. Therefore, I want to try myself starting with the courses. I am studying in the 3rd year. Занимался на курсах [html academy][1].

[1]:https://htmlacademy.ru/ "html academy" 
I hope that my diligence and courses will help me get useful knowledge.
***
## Skills:
- Delphi
- Python
- Html,css
- c#
- Git
***
## Sample code:
``` Python: 
class Phones:
    dictionary = {}

    def __init__(self, number):
        self.number = number

    def info(self):
        print(' телефон:', self.number, end='')

    def print_phones(self):
        for a in self.dictionary:
            print('Фамилия: ', a, ', телефон: ', self.dictionary[a])

    def find(self, family):
        if family in self.dictionary:
            print('Запись найдена!!!')
            print('Фамилия ', family, ', телефон:', self.dictionary[family])
        else:
            print('Такой фамилии в справочнике не существует')


class Person(Phones):
    def __init__(self, family, adress, number):
        self.family = family
        self.adress = adress
        self.number = number
        Phones.dictionary[self.family] = self.number

    def info(self):
        print('Фамилия - ', self.family, ', адрес: ', self.adress, end='')
        Phones.info(self)
        print()


class Organization(Phones):
    organization_dict = dict()
    def __init__(self, name, adress, number, phaks, kont_face):
        self.name = name
        self.adress = adress
        self.number = number
        self.phaks = phaks
        self.kont_face = kont_face
        self.organization_dict[self.name] = self.number

    def info(self):
        print('Организация - ', self.name, ', адрес: ', self.adress, ', факс: ', self.phaks, ', контактное лицо:',
              self.kont_face,',', end='')
        Phones.info(self)
        print()

    def find(self, name):
        if name in self.organization_dict:
            print('Запись найдена!!!')
            print('Организация: ', name , ', телефон:', self.organization_dict[name])
        else:
            print('Такой организации в справочнике не существует')


class Friend(Person):
    def __init__(self, family, adress, number, birthday):
        self.family = family
        self.adress = adress
        self.number = number
        self.birthday = birthday
        Phones.dictionary[self.family] = self.number

    def info(self):
        Person.info(self)
        print('день рождения: ', self.birthday)

p1 = Person('Иванов', 'Кабяка 37', '+3753339033')
p1.info()
p1.find('Иванов')

p2 = Person('Мельничек', 'Кремко 12', '+375332953602')
p2.info()
p2.find('Мель')

org1 = Organization('Гродножилстрой', 'Суворова 125', '+375296530212', 'f315613', 'Иванов Сергей')
org1.info()
org1.find('Гродножилстрой')

fr1 = Friend('Войтюнко', 'Каравайная 15', '+375293520135', '24.03.2004')
fr1.info()
fr1.find('Войтюнко')

print('------------Весь справочник----------')
ph1 = Phones('+1231651')
ph1.print_phones()
  ```
  ## Education:
  - Grodno State Polytechnic College
 ***
## Languages:
 - Russian - native speaker.
- English - A2

