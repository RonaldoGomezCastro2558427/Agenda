# ⮘Dia 28/08/22⮚

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
    
    For c = 1 To 3
        pregunta = InputBox("Desea aportar para la recolecta (si o no")
        If pregunta = "si" Then
            abono = abono + 1
            dinero_rec = Int(InputBox("que cantidad va a aportar?"))
            recaudo_total = recaudo_total + dinero_rec
            If dinero_rec >= 10000 Then
                cant = cant + 1
            End If
        Else
            no_abono = no_abono + 1
        End If
    Next c
    
    prom = recaudo_total / abono
    MsgBox "El total de recaudado por los estudiantes es: " & recaudo_total
    MsgBox "El promedio recaudado por estudiante es: " & prom
    MsgBox "El numero de estudiantes que aportaron es: " & "(" & abono & ")" & " Estudiantes"
    MsgBox "El numero de estudiantes que no aportaron es: " & "(" & no_abono & ")" & " Estudiantes"
    MsgBox "Los estudiantes que aportaron una cantidad superior a $10.000: " & "(" & cant & ")" & " Estudiantes"
        
End Sub
``` 
