Welcome to Lion's Den XML Repository
---
This is an unofficial repository meant for the Lion's Den series of apps, that contain the information from the Dungeons & Dragons sourcebooks. My version is nuanced to my idea of how the information should be organised.

The Basics
---
XML is a markup language, much like HTML. It was designed to describe date. The most basic units of an XML documents are called **elements**. Elements consist of three parts: start tag, content, and end tag. The start tag is represented using ```<abc>```, while the end tag is represented using ```</abc>```. The "abc" represents the element name, which is placed between '<' and '>' characters. Content describing the element is placed between the start and end tags. For example, ```<name>Gandalf</name>```, is an element named "name" and is set to "Gandalf".

Element may be embedded with each other. In the example below, the "people" element takes a list of name elements as its content.
```
<people>
  <name>Gandalf</name>
  <name>Saruman</name>
</people>
```

Some elements may also specify **attributes**, which further define an element. Attributes are placed within the start tag and consist of a name / value pair. For example, ```<name color="grey">Gandalf</name>```, the name element from before now has an attribute named "color" with its value set to "grey".

These are the basics you'll need to make your Fight Club import file. You'll see the terminology learned throughout the rest of the tutorial.

Terminology
---
The next few  section will teach you the elements needed to define your data. The content for these elements will consist of text, numbers, dice rolls formulas, or otherwise specified values.

Here are a few common ways this tutorial will describe content:
* **ABC** — Any text may be inputted. There are a few characters that cannot be used. **&**, **<**, and **>**. These characters must be replaced with ```&amp;```, ```&lt;```, and ```&gt;```, respectively.
* **###** — Any number may be inputted. Only unformatted numbers are acceptable, meaning remove any commas and other characters, except for dots for decimal point numbers.
* **D20** — A dice roll formula. For example, "*1d10+5*", "*5d6*", or "*3d3+1d7-2*". Use 'd' to denote a die. = and - operators are acceptable. Remove any white spaces.
* The | denotes that the element can take a specific value from the given list. Acceptable values are separated the | character.
* Some elements take multiple values. Acceptable values are separated by commas.

For example, when you see "name(ABC)' throughout the tutorial, that says the element's name is "name" and it takes text as its content, as in ```<name>Gandalf the Grey</name>```. "classes(ABC, ABC, ...)" says the classes element takes multiple text strings, as in ```<classes>Fighter, Wizard</classes>```.

Getting Started
---
Create a file with an XML extension (i.e. compendium.xml). Open the file in any text editor. This file must be start with the following line: ```<?xml version="1.0' encoding="UTF-8"?>```. This line defines the XML document that it is read into the app.

The first element needed is named "compendium". The element must contain an attribute named "version" with its value set to "5". The content for the **compendium** element will be your lists of spells, items, creatures, races, classes, backgrounds, and / or feats.

The shell of your document will look like this:
```
<?xml version="1.0" encoding="UTF-8"?>
<compendium version="5">
  Content goes here
</compendium>
```

The **compendium** element may optionally take the ```auto_indent``` attribute with a value set to "YES" or "NO". Yes means certain text descriptions elements will automatically indent paragraphs.
