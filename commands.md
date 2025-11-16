# Commands

Commands are what you use to display stuff on screen, move things around and whatever.  
  
**Here's some stuff you should be able to understand:**
- string: Text (use quotes if it contains spaces "such as this")
- float: Number with decimal places if needed (ex: 1.2, 0.5, 3.14)
- integer: Number without decimal places (ex: 1, 2, 3)
- boolean: `true` or `false`
  

**But also some more important stuff:**
- Node ID's are strings that should be given to stuff you create on screen. It can be used to change properties of a node **(which is something that is on screen, most nodes have an ID assigned)** such as it's position, size, color, etc.
- When you create a node using GStyle2, the Node ID you assign it will be transformed into `authorName-packID-cleanedID` **(ex: `jarvisdevil-jarvisdevil.test_pack-my_actual_node_id`)** to make sure it doesn't conflict with other things. **(cleanedID is your node ID but lowercase and spaces are replaced with underscores)**
- List of fonts you can choose from are: bigFont, ArchivoBlack, BitcountGridDouble, BitTrip, Oswald, Roboto, ZalandoSansExpanded. **(bigFont is Pusab)**
- **If you have read all of the documentation here and still don't understand anything about how to create a GStyle2 pack then why are you even trying?**

## List of Commands

- draw.rect x y w h r g b a id
  - x, y: position (float)
  - w, h: width and height (float)
  - r, g, b, a: color (int 0-255)
  - id: node id (string)

- draw.circle x y radius r g b a id
  - x, y: center position (float)
  - radius: float
  - r, g, b, a: color (int 0-255)
  - id: node id (string)

- text.create "text" scale x y font id
  - text: text (string)
  - scale: size (float)
  - x, y: position (float)
  - font: font name (string)
  - id: node id (string)

- sprite.create filename scale x y id
  - filename: image file name inside `packs/<pack>/sprites/` (string)
  - scale: size (float)
  - x, y: position (float)
  - id: node id (string)

- audio.music file loop fadeIn channel
  - file: filename inside `packs/<pack>/audio/` (string)
  - loop: if the audio should loop (boolean)
  - fadeIn: seconds to fade in (use 0 for immediate, float)
  - channel: channel id (int. if you don't know what this is, just use 0)

- audio.effect file
  - file: filename inside `packs/<pack>/audio/` (string)

- audio.stopMusic (no args)
  - stops all music playback

- audio.stopEffect (no args)
  - stops all effect playback

- set.position x y id
  - x, y: position (float)
  - id: node id (string)

- set.scale scale id
  - scale: size (float)
  - id: node id (string)

- set.x value id
  - value: x position (float)
  - id: node id (string)

- set.y value id
  - value: y position (float)
  - id: node id (string)

- set.scaleX value id
  - value: width (float)
  - id: node id (string)

- set.scaleY value id
  - value: height (float)
  - id: node id (string)

- set.rotation degrees id
  - degrees: rotation in degrees (int 0-360)
  - id: node id (string)

- set.skewX value id
  - value: skew of x (float)
  - id: node id (string)

- set.skewY value id
  - value: skew of y (float)
  - id: node id (string)

- set.anchorX value id
  - value: anchor of x (float)
  - id: node id (string)

- set.anchorY value id
  - value: anchor of y (float)
  - id: node id (string)

- set.z zIndex id
  - zIndex: z-order (int)
  - id: node id (string)

- set.visible bool id
  - bool: if it should be visible (boolean)
  - id: node id (string)

- set.contentWidth width id
  - width: width of content (float)
  - id: node id (string)

- set.contentHeight height id
  - height: height of content (float)
  - id: node id (string)

- set.color r g b id
  - r, g, b: color (int 0-255)
  - id: node id (string)

- set.opacity value id
  - value: opacity (int 0-255)
  - id: node id (string)

- pack.info key
  - key: key to log (string)

- log.info message
  - message: message to log (string)

- log.warn message
  - message: message to log as a warning (string)

- log.error message
  - message: message to log as an error, but why? (string)
