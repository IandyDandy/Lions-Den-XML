Bestiary
---
Beast shapes, companions, familiars, etc. are defined using an element named ```monster```. it;s content can consist of the following elements:
* **name (ABC)**
* **size (T | S | M | L | H | G)** - *Creature size*
  * **T** = Tiny
  * **S** = Small
  * **M** = Medium
  * **L** = Large
  * **H** = Huge
  * **G** = Gargantuan
* **type (ABC)** - *Creature type*
* **alignment (ABC)**
* **ac (## (ABC))** - *Armor class followed by armor type enclosed in parenthesis*
* **hp (## (D20))** - *Default Hit Points followed by hit dice formula enclosed in parenthesis*
* **speed (ABC)**
* **str (##)** - *Strength Score*
* **dex (##)** - *Dexterity Score*
* **con (##)** - *Constitution Score*
* **int (##)** - *Intelligence Score*
* **wis (##)** - *Wisdom Score*
* **cha (##)** - *Charisma Score*
* **save (Str ##, Dex ##, ...)** - *Saving throws with modifiers separated by commas*
* **skill ([skill name] ##, [skill name] ## ...)** - *Skills with modifiers separated by commas*
* **vulnerable (ABC)** - *Damage vulnerabilities*
* **resist (ABC)** - *Damage resistances*
* **immune (ABC)** - *Damage immunities*
* **conditionImmune (ABC)** - *Conditional immunities*
* **senses (ABC)**
* **passive (##)** - *Passive perception*
* **languages (ABC)**
* **cr (##)** - *Challenge rating. A number from 1 to 30, or 1/2, 1/4, 1/8, 0, or 00 (denotes CR 0 and 0 XP)*
* **trait, action, reaction, legendary** - *These elements take the following elements as context:*
  * **name (ABC)**
  * **text (ABC)** - *Item description. Multiple text elements may be inputted. Each one represents a paragraph. If the ```auto_indent``` attribute is set in the compendium element, paragraphs after the first will automatically indent the first line.
  * **attack (ABC|##|D20)** - *Attacks consist of three parts, separated by the '|' character. The first part is the attack label, which takes a text string. The second is a number representing the attack roll bonus. The last is the damage roll. All of these parts are optional and can be left empty.

Sample Monster - Lion
---
