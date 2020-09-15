STARBLUE VALLEY - a world recoloring mod.


HOW TO INSTALL:
	- Install the most recent versions of SMAPI and Content Patcher.
	- Run SMAPI to start the game, then close it to generate the config.json.
	- Adjust the config.json to your preferences.
	- Run SMAPI and play.


CHANGES:
	- Files now compatible with the most recent update of SDV (1.4.5).
	- Now uses a config.json to handle variations such as pink oak trees.
	- Recolors of the new building exteriors, including Pam’s House and the Movie Theater.
		- Modifies: {{season}}_town
	- A full recolor of the Night Market, including color-matched docks, revamped duochromatic color schemes for the boats themselves to inject subtle but still-vibrant color into the market, and various small fixes (the mermaid sign now looks like the mermaid!).
		- Modifies: night_market_tilesheet_objects
	- Support for the new outdoors, desert, and monster grave tiles added by prior updates.
		- Modifies: {{season}}_outdoorsTileSheet, {{season}}_outdoorsTileSheet2, {{season}}_monsterGraveTiles
	- Recolored the new desert tiles to match the rest of the desert.
		- Modifies: DesertTiles_Extended
	- Recolored the new desert trader’s tent and area to match the Starblue palette.
		- Modifies: temporary_sprites_1
	- Joja’s exterior is now more consistent across seasons and uses more metal and concrete in its color scheme.
		- Modifies: {{season}}_town
	- The seasonal map now shows all new buildings.
	- Several in-game cutscenes have had their assets recolored, such as Harvey’s Balloon - Ride basket, Elliott’s boat, and Vincent’s sand castle.
	- Now includes my Blossoming Trees and Flowering Grass as config options. See config - menu documentation for details.
	- New seasonal mailbox option.
	- Pink oak trees now set via config.json, with the option to set to persist.
	- New white maple option for maple trees in spring.
	- New blue spruce option for pine trees.
	- A major interior recolor using my neutral wood tones and countless other items, - impacting the town interiors, buyable walls, floors, and furniture, and the farmhouse. See the config menu options for details on what is affected.
	- An optional interface in my neutral wood tones.
	- Recolors of several craftable items in neutral tones, including flooring/paths, hardwood - fences, and craftable objects. See config menu options for details.
	- Optional bluer grass for spring.
	- Option to disable Shane’s chicken coop.
	- More event objects recolored, including the traveler’s wagon.
	- Tons more small fixes, from small objects I missed on prior passes to bad transparencies and other errors.


CONFLICTS:
	- Content Patcher packs do not modify game files. However, almost every tilesheet in the game will be modified by Starblue Valley. Most of the new additions have a config menu option to turn them on/off, so please study the configuration menu options and adjust your load orders accordingly.
	- Starblue may conflict with custom maps. I will not provide further support or assets for custom mods. If you are a modder who wants to make provide custom assets for Starblue, please feel free to use my assets to make your mods compatible. Make sure to credit me and provide a link back to Starblue.
	- Starblue's seasonal maps are not compatible with Bohum's NPC Map Locations. Starblue will detect whether you have Bohum's mod installed and automatically disable seasonal maps in that case.


LANGUAGE SUPPORT:
	- Starblue is only available in English at this time. While the code provides the option of adding overlays based on language (Portuguese overlay examples are contained in the file), I will not be generating further overlays due to the time commitment. If you are a non-English-speaking player who wants to help make Starblue compatible in your language, feel free to reach out to me and I’ll explain what you need to do.


