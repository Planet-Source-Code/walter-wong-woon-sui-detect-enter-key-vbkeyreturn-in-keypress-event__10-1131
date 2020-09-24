<div align="center">

## Detect Enter Key \(vbkeyreturn\) in Keypress Event


</div>

### Description

It able to detect ENTER key press by user. VB6 use " Keyascii = vbkeyreturn " but .Net need to write another function to detect it. Try to use this function to help you. Vote this code if you found it useful 2 you.
 
### More Info
 
user input

Boolean value


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Walter Wong Woon Sui](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/walter-wong-woon-sui.md)
**Level**          |Beginner
**User Rating**    |3.1 (31 globes from 10 users)
**Compatibility**  |VB\.NET
**Category**       |[Controls/ Forms/ Dialogs/ Menus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/controls-forms-dialogs-menus__10-3.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/walter-wong-woon-sui-detect-enter-key-vbkeyreturn-in-keypress-event__10-1131/archive/master.zip)





### Source Code

```
Public Function KeyAscii(ByVal UserKeyArgument As KeyPressEventArgs) As Short
 KeyAscii = Asc(UserKeyArgument.KeyChar)
End Function
Private Sub txtusername_KeyPress(ByVal sender As Object, ByVal e As System.Windows.Forms.KeyPressEventArgs) Handles txtusername.KeyPress
 If User.KeyAscii(e) = 13 Then
  msgbox "you press ENTER key"
 End If
End Sub
```

