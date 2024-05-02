Free trial bypass:
When your free trial expires, install appcleaner at https://freemacsoft.net/appcleaner/ and reinstall Keyboard Maestro after cleaning it, you will have to set up the macros again, however.




In this guide, you will learn to set up multi-instancing on MacOS with the help of Keyboard Maestro.
You will need-
  At least 2 instances
  Keyboard Maestro
  Rectangle
For this guide, I will be setting up 4 instances but you can set up as many as you'd like by changing the macros accordingly

standardsettings F3Pause on world load:
In standardsettings, you should enable an option which does the F3 + ESC keybind upon world loading, enabling this option increases visiblity and removes the need for the unfocus parts of the macros if not possible(i.e- hide dock is on).

![image](https://github.com/skillphobia/MacOS-multi-instancing-with-Keyboard-Maestro/assets/165536766/5c1b3032-3e5d-4804-965c-b132e246a9bf)


Step one: Installing Keyboard Maestro and Rectangle
Head to https://www.keyboardmaestro.com/main/ and install Keyboard Maestro, open the file and follow the instructions to install the app.
Then, go to https://rectangleapp.com and install rectangle.

Step two: Setting up Rectangle
After installing rectangle, click its menu on the top bar and click on settings.
![image](https://github.com/skillphobia/MacOS-multi-instancing-with-Keyboard-Maestro/assets/165536766/81ad6e79-e559-4ee3-985b-7b88043e1b19)
In there, you should set up shortcuts for maimizing a window, setting the positions of windows according to how many instances you are settings up. (eg: 2 instance - Halves, 3 instances - Thirds, 4 instances- Fourths or Corners)
![image](https://github.com/skillphobia/MacOS-multi-instancing-with-Keyboard-Maestro/assets/165536766/899af5b4-76eb-42df-a0eb-9e81e0b5fed4)

Step three: Setting up the macros
You should have Keyboard Maestro, your instances, and Rectangle set up by now. We will set up the macros.
I will be setting up 4 instances, so I will need 4 macros for resetting in-game, 4 for resetting in the reset screen, 4 for selecting the instance, and 1 for resetting all instances.
This totals to 13 macros, but this will vary based on how many instances you decide to set up.
Reset all:
  Press the + button on the bottom to create a macro.
  ![image](https://github.com/skillphobia/MacOS-multi-instancing-with-Keyboard-Maestro/assets/165536766/c47c0633-8714-495b-865d-2a331256edb1)
  Select "this hotkey" and set your shortcut
  ![image](https://github.com/skillphobia/MacOS-multi-instancing-with-Keyboard-Maestro/assets/165536766/7b5ae621-f030-416f-8a46-dff5ae94c26c)
  Now, for resetting, you should have your instances ready in their positions
  ![image](https://github.com/skillphobia/MacOS-multi-instancing-with-Keyboard-Maestro/assets/165536766/29494a4b-71ac-4f7f-8628-1385787cddb6)
  In Keyboard Maestro, select "new action" and select "Move or click mouse"
  ![image](https://github.com/skillphobia/MacOS-multi-instancing-with-Keyboard-Maestro/assets/165536766/f06b8c31-745f-4f5d-a7e6-132dbc1f9136)
  Click "get" to get the position of anywhere in the first instance, after you got the position, set the relative to "absolute position".
  Now, add another action, this time, "Type a keystroke" and set it to your reset keybind.
  Repeat the same actions but with different positions so all instances get reset.

  
  COORDINATES WILL VARY!
  ![image](https://github.com/skillphobia/MacOS-multi-instancing-with-Keyboard-Maestro/assets/165536766/3749b6d3-78dc-4f96-8618-2def4599c667)

  Now, after all of that, add an action to click at the botton left corner of your screen, and another one to just move it back to the center, this will make sure no window is focused.
  
  
  ![image](https://github.com/skillphobia/MacOS-multi-instancing-with-Keyboard-Maestro/assets/165536766/2270ddf0-ad12-42d6-b84f-2b7acbd71831)
  It should look something like this.


  Repeat this for all your instances. 
Resetting an instance in-game:
  Make a new macro, name it whatever you'd like. Add a new action, "Type a keystroke," set it to your reset keybind, then add "Type a keystroke" again, but set it to the respective keybing which you set in Rectangle. Then add the same set of actions to make sure no window is focused that you set in the previous macro.
  ![image](https://github.com/skillphobia/MacOS-multi-instancing-with-Keyboard-Maestro/assets/165536766/79b5e4ac-2221-43c3-97a6-2545f8a2b8ac)

  It should look something like this, with different shortcuts.
  Repeat this for all instances.

Resetting in reset screen:
  This is similar to the macro you made for resetting all, the only difference is that youre resetting one instance at a time instead of all of them. So, each macro should look something like this
  ![image](https://github.com/skillphobia/MacOS-multi-instancing-with-Keyboard-Maestro/assets/165536766/c6d1bc98-2422-49b0-a82c-017d072bde12)


  COORDINATES AND SHORTCUTS WILL VARY

Selecting an instance:
  
  Create a new macro, click new action, and add "Move or click mouse" and set the coordinates to any part of the instance window and set the relativity to "absolute position," then add the action "type keystroke" and add your shortcut for maximizing a window, the add another "type keystroke" action and press the "escape" key.
  It should look something like this:

  ![image](https://github.com/skillphobia/MacOS-multi-instancing-with-Keyboard-Maestro/assets/165536766/ef45e622-6912-4e2d-a24b-ef6dd43fba5f)




  Repeat this for all instances.






Happy resetting!
