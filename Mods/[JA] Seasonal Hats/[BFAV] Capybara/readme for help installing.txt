README

INSTALL:

(1) download and install Paritee’s Better Farm Animal Variety (BFAV) mod from nexus mods

(2) download and extract the "[BFAV] Capybara" folder into your StardewValley/Mods folder. 

(3) within the "[BFAV] Capybara" folder, locate and copy the "animal_shop_capybara.png" file.
	
(4) go into your "Paritee's Better Farm Animal Variety (BFAV)" folder located in your StardewValley/Mods folder. 

(5) paste the copied "animal_shop_capybara.png" file into the assets folder 
				
assets folder location	| StardewValley/Mods/Paritee's Better Farm Animal Variety/Assets

(5) go into your "Paritee's Better Farm Animal Variety (BFAV)" folder and open the config.json file.

			- open config.json file located in \stardewvalley\mods\paritee's better farm animal variety
			- scroll to end of code, there should be FOUR brackets
			- after the SECOND bracket add a comma, then insert the following code:


    "Capybara": {
      "Types": [
        "Capybara"
      ],
      "Buildings": [
        "Barn",
        "Big Barn",
        "Deluxe Barn"
      ],
      "AnimalShop": {
        "Name": "Capybara",
        "Description": "A shy, friendly girl to help you make friends!",
        "Price": "2000",
        "Icon": "assets\\animal_shop_capybara.png"
      }
