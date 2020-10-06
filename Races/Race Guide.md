Races
---
A race is defined using an element named ```race```. Its content can consist of the following elements:
* **name (ABC)**
* **ability (Str ##, Dex ##, ...)** - *Ability score increases. Abilities with increase amounts, separated by commas.
* **size (T | S | M | L | H | G)** - *Creature size*
  * **T** = Tiny
  * **S** = Small
  * **M** = Medium
  * **L** = Large
  * **H** = Huge
  * **G** = Gargantuan
* **speed (##)** - *Speed in feet*
* **spellAbility** - *Spellcasting ability, Strength, Dexterity, etc*
* **proficiency (ABC, ABC, ...)** - *Saving throw and class skill proficiencies. Enter names of abilities or skills separated by commas*
* **trait** - *Racial traits. Multiple traits are allowed. The following elements may be used as content.
  * **name (ABC)**
  * **text (ABC)** - *Trait description. Multiple text elements may be inputted. Each one represents a paragraph. If the ```auto_indent``` attribute is set in the compendium element, paragraphs after the first will automatically indent the first line.
* **modifier (ABC [+/-]##)** - *Modifiers. This element takes an attribute named ```category```. The category can be set to one of the following: ```bonus```, ```ability score```, ```ability modifier```,  ```saving throw```, or ```skill```. Te value for this element is the modifier name, followed by its value.
