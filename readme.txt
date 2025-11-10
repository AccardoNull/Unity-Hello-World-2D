Implemented features:

- Made a player character that has Walk. Idle. Jump animations. The character uses spritesheet animation, sets to a reasonable sample frequency, and transitions appropriately, smoothly, and on time using the speed parameter given player inputs.

- The Player object has a player movement script that implements left, right, and jump movement base don player inputs. it can only jump once when on the ground with functions that correctly detect being on the ground for jumps. The player character has smooth, no sticky left-right movement with no wall sticking.

- The player character has clean reasonable physical bounds that match up with the visual expectations of the character and environment.

- The world is physical but only the physical platform layer. It makes use of the tilemap collider and additionally correctly setup composite collider to ensure smooth contact.

- Correctly support moving platform interactions by using physics callbacks and the scene hierarchy. Have four horizontal movement platforms and three vertical movement platforms. Every platform should oscillate between two points at reasonable rates.

- The camera follows the player through parenting.

- Extend the world and polish both horizontal and vertical transitions/platforms such that the world is traversable given the character's movement abilities, with multiple regions that player can now access.