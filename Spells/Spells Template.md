Spells Template
---
A spell is defined using an element named **spell**. Its content will consist of several elements, which will define your spell.

The following is a list of elements that can be used:
* **name (ABC)**
* **level (##)**
* **school (A | C | D | EN | EV | I | N | T)** - *Spell School*
  * **A** = Adjuration
  * **C** = Conjuration
  * **D** = Divination
  * **EN** = Enchantment
  * **EV** = Evocation
  * **I** = Illusion
  * **N** = Necromancy
  * **T** = Transmutation
* **ritual (YES | NO)** - *This element may be left out if the spell is not a ritual.*
* **time (ABC)** - *Casting Time*
* **range (ABC)**
* **components (ABC)**
* **duration (ABC)**
* **text (ABC)** - *Spell Description. Multiple text elements may be inputted. Each one represents a paragraph. IF the ```auto_indent``` attribute is set in the compendium element, paragraphs after the first will automatically indent the first line.*
* **roll (D20)** - *Dice Roll Formulas. Ability modifiers can be inputted using ```STR```, ```DEX```, ```CON```, ```INT```, ```WIS```, and ```CHA```. To input the class spell ability modifier, use ```SPELL```.

* **classes (ABC, ABC, ...)** - Classes.