CONFIG.JSON MENU OPTIONS:
	- Mailbox: basic, fancy, none. Default: basic.
		- A ‘fancy’ Victorian-style mailbox with seasonal decorations has been added as an optional mailbox. The ‘basic’ mailbox recolors the wood post. Select ‘none’ to use a different mailbox option.
		- Modifies: {{season}}_outdoorsTileSheet
	- Oak Trees: pink, green. Default: pink.
		- Gives you the option of oak trees having green or pink leaves during spring. Green for a natural look, pink to go Full Candyland.
		- Modifies: tree1, spring_outdoorsTileSheet
	- Maple Trees: green, white. Default: green.
		- Gives you the option for green or white leaves on maple trees during spring. 
		- Modifies: tree2, spring_outdoorsTileSheet
	- Pine Trees: pine, spruce. Default: pine.
		- Choose between a green-toned pine tree and a silver-blue blue spruce tree. Spruce tree coloration persists through all seasons.
		- Modifies: tree3, {{season}}_outdoorsTileSheet
	- Grass: basic, flowering, none. Default: basic.
		- Use either basic grass or the flowering grass from my Flowering Grass mod. Set to ‘none’ if using custom grass from another mod.
		- Modifies: grass
	- WorldMap: true, false. Default: true.
		- If you use Bohum’s NPC Locations or another mod that changes the world map, set this to ‘false’ to avoid conflicts.
	- Modifies: map
	- GroundUnderBowl: default, grass, dirt, void, darkgrass. Default: default.
		- Useful for custom maps that change the dog bowl’s position. Leave as default unless using one of these.
	- ForeverPink: false, true. Default: false.
		- An option added by mouse by request to keep the pink leaf oak trees for spring, summer, and fall. I’ve left it as an option.
	- BlossomTrees: false, true.  Default: true.
		- Sets the fruit trees in game to use my blossom trees. Non-evergreen version of the orange trees only. If you use another mod’s fruit trees, set this to false.
		- Modifies: fruitTrees
	- Interiors: false, true. Default: true.
		- A partial recolor of the interior. Woodwork and wooden flooring now use my neutral wood tones, and there have been adjustments to countless objects and several wallpapers/floors. The greenhouse flooring (now uses a toned-down version of my new crystal paths). A WIP, does not yet handle Caroline’s tea garden or the movie theater interior.
		- Modifies: townInterior, townInterior_2, Farmhouse_Tiles, ElliottHouseTiles
	- Walls&Floors: a partial overlay for the farmhouse wallpaper and floor options. Mostly changes wood tones, particularly baseboards, to match my neutral wood tones, although a few others have been adjusted to match grass, dirt, straw, and other elements. If you use custom walls and floors in-game, set this to ‘false.’
		- Modifies: walls_and_floors
	- Interface: false, true. Default: true.
		- A full interface recolor that uses my neutral wood tones. Very chill. WIP, but mostly complete.
		- Modifies: Billboard, chatBox, Cursors, Cursors2, DialogBoxGreen, font_bold, JunimoNote, letterBG, MenuTiles, textBox, TitleButtons
	- Furniture: false, true. Default: true.
		- A partial overlay of the furniture you can purchase in-game to make it consistent with my neutral wood tones and other interior elements. WIP. If you use custom furniture in-game, set this to ‘false.’
		- Modifies: Furniture
	- Flooring: false, true. Default: true.
		- Recolors several base game paths and floors with my seasonal versions. All associated inventory icons were updated to match. All flooring has seasonal variations when outdoors.
			- Wooden and straw floors use my neutral wood tones.
			- Weathered floors have seasonal weathered brick tones.
			- Gravel paths have been adjusted to be more neutral.
			- Cobblestone and stepping stone paths have been significantly desaturated, but now have seasonal moss and shoots of grass growing around them. The cobblestones are iced over, while the stepping stones are snow-covered.
			- Wood paths now use my neutral wood tones with seasonal grass shoots and an outdoor winter variant.
			- The recently-added brick floors were given a neutral update. I may revisit this.
     - Several floors were substantially reworked.
			- I never liked the stone floors, so I replaced these with a cobblestone floor matching Pelican Town’s main square. It has all seasonal variants and looks very nice in-game. The inventory icon has been reworked to match.
			- I also hate the crystal floors and crystal paths. So I redid them.
				- Crystal Floors: use a diagonal tile pattern that has been given a subtle blue-green color-shift effect using a seamless pattern I stitched together from my opal paths. Much more crystal-like, in my opinion. Matching inventory tile available.
				- Crystal Paths: I created a semi-transparent ‘glass shard’ effect that tiles quite nicely. Matching inventory tile available.
		- Due to the crystal paths, edit mode replaces the entire file instead of simply overlaying them. 
		- Replaces: Flooring, Flooring_winter
		- Modifies: springobjects
	- HardwoodFence: false, true. Default: true.
		- Makes the hardwood fence use my neutral wood tones.
		- Replaces: Fence5
		- Modifies: springobjects
	- Craftables: false, true. Default: true.
		- A partial seasonal overlay of the crafting machines and several craftable items. WIP.
			- Wooden elements, including crafting machines, signposts, scarecrow posts, barrels, chests, braziers, lamp-posts and some furniture use my neutral wood tones.
			- Beehives have snow on their roofs in winter.
			- The tub o’ flowers object now has seasonal variations. (Credit to SchrodingersKit’s Tub O’ Flowers Color Varieties.)
				- Spring: Sunrise
				- Summer: Rainbow
				- Fall: Sunset
				- Winter: Icy Blues
			- The Lucky Cat has a more neutral brass recolor, as does the Iridium Cat.
		- Set to ‘false’ if using a separate craftables recolor pack.
		- Modifies: Craftables, springobjects
	- Junimo Huts: false, true. Default: true.
		- Makes the Junimo Huts match the Starblue palette. If using custom Junimo Huts, set this to false.
		- Replaces: Junimo Huts
	- ShaneCoop: false, true. Default: true.
		- If using custom buildings that include Shane’s coop, set this to ‘false.’
		- Modifies:  {{season}}_outdoorsTileSheet
	- SpringGrass: green, blue. Default: green.
		- Makes the spring grass even bluer! Grass is a deep teal-green shade. Really pops the Full Candyland tree choices.
		- Modifies: secondary overlay to spring_outdoorsTileSheet, spring__outdoorsTileSheet2, and spring__monsterGraveTiles


CREDITS:
	- hatmouse for updating this unofficially in the interim, making my job MUCH easier
	- drew on Discord for playtesting
	- SpringSong for matching pet bowl grass for custom maps
	- Pathoschild for the Content Patcher (especially config options!)

POLICY:
	- Please do not upload my mods to sites other than Nexus, especially sites with a profit motive. (Basically don't make money off my stuff.)
	- You may use my assets to create patches for your own mods. Please add credit and a link back to my mod.