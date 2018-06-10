from Tkinter import *
import random

ventana = Tk()
ventana.geometry("1600x800+0+0")
ventana.title("Cotizador de eventos")

text_Input = StringVar()
operator = ""

Tops = Frame(ventana, width = 1600,height = 50,bg="gold", relief=RIDGE)
Tops.pack(side=TOP)

F1 = Frame(ventana, width = 800,height = 700, relief=RIDGE)
F1.pack(side=LEFT)

F2 = Frame(ventana, width = 300,height = 700, relief=RIDGE)
F2.pack(side=RIGHT)


lblInfo = Label(Tops, font = ('arial',40, 'bold'),text= "Cotizador de eventos", fg = "goldenrod", bd=10, anchor='w')
lblInfo.grid(row=0, column=0)

#----------------------------------Nombre del Cliente------------------------------------
Nombre = Label(F1, font=('arial',12,'bold'), text = "Nombre", bd=12, anchor = 'w')
Nombre.grid(row=0, column=0)
txtNombre=Entry(F1, font=('arial',12,'bold'), textvariable=Nombre, bd=6, insertwidth=4,
                               bg = "snow2", justify = 'left')
txtNombre.grid(row=0, column=1)

#----------------------------------Apellido del Cliente------------------------------------
Apellido = Label(F1, font=('arial',12,'bold'), text = "Apellido", bd=12, anchor = 'w')
Apellido.grid(row=1, column=0)
txtApellido=Entry(F1, font=('arial',12,'bold'), textvariable=Apellido, bd=6, insertwidth=4,
                               bg = "snow2", justify = 'left')
txtApellido.grid(row=1, column=1)

#----------------------------------Email del Cliente------------------------------------
Email = Label(F1, font=('arial',12,'bold'), text = "Email", bd=12, anchor = 'w')
Email.grid(row=2, column=0)
txtEmail=Entry(F1, font=('arial',12,'bold'), textvariable=Email, bd=6, insertwidth=4,
                               bg = "snow2", justify = 'left')
txtEmail.grid(row=2, column=1)

#----------------------------------Numero de contacto del Cliente------------------------------------
Telefono = Label(F1, font=('arial',12,'bold'), text = "Telefono", bd=12, anchor = 'w')
Telefono.grid(row=3, column=0)
txtTelefono=Entry(F1, font=('arial',12,'bold'), textvariable=Telefono, bd=6, insertwidth=4,
                               bg = "snow2", justify = 'left')
txtTelefono.grid(row=3, column=1)







ventana.mainloop()
