Creating a game object:
  function(){
    var game = new Phaser.Game(320,480, Phaser.CANVAS, "game");
  }
  
adding states to your game:
  game.state.add("State_name1", state_name2);
  
Note: make sure that state_name2 matches the var name in that State

Note: to call that state from a different state:
  game.state.start("State_name1");
  
Start a state:
  game.state.start("State_name");

Make a Prototype:
  state.prototype = {
    ...
   }
   
Make a function:
  func_name : function(){
    ....
  },
  func_name: function(){
   ....
  }
  
When having multiple functions, put a comma after each one except the last one.

Loading an image:
  this.game.load.image("var_name","path_to_img");
 
Loading a spritesheet:
  this.game.load.spritesheet("var_name","path_to_img",x_frame_size, y_frame_size);

Adding a loading bar to your preload state:
  var loadingBar = this.add.sprite(x_location,y_location,"var_name");
  
Set a loading bar to visibly load on your game:
  this.load.setPreloadSprite(loadingBar);
  
Anchor a sprite:
  var_name.anchor.setTo(x_location, y_location);
 
Add a button:
  this.game.add.button(x_location, y_location, "var_name", button_action, this);
