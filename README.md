# andrea.lomniczi
from Tkinter import *
ventana=Tk()
ventana.geometry("1600x800+0+0")
ventana.title("Cotizador de eventos")
text_Input = StringVar()

Tops = Frame(ventana, width = 1600,height = 50,bg="Powder blue", relief=SUNKEN)
lblInfo = Label(Tops, font = ('arial',40, 'bold'),text= "Restaurant Management System", fg = "Steel Blue", bd=10, anchor='w')
lblInfo.grid(row=0, column=0)
# row 1 : the name
nombre_label = Label(text="Nombre :")
nombre_label.grid(row=3,column=3)
nombre_str = StringVar()
nombre_entry = Entry(textvariable=nombre_str)
nombre_entry.grid(row=3,column=4)
#row 2 : the last name
last_label= Label(text="Apellido : ")
last_label.grid(row=4,column=3)
last_str = StringVar()
last_entry = Entry(textvariable=last_str)
last_entry.grid(row=4,column=4)
#row 3 : the email
mail_label = Label(text="Email : ")
mail_label.grid(row=5,column=3)
mail_str = StringVar()
mail_entry = Entry(textvariable=mail_str)
mail_entry.grid(row=5,column=4)
#cosas
def Ref():
    CdI = float(Invitados.get())
    CdT = float(Toldo.get())
    MdT=float(MToldo.get())
    CdB = float(Buffet.get())
    CdM =float(Mozos.get())
    CdL = float(Local.get())
    CdB = float(Bebidas.get())

    CostoDeToldo = CdT * 300
    CostodeBebidas = CdI * 4.50
  

#row 4 : end
finish = Button(text="finalizar",relief=FLAT)
finish.grid(row=4,column=2)
ventana.mainloop()
