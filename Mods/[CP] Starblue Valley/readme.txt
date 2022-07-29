# Starblue-Valley
 A world recolor mod for Stardew Valley.


### HOW TO INSTALL: 
* Install the most recent versions of SMAPI and Content Patcher.
* Run SMAPI to start the game, then close it to generate the config.json.
* Open the config.json and edit it to your preferences.
* Run SMAPI and play.


### LANGUAGE SUPPORT: 
* **Starblue is only available in English at this time.  I will not be adding cross-language support.**
* For non-English-speaking players, I am looking at options to easily enable language compatibility patches. Once that's ready, I'll release a guide on how to make assets for Starblue in your language.


### CHANGELOG: 
* Updated code on craftables and flooring so they display correctly based on season and location.
* A partial/basic recolor of {{season}}\_island\_tile\_sheet_1. Beach farm tiles will no longer be mismatched. This is a WIP.
	* Modifies: {{season}}\_island\_tile\_sheet_1
* Adjustments to the seasonal menu map. The beach farm interface now matches the other seasons, and the Ginger Island border matches the interface.
	* Modifies: map
* Added code to suppress Ginger Island's use of the summer_outdoorsTileSheet during summer. This makes Ginger Island appear with 100% vanilla coloration, but fixes all the mismatches/errors during the summer season. 
* Caroline's Greenhouse has now been recolored to match the rest of the interior. I've also recolored the door to the greenhouse and the floor tile in front so they match the rest of the interiors.
	* Modifies: CarolineGreenhouseTiles, CarolineGreenhouseTiles\_rainy, townInterior\_2
* Fixed the fruit trees tilesheet so mango/banana trees aren't invisible.
	*Modifies: fruitTrees
* Fixed the flooring tilesheets so the new stone walkway and rustic plank floors are visible.
	*Modifies: Flooring, Flooring_winter
* The tailoring menu interface has been recolored.
	* Modifies: tailoring
* The shipping bin has now been removed from the main tilesheet and is a separate configurable option. Please note I added this prior to 1.5 and I have not yet properly optimized it to work with the new island bin or the moveable bin.
	* Modifies: {{season}}\_outdoorsTileSheet
* The menu character sprite background has been recolored to match both the interface and the Starblue environment; it's also seasonally dynamic.
	* Modifies: daybg, nightbg
* The Language selection buttons have been recolored to match the rest of the interface.
	* Modifies: LanguageButtons
* Additional items have been recolored on the craftables sheet: snowman, some rarecrow stakes, the Stardew Hero Trophy, and the Solid Gold Lewis.
	* Modifies: craftables
* The butterfly hutch was missing its roof. It should now appear without issue.
	* Modifies: furniture
* Minor fixes.


### CONFLICTS: 
* Content Patcher packs do not modify game files. However, almost every tilesheet in the game will be modified by Starblue Valley. Almost all of the new additions have a config menu option to turn them on or off, so please study the configuration menu options to turn off the options you don't need.
* If you are looking to mix my assets with assets from other mods, you will either need to adjust your load order or edit my tilesheets to remove whichever sections you don't want to use. 
* Starblue may conflict with custom maps. I will not provide further support or assets for custom mods. If you are a modder who wants to make provide custom assets for Starblue, please feel free to use my assets to make your mods compatible. Make sure to credit me and provide a link back to Starblue.
* To repeat: **I WILL NOT BE SUPPORTING STARDEW VALLEY EXPANDED SO STOP ASKING.** It's FlashShifter's mod; bug him instead.
* Starblue's seasonal maps are not compatible with Bohum's NPC Map Locations. Starblue will detect whether you have Bohum's mod installed and automatically disable seasonal maps in that case.


### CONFIGURATION OPTIONS: 
* Mailbox: basic, fancy, none. Default: basic.
	* A ‘fancy’ black Victorian mailbox with seasonal decorations has been added as an optional mailbox. The ‘basic’ mailbox recolors the wood post. Select ‘none’ to disable the mailbox.
	* Modifies: {{season}}\_outdoorsTileSheet
* Oak Trees: pink, green. Default: pink.
	* Gives you the option of oak trees having green or pink leaves during spring. Green for a natural look, pink to go Full Candyland.
	* Modifies: tree1, spring\_outdoorsTileSheet
* Maple Trees: green, white. Default: green.
	* Gives you the option for green or white leaves on maple trees during spring. 
	* Modifies: tree2, spring\_outdoorsTileSheet
* Pine Trees: pine, spruce. Default: pine.
	* Choose between a green pine tree and a silvery teal blue spruce tree. Spruce tree coloration persists through all seasons.
	* Modifies: tree3, {{season}}\_outdoorsTileSheet
* Grass: basic, flowering, none. Default: basic.
	* Use either basic grass or the basic flowering grass from my Flowering Grass mod. Set to ‘none’ if using custom grass from another mod.
	* Modifies: grass
* WorldMap: true, false. Default: true.
	* If you use Bohum’s NPC Locations or another mod that changes the world map, keep this set to ‘false’ to avoid conflicts.
	* Modifies: map
* GroundUnderBowl: default, grass, dirt, void, darkgrass. Default: default.
	* Useful for custom maps that change the dog bowl’s position. Leave as default unless using one of these.
* ForeverPink: false, true. Default: false.
	* An option added by mouse by request to keep the pink leaf oak trees for spring, summer, and fall. I’ve left it as an option.
* BlossomTrees: false, true.  Default: true.
	* Sets the fruit trees in game to use my blossom trees. Uses the non-evergreen version of the orange trees only. If you use another mod’s fruit trees, set this to false.
	* Modifies: fruitTrees
