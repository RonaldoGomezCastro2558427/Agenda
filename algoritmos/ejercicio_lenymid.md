# Ejercicio con Len y Mid 02/09/2022

Ejercicio con Len y Mid

``` 
Sub nombres()
    For x = 2 To 21
        nombre = Nom.Cells(x, 1)
        ulti = Len(nombre) - 1
        Nom.Cells(x, 2) = Mid(nombre, ulti, 2)
    Next x
End Sub
 ``` 
# Ejercicio #2

``` 
Sub nombres()
    For x = 2 To 21
    nombre = Nom.Cells(x, 1)
    año = Nom.Cells(x, 2)
    municipio = Nom.Cells(x, 3)
    ulti = Len(municipio) - 1
    Nom.Cells(x, 4) = Mid(año, 1, 2) & Mid(municipio, ulti, 2) & Mid(nombre, 1, 2)
    Next x
End Sub
```