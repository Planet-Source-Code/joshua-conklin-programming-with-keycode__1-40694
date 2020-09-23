<div align="center">

## Programming with keycode


</div>

### Description

This article is trying to help show how to program in visual basic, how to make applications execute commands upon the keystroke of a specific key.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Joshua Conklin](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/joshua-conklin.md)
**Level**          |Beginner
**User Rating**    |4.0 (8 globes from 2 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__1-43.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/joshua-conklin-programming-with-keycode__1-40694/archive/master.zip)





### Source Code

Have you ever wondered how to make your application execute a unique command when a specific key has been pressed?
Say you press the 'w' key, you could make your program say "Hey! don't touch my w key on the keyboard its mine!".
Or knowing this you can create games. You can be allowed to use the arrow keys for movement of characters or make the spacebar shoot or punch or whatever.
First off create a new project and start with your Form1..
double click on your form and get to the form1 code area. from here, select form1 in the item combo box and then in the second combo box on the right, select your form key down event.
so right now you should see this:
<br>
<br>
Private Sub Form_KeyDown(KeyCode As Integer, Shift As Integer)
<br>
End Sub
<br>
<br>
<br>
now for some easy stuff... lets do what i said in the above situation. Lets make our app say "dont touch my letter W!!"
all you have to do is insert this code between your form_keydown event:
<br>
<br>
If KeyCode = vbKeyW Then MsgBox "Dont touch my letter W!!"
<br>
<br>
Taa Daa!! success eh? It always feels good when the W no touch test is a success! :D
Now you have a basic idea!
Now with this knowledge we can start doing some tricky stuff...
you could add a shape like a circle and move it left or right... want to know how? I bet you do!
so add the Circle and name it 'theCircle'
this is where some of your own personal programmign skills would come on.. i am sure there are hundreds of ways to make movements and stuff, but the way i do it is this... I create individual Private Subs for each different movement or event that i want my circle to do... and hten i put my code in it. I will show you below and you can figure it out:
<br>
<br>
<br>
Private Sub Form_KeyDown(KeyCode As Integer, Shift As Integer)
<br>
If KeyCode = vbKeyLeft Then CircleGoLeft
If KeyCode = vbKeyRight Then CircleGoright
<br>
End Sub
<br>
<br>
Private Sub CircleGoLeft()
<br>
 thecircle.Left = thecircle.Left - 100
<br>
End Sub
<br>
<br>
Private Sub CircleGoright()
<br>
thecircle.Left = thecircle.Left + 100
<br>
End Sub
<br>
<br>
<br>
OOOO!!! awesome huh? just think now! The possibilities are endless! Now you are on your way to gaming in no time! Drop me a line if you think my tut' really stinks or you have an idea, or want to tell me that you just sold a million copies of your game and that i was the one who taught you form_keydown event :-)
Happy Programming!
* Love Peace & Chicken Grease *
- Josh Conklin

