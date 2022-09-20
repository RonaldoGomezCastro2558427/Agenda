# Recaudación para evento estudiantil con while ⮘Dia 31/08/22⮚

En una entidad educativa con 7500 estudiantes se requiere realizar una recolecta para sufragar los gastos de un evento organizado por el colegio.

Se necesita que el programa entregue la siguiente información. 
1) El total recaudado por los estudiantes del colegio
2) Valor del recaudo promedio para los estudiantes que aportaron dinero 
3) Número de estudiantes que aportaron en la recolecta
4) Número de estudiantes que no aportaron a la recolecta
5) cantidad de estudiantes que aportaron una cantidad mayor a $10.000

``` 
Sub inicio()
    
    abono = 0
    no_abono = 0
    cant = 0
    recaudo_total = 0
    c = 0
    cant10k = 0
    
    c = InputBox("¿Cuanto va aportar para la recolecta?")
    
    While c >= 3000000
        abono = abono + c
        cant = cant + 1
            If c < 10000 Then
              cant10k = cant10k + 1
            Else
              no_abono = no_abono + 1
            End If
    Wend
    
    prom = 3000000 / cant
    MsgBox "El promedio recaudado por estudiante es: " & prom
    MsgBox "El numero de estudiantes que aportaron es: " & "(" & cant & ")" 
    MsgBox "El numero de estudiantes que no aportaron es: " & "(" & no_abono & ")"  
    MsgBox "Los estudiantes que aportaron una cantidad superior a $10.000: " & "(" & cant10k & ")" 
        
End Sub
```