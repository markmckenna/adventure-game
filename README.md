Adventure Game
==============

A choose-your-own-adventure style game engine/platform.

A story-driven adventure game where the player moves through a semi-scripted environment and tries to survive to the end.
  - Each 'scene' accompanied by a picture and a description, plus a choice the player must make.  Different choices result in
    different outcomes, some better than others.
  - Multiple story endings, achievements for getting more of them
  - Start with a simple demo renderer, story but no pictures
  - Move on to an Android renderer so it can be easily passed around
  - Different renderers can all render the same content which can be served on the web

Architecture
------------

- Base library which parses a JSON-derived content file
	- Support compressed/encrypted payloads too (embedded cryptokey)
- Test app which supports text output and keyboard entry, like a classical adventure game
	- Top-level Main object holding everything in place
	- Parse JSON of command-line supplied data file

JSON Format
-----------

```json
{
	
}
```