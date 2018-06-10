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

#------------------------------------Titulo-----------------------------------------------------------------------
Titulo = Label(Tops, font = ('arial',40, 'bold'),text= "Cotizador de eventos", fg = "goldenrod", bd=10, anchor='w')
Titulo.grid(row=0, column=0)

#---------------------------------------Menu 1 --------------------------------------------------------------------
menu1= Label(Tops, font=('arial',25,'bold'), text = "Menu 1:", bd=12, anchor = 'w', justify='left')
menu1.grid(row=1, column=0)
menu11= Label(Tops, font=('arial',12,'bold'), text = "- Barra de Ensaladas", bd=12, anchor = 'w', justify= 'left')
menu11.grid(row=2, column=0)
menu12= Label(Tops, font=('arial',12,'bold'), text = "- Ravioles", bd=12, anchor = 'w', justify= 'left')
menu12.grid(row=3, column=0)
menu13= Label(Tops, font=('arial',12,'bold'), text = "- Frejoles", bd=12, anchor = 'w', justify= 'left')
menu13.grid(row=4, column=0)
menu14= Label(Tops, font=('arial',12,'bold'), text = "- Barra de frutas", bd=12, anchor = 'w', justify= 'left')
menu14.grid(row=5, column=0)
menu15= Label(Tops, font=('arial',12,'bold'), text = "- Zapallo con verduras", bd=12, anchor = 'w', justify= 'left')
menu15.grid(row=6, column=0)
menu16= Label(Tops, font=('arial',12,'bold'), text = "- Barra de postres", bd=12, anchor = 'w', justify= 'left')
menu16.grid(row=7, column=0)

#---------------------------------------Menu 2 --------------------------------------------------------------------
menu2= Label(Tops, font=('arial',25,'bold'), text = "Menu 2:", bd=12, anchor = 'w', justify='left')
menu2.grid(row=1, column=1)
menu21= Label(Tops, font=('arial',12,'bold'), text = "- Estofado", bd=12, anchor = 'w', justify= 'left')
menu21.grid(row=2, column=1)
menu22= Label(Tops, font=('arial',12,'bold'), text = "- Ravioles", bd=12, anchor = 'w', justify= 'left')
menu22.grid(row=3, column=1)
menu23= Label(Tops, font=('arial',12,'bold'), text = "- Asado", bd=12, anchor = 'w', justify= 'left')
menu23.grid(row=4, column=1)
menu24= Label(Tops, font=('arial',12,'bold'), text = "- Chancho", bd=12, anchor = 'w', justify= 'left')
menu24.grid(row=5, column=1)
menu25= Label(Tops, font=('arial',12,'bold'), text = "- Sopa de verduras", bd=12, anchor = 'w', justify= 'left')
menu25.grid(row=6, column=1)
menu26= Label(Tops, font=('arial',12,'bold'), text = "- Barra de postres", bd=12, anchor = 'w', justify= 'left')
menu26.grid(row=7, column=1)

#---------------------------------------Menu 3 --------------------------------------------------------------------
menu3= Label(Tops, font=('arial',25,'bold'), text = "Menu 3:", bd=12, anchor = 'w', justify='left')
menu3.grid(row=1, column=2)
menu31= Label(Tops, font=('arial',12,'bold'), text = "- Lomo saltado", bd=12, anchor = 'w', justify= 'left')
menu31.grid(row=2, column=2)
menu32= Label(Tops, font=('arial',12,'bold'), text = "- Arroz chaufa", bd=12, anchor = 'w', justify= 'left')
menu32.grid(row=3, column=2)
menu33= Label(Tops, font=('arial',12,'bold'), text = "- Arroz con mariscos", bd=12, anchor = 'w', justify= 'left')
menu33.grid(row=4, column=2)
menu34= Label(Tops, font=('arial',12,'bold'), text = "- Anticuchos", bd=12, anchor = 'w', justify= 'left')
menu34.grid(row=5, column=2)
menu35= Label(Tops, font=('arial',12,'bold'), text = "- Menestron", bd=12, anchor = 'w', justify= 'left')
menu35.grid(row=6, column=2)
menu36= Label(Tops, font=('arial',12,'bold'), text = "- Barra de postres", bd=12, anchor = 'w', justify= 'left')
menu36.grid(row=7, column=2)


#----------------------------------Nombre del Cliente---------------------------------------------------------------
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
