# Registro de autos 29/08/2022

Crear un progrma en visual basic, que permita al trabajador registrar datos ingresados por el cliente y mostrarlos en otra hoja.

~~~

Sub almacenar()
    fila = datos.Cells(1, 7)
    datos.Cells(fila, 1) = formulario.Cells(7, 4)
    datos.Cells(fila, 2) = formulario.Cells(9, 4)
    datos.Cells(fila, 3) = formulario.Cells(11, 4)
    datos.Cells(fila, 4) = formulario.Cells(13, 4)
    MsgBox ("los datos se guardaron correctamente")
    datos.Cells(1, 7) = fila + 1
End Sub

Registro


Sub sena()
    For x = 1 To 15
    Z = InputBox(" ingrese un nombre")
    fila = Hoja1.Cells(1, 7)
    Hoja1.Cells(fila, 2) = Z
    Hoja1.Cells(1, 7) = fila + 1
    Next x
End Sub

~~~
 
  