* Interiors: false, true. Default: true.
	* A partial recolor of the interior. Woodwork and wooden flooring now use my neutral wood tones, and there have been adjustments to countless objects and several wallpapers and floors. The greenhouse flooring (now uses a neutral version of my new crystal paths). A WIP, does not yet handle Caroline’s tea garden or the movie theater interior.
	* Modifies: townInterior, townInterior\_2, Farmhouse\_Tiles, ElliottHouseTiles, CarolineGreenhouseTiles, CarolineGreenhouseTiles\_rainy
* Walls&Floors: a partial overlay for the farmhouse wallpaper and floor options. Mostly changes wood tones, particularly baseboards, to match my neutral wood tones, although a few others have been adjusted to match grass, dirt, straw, and other elements. If you use custom walls and floors in the game, set this to ‘false.’
	* Modifies: walls\_and\_floors
* Interface: false, true. Default: true.
	* A full interface recolor that uses my neutral wood tones. Very chill. Missing 1.5 menus.
	* Modifies: Billboard, chatBox, Cursors, Cursors2, DialogBoxGreen, font\_bold, JunimoNote, letterBG, MenuTiles, textBox, TitleButtons, LanguageButtons, Tailoring, daybg, nightbg
* Furniture: false, true. Default: true.
	* A partial overlay of the furniture you can purchase in the game to make it consistent with my neutral wood tones and other interior elements. WIP. If you use a custom furniture replacer in the game, set this to ‘false.’
	* Modifies: Furniture
* Flooring: false, true. Default: true.
	* Recolors several base game paths and floors with my seasonal versions. All associated inventory icons were updated to match. All flooring has seasonal variations when outdoors.
		* Wooden and straw floors use my neutral wood tones.
		* Weathered floors have seasonal weathered brick tones.
		* Gravel paths have been adjusted to be more neutral.
		* Cobblestone and stepping stone paths have been significantly desaturated, but now have seasonal moss and shoots of grass growing around them. The cobblestones are iced over, while the stepping stones are covered in snow.
		* Wood paths now use my neutral wood tones with seasonal grass shoots and an outdoor winter variant.
		* The recently added brick floors were given a neutral update. I may revisit this.
     * Several floors were substantially reworked.
		* I never liked the stone floors, so I replaced these with a cobblestone floor matching Pelican Town’s main square. It has all seasonal variants and looks very nice in the game. The inventory icon has been reworked to match.
		* I hate the crystal floors and crystal paths. So I redid them.
			* Crystal Floors: use a diagonal tile pattern that has been given a subtle bluish green color shifting effect using a seamless pattern I stitched together from my opal paths. Much more like crystal, in my opinion. Matching inventory tile available.
			* Crystal Paths: I created a partly transparent ‘glass shard’ effect that tiles quite nicely. Matching inventory tile available.
	* Due to the crystal paths, edit mode replaces the entire file instead of simply overlaying them. 
	* Replaces: Flooring, Flooring\_winter
	* Modifies: springobjects
* HardwoodFence: false, true. Default: true.
	* Makes the hardwood fence use my neutral wood tones.
	* Replaces: Fence5
	* Modifies: springobjects
* Craftables: false, true. Default: true.
	* A partial seasonal overlay of the crafting machines and several craftable items. WIP.
		* Wooden elements, including crafting machines, signposts, scarecrow/rarecrow posts, barrels, chests, braziers, lamp posts and some furniture use my neutral wood tones.
		* The snowman is colored to match Starblue snow.
		* Beehives have snow on their roofs in winter.
		* The tub o’ flowers object now has seasonal variations. (Credit to SchrodingersKit’s Tub O’ Flowers Color Varieties.)
			* Spring: Sunrise
			* Summer: Rainbow
			* Fall: Sunset
			* Winter: Icy Blues
		* The Lucky Cat has a more neutral brass recolor, as does the Iridium Cat, Lewis's Statue, and the Stardew Hero Trophy. 
	* Set to ‘false’ if using a separate craftables recolor pack.
	* Modifies: Craftables, springobjects
* Junimo Huts: false, true. Default: true.
	* Makes the Junimo Huts match the Starblue palette. If using custom Junimo Huts, set this to false.
	* Replaces: Junimo Huts
* ShaneCoop: false, true. Default: true.
	* If using custom buildings that include Shane’s coop, set this to ‘false.’
	* Modifies:  {{season}}\_outdoorsTileSheet
* ShipBin: false, true. Default: true.
	* If using a custom shipping box, set this to 'false.'
	* Modifies: {{season}}\_outdoorsTileSheet
* SpringGrass: green, blue. Default: green.
	* Makes the spring grass even bluer! Grass is a deep teal-green shade. Really pops the Full Candyland tree choices.
	* Modifies: secondary overlay to spring\_outdoorsTileSheet, spring\_outdoorsTileSheet2, and spring\_monsterGraveTiles


### CREDITS: ###
* hatmouse for the unofficial updates and for help coding around the Ginger Island summer issues.
* SpringSong for matching pet bowl grass for custom maps.
* Pathoschild for the Content Patcher (especially config options!).
* [ThisIsLonelyStar](https://www.youtube.com/watch?v=pK9J9eCZwVk) for donating Calisto farm so I could use it in my preview pic.


### POLICY: ###
* Please do not upload my mods anywhere else, especially sites with a profit motive. (Basically, don't make money off my stuff.)
* You may use my assets to create patches for your own mods. Please add credit and a link back to my mod. You may upload patches to mods that have donations open. You may NOT upload these patches to Patreon or other paysites.
* If you need me to add anything to Starblue to accommodate your mods, I do intend to get a GitHub running so I can accept pull requests, but for now, please message me on Discord.
