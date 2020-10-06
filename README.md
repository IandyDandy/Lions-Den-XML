Welcome to Lion's Den XML Repository
---
This is an unofficial repository that contain the information from the Dungeons & Dragons sourcebooks. My version is nuanced to my idea of how the information should be organised.

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

Terminiology
---
The next few  section will teach you the elements needed to define your data. The content for these elements will consist of text, numbers, dice rolls formulas, or otherwise specified values.

Here are a few common ways this tutorial will describe content:
* **ABC** — Any text may be inputted. There are a few characters that cannot be used. **&**, **<**, and **>**. These characters must be replaced with ```&amp;```, **&lt;**, and **&gt;**, respectively.
