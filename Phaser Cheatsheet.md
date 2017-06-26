-<strong> Creating a game object:</strong>
  
  - function(){
    var game = new Phaser.Game(320,480, Phaser.CANVAS, "game");
  }
  
-<strong> adding states to your game:</strong>
  - game.state.add("State_name1", state_name2);
  

<strong>Note:</strong> make sure that state_name2 matches the var name in that State

<strong>Note:</strong> to call that state from a different state:
  - game.state.start("State_name1");
  

-<strong> Start a state:</strong>
  - game.state.start("State_name");


-<strong> Make a Prototype:</strong>
  - state.prototype = {
    ...
   }
   

-<strong> Make a function:</strong>
  - func_name : function(){
    ....
  },
  func_name: function(){
   ....
  }
  


-<strong> When having multiple functions, put a comma after each one except the last one.</strong>



-<strong> Loading an image:</strong>
  - this.game.load.image("var_name","path_to_img");
 
-<strong> Loading a spritesheet:</strong>
  - this.game.load.spritesheet("var_name","path_to_img",x_frame_size, y_frame_size);

-<strong> Adding a loading bar to your preload state:</strong>
  - var loadingBar = this.add.sprite(x_location,y_location,"var_name");
  
-<strong> Set a loading bar to visibly load on your game:</strong>
  - this.load.setPreloadSprite(loadingBar);
  
-<strong> Anchor a sprite:</strong>
  - var_name.anchor.setTo(x_location, y_location);
 
-<strong> Add a button:</strong>
  - this.game.add.button(x_location, y_location, "var_name", button_action, this);
