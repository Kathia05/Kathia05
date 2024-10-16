import tkinter as tk

ventana = tk.Tk()
ventana.title = "Primer formulario"
ventana.geometry("300x200")

def datos():
    print("Apellido Paterno: ", apepat.get())
    print("Nombre: ", nombre.get())
    print("Apellido Materno ", apemat.get())
    print("Edad: ", edad.get())
    print("Correcto: ", correo.get())

tk.Label(ventana, text= "☻Nombre: ").grid(row = 0, column = 0)
nombre = tk.Entry(ventana)
nombre.grid(row = 0, column = 1)
tk.Label(ventana, text= "Apellido Paterno: ").grid(row = 1, column = 0)
apepat = tk.Entry(ventana)
apepat.grid(row = 1, column = 1)
tk.Label(ventana, text= "Apellido Materno: ").grid(row = 2, column = 0)
apemat = tk.Entry(ventana)
apemat.grid(row = 2, column = 1)
tk.Label(ventana, text= "Edad: ").grid(row = 3, column = 0)
edad = tk.Entry(ventana)
edad.grid(row = 3, column = 1)
tk.Label(ventana, text= "Correo: ").grid(row = 4, column = 0)
correo = tk.Entry(ventana)
correo.grid(row = 4, column = 1)

boton_aceptar = tk.Button(ventana, text = "Aceptar", command= datos)
boton_aceptar.grid(row = 5, column = 1, columnspan= 2)
boton_cancelar = tk.Button(ventana, text = "Cancelar")
boton_cancelar.grid(row = 5, column = 0, columnspan= 2)

ventana.mainloop()
