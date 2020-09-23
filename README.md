<div align="center">

## Take a full\-screen screenshot \(capture screen\) and save it to disk


</div>

### Description

Takes a screenshot (like PrintScreen keayboard key) and saves it to a diskfile (you can also manipulate it like any other bitmap/graphic)
 
### More Info
 
Microsoft .NET Framework 2.0 or later required...


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Rodolfo Gonzalez Ruiz](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/rodolfo-gonzalez-ruiz.md)
**Level**          |Beginner
**User Rating**    |5.0 (15 globes from 3 users)
**Compatibility**  |C\#, VB\.NET
**Category**       |[Graphics/ Sound](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/graphics-sound__10-15.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/rodolfo-gonzalez-ruiz-take-a-full-screen-screenshot-capture-screen-and-save-it-to-disk__10-5094/archive/master.zip)





### Source Code

```
Dim screenSize As Size = New Size(My.Computer.Screen.Bounds.Width, My.Computer.Screen.Bounds.Height)
Dim screenGrab As New Bitmap(My.Computer.Screen.Bounds.Width, My.Computer.Screen.Bounds.Height)
Dim g As System.Drawing.Graphics = System.Drawing.Graphics.FromImage(screenGrab)
g.CopyFromScreen(New Point(0, 0), New Point(0, 0), screenSize)
screenGrab.Save("C:\screenGrab.bmp")
'or screenGrab.Save("C:\screenGrab.jpg", System.Drawing.Imaging.ImageFormat.Jpeg)
```

