**from tkinter import *


class animal:
    def __init__(self, pet_name, animal_type, virus, birthday, date_operacia):
        self.pet_name = pet_name
        self.birthday = birthday
        self.animal_type = animal_type
        self.virus = virus
        self.date_operacia = date_operacia


pets = []


def pets_info(self):
    label = Label(
        text=f"pet_name-{self.pet_name}, animal_type-{self.animal_type}, animal_virus-{self.virus}, birthday-{self.birthday}, animal_date_operacia-{self.date_operacia}")
    label.pack()


def pet_list():
    root = Tk()
    root.geometry("300x300")
    btn3 = Button(text=-pets, command=pets_info)
    btn3.pack()
    root.mainloop()


def pet_add():
    pets.add(animal(input(), input(), input(), input(), input()))
    print(f'pet add - {pets}')


def pet_remove():
    pets.remove(animal)


root = Tk()
root.geometry("300x300")
btn = Button(root, text='pet_list', command=pet_list)
btn.pack()
btn1 = Button(root, text='pet_add')
btn1.pack()
btn2 = Button(root, text='pet_remove')
btn2.pack()
root.mainloop()
**
