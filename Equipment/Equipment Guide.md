Equipment
---
An item is defined using an element named ```item```. Its content can consist of the following elements:
* **name (ABC)**
* **type (LA | MA | HA | S | M | R | A | RD | ST | WD | RG | P | SC | W | G | $)** - *Item Category*
  * **LA** = Light Armor
  * **MA** = Medium Armor
  * **HA** = Heavy Armor
  * **S** = Shield
  * **M** = Melee Weapon
  * **R** = Ranged Weapon
  * **A** = Ammunition
  * **RD** = Rod
  * **ST** = Staff
  * **WD** = Wand
  * **RG** = Ring
  * **P** = Potion
  * **SC** = Scroll
  * **W** = Wondrous Item
  * **G** = Adventuring Gear
  * **$** = Money
* **value (##)** - *Value. Gold value of the item.*
* **weight (##)**
* **text (ABC)** - *Item description. Multiple text elements may be inputted. Each one represents a paragraph. If the ```auto_indent``` attributes is set in the compendium element, paragraphs after the first will automatically indent the first line.*
* **ac (##)** - *Armor Class*
* **strength (##)** - *Strength ability score required to wear armor*
* **stealth (YES | NO)** - *Disadvantage on Stealth checks*
* **dmg1 (D20)** - *One-handed weapon damage*
* **dmg2 (D20)** - *Two-handed weapon damage*
* **dmgType (B | P | S | A | C | F | FC | L | N | PS | R | T)** - *Damage type*
  * **B** = Bludgeoning
  * **P** = Piercing
  * **S** = Slashing
  * **A** = Acid
  * **C** = Cold
  * **F** = Fire
  * **FC** = Force
  * **L** = Lightning
  * **N** = Necrotic
  * **PS** = Poison
  * **R** = Radiant
  * **T** = Thunder
* **property (A, F, H, L, LD, R, S, T, 2H, V)** - *Weapon properties. Multiple values separated by commas allowed*
  * **A** = Ammunition
  * **F** = Finesse
  * **H** = Heavy
  * **L** = Light
  * **LD** = Loading
  * **R** = Reach
  * **S** = Special
  * **T** = Thrown
  * **2H** = Two-handed
  * **V** = Versatile
  * **M** = Martial Weapon
* **range (##/##)** - *Weapon range. (range/long rage)*
* **modifer (ABC [+/-] ##)** - *Modifiers. This element takes an attribute named ```category```. The category can be set to one of the following:*
  * ```bonus```
  * ```ability score```
  * ```saving throw```
  * ```skill```
* **roll (D20)** - *Dice roll formulas. Ability modifiers can be inputted using ````STR```, ```DEX```, ```CON```, ```INT```, ```WIS```, and ```CHA```.

Sample Item - Scale Mail
---
```
<item><name>Scale Mail</name>
  <type>MA</type>
  <ac>14</ac>
  <stealth>1</stealth>
  <weight>45</weight>
</item>
```
Sample Item - +1 Longbow
---
```
<item><name>+1 Longbow</name>
  <type>R</type>
  <dmg1>1d8</dmg1>
  <dmgType>P</dmgType>
  <weight>2</weight>
  <property>A,H,2h</property>
  <range>150/600</range>
  <modifier category="bonus">Weapon Attack +1</modifier>
  <modifier category="bonus">Weapon Damage +1</modifier>
