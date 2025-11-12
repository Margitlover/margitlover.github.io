#my coding notebook
## Table of Contents
- [Flutter notes](#flutter-notes)
  - [what is flutter? ](#what-is-flutter)
  - [Key Terms and Definitions](#Key-Terms-and-Definitions)
  -  [Layout and Design Widgets](layout-and-design-widgets)
  - [Flutter Definitions with structures](#flutter_definitions)
- [Code Definitions](#code_definitions)
- [Notebook Style Guide](#Markdown-Style-Guide-for-Coding-Notebooks)


## Flutter Notes

### What is Flutter?
- Definition:
- Why is it useful?

---

### Key Terms and Definitions

| Term             | Definition                                      | Example / Notes                          |
|------------------|--------------------------------------------------|-------------------------------------------|
| Widget           |   Basic building block of a flutter app. Everything is a widget|Text,Image,Container,Column  |
| MaterialApp      |      The root of the app. Sets up routes and theme|  Found in main.dart                      |
| Scaffold         |      Provides basic visual layout-like a header, body floating button| Each screen uses it   |
| StatelessWidget  |       a widget that doesn't change               |  Most of the screen files                 |
| StatefulWidget   |       A widget that can change over time         |  Used in MyHomePage()                     |
| Navigator        |      Manages screen transitions                  |  Navigator .pushNamed(context,  '/page'); |
| AppBar           |      Top navigation bar                          |   Title of each page appears here         |
| Column           |      vertical layout                             |                                           |
| Row              |      horizontal layout                           |                                           |
| Container        |      wraps content with padding, margin or color |                                           |
| Text             |      displays text                               |                                           |
| Image.network    |      displays images from a URL                  |                                           |
| padding          |      adds space around a widget                  |                                           |
| Center           |      centers its child                           |                                           |
| main             |      The function that runs the app              |         found in main.dart                |
| Named Routes     |      Predefined paths to navigate between screens|         '/','/page2','/page3',ect         |
---

### Layout and Design Widgets
- How do you center a widget?
- How do you align something to the left or right?
- What widget adds space around content?


## Flutter Definitions with structures

| Term | Definition and Description | Base Structure | Real Life Example | App Example |
|------|----------------------------|----------------|-------------------|-------------|
| Main() | A function that runs when your app starts. It tells Flutter what app to show. | `void main() => runApp(MyApp());` | Turning on phone  | main.dart void main() => runApp(MyPortfolioApp());  |
|MaterialApp| The widget that sets up your whole app’s look and navigation. | `MaterialApp(...)` |setting up accounts  | main.dart return MaterialApp( |
|Scaffold| A widget that gives you the basic layout: background, navigation bar, floating button, etc. | `Scaffold(...)` | A templet  |alt_design_screen.dart return Scaffold(body: ListView(children: dogInfo  |
|Column| A widget that holds and displays your content in a straight line from top to bottom. | `Column(...)` |Using division  | showcase.dart child: Column(children: [ |
|Row   | A widget that shows things side-by-side. | `Row(...)` |every thing related to the term  | infoCard.dart child: Row(children: [ |
|Container| A box that holds other widgets. You can add color, padding, borders, or size. | `Container(...)` | backgroumds to hold things  |home.dart Container(width: 200,height: 200,decoration: BoxDecoration(  |
|Text  | A widget to display text on the screen. | `Text('Hello')` | words |const Text('HI EVERYONE,\nWelcome to the',style: TextStyle(   |
|Image.network| A widget to show an image using a link from the internet. | `Image.network('https://...')` |Pictures  |home.dart child: Image.network('https://placedog.net/640/480?random',fit: BoxFit.cover,),  |
|ElevatedButton| A clickable button that floats above content. You choose what happens when it's clicked. | `ElevatedButton(onPressed: ..., child: ...)` |exposive button  |home.dart ElevatedButton(onPressed: () => Navigator.pushNamed(context, '/background'),child: const Text('Next'),),  |
|onPressed| The code that gets run when a button is tapped or something happens. | `onPressed: () => doSomething()` | everytime that you prees a button +1$  | onPressed: () => Navigator.pushNamed(context, '/showcase'),child: const Text('Next'),), backgroung.dart|
|StatelessWidget| A class that creates widgets that never change. Good for static screens. | `class HomeScreen extends StatelessWidget` | info on welcome page  | class AltDesignScreen extends StatelessWidget { alt_design_screen|
|StatefulWidget | A class for widgets that can change while the app is running. | `class MyWidget extends StatefulWidget` | a game that you play  | not found in app |
|Navigator      | Lets you move from one screen to another using route names. | `Navigator.pushNamed(context, '/about')` | Navigateing through a website |  |
| padding      | Makes space around a widget inside its container. | `Padding(padding: EdgeInsets.all(8.0), child: ...)` | adding some space |  |
|center      | Aligns content in the center of the screen or container. | `Center(child: ...)` | a tital |  |
| wrap     | Automatically puts widgets onto a new line when there's no space. | `Wrap(children: [...])` | going to another line |  |
|@override| This marks a method as one that’s replacing a method in a parent class. | `@override` | Override a rule  |  |
|build      | The special function in every widget that describes what gets drawn on the screen. | `Widget build(BuildContext context) {...}` | Building something |  |
|build      | Required in every widget class to describe what to show. | `build` | Building something |  |
|buildContext   | A variable that helps the widget know where it is and lets it communicate with the app. | `BuildContext context` | what you have previesly done |  |
|Super.key      | A keyword used to pass a value to the parent widget. | `super.key` | emailing someone  |  |
| const     | A keyword that means the value won't change and is set once. | `const` | something that wont change |  |




























## Code Definitions

| Term | Definition | Base Structure / Syntax | Real Life Example | App Example |
|------|------------|--------------------------|-------------------|-------------|
| Algorithms | Define step by step processes to follow when completing a task or solving a problem | no syntax | Make a grilled cheese | Verify user |
| Sequencing | Define an order for when steps in an algorithm are completed | Follows 1, 2, 3 | which step comes first in making a grilled cheese | Get bread, add butter, add cheese |
|variable| A named container used to store a value that may change. | `var x = 5;` | student age is 15 | main.dart title: 'TSA Portfolio', |
|Constant| A fixed value that cannot change once set. | `const PI = 3.14;` |The Apps Tital  | padding: const EdgeInsets.all(12), |
|Data Type| The kind of value a variable holds, like numbers or text. | `int`, `String`, `bool` |Age vs Name| const SizedBox(width: 12), |
|String| A sequence of characters used to represent words or text. | `"Hello World"` |Sentisis  |title: 'TSA Portfolio', |
|Integer| Whole number values. | `int age = 16;` |grades  | fontSize: 28, home.dart |
|Double |Number values with decimals. | `double age = 16.2;` |any use o calculation  | vertical: 8.0 infocard |
|Boolean| A value that can be true or false. | `bool isLoggedIn = false;` |Are dogs real  |  debugShowCheckedModeBanner: false, main.dart |
|List  | A collection of values in a specific order. | `List<String> names = [];` |To Be organized  | final List<Map<String, String>> dogInfo = [{"image": "https://placedog.net/550","text": "This is Luna, a cheerful retriever who loves playing fetch.",}, alt_design_screen |
|Null  | A special value that means “nothing.” | `String? name = null;` |not no what game is called untill started  | final String imageUrl; = null infocard.dart |
|Function| A reusable block of code that performs an action. | `void sayHi() { print("Hi"); }` |jumping in a game | not found in app |
|Parameter| The information passed into a function to change how it works. | `greet(String name)` |  |  |
|Return| The result a function gives back. | `return total;` |  |  |
|Scope | Where a variable or function can be used. | (No set syntax — concept-based) |  |  |
|Class | Blueprint for creating objects with specific structure and behavior. | `class Dog {}` |  |  |
|object| A specific version of a class. | `Dog myDog = Dog();` |  |  |
|Property A variable that belongs to a class/object. | `String name;` |  |  |
|Method| A function that belongs to a class. | `void bark() {}` |  |  |
|Constructor| A special function used to set up a class when it’s created. | `Dog(this.name);` |  |  |
|Abstarction| Hiding the inner workings of code so users only interact with what they need. | (Concept — not specific code) |  |  |
|Override| Changing how a built-in or inherited function behaves. | `@override` |  |  |
|Void    | A function that does not return a value. | `void printMessage() {}` |  |  |
|Scanner|Creates a scanner object to take input from user |Scanner in = new scanner(System.in);  |  |  |
|impor scanner  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|overloded methods/function or constructor | uses the same name, but has different parameters | pizza(), pizza(String toppings) 2
constructors, first is a defalt cheese pizza, 2nd has 1 topping |||
| dot notation | methods are called on objects using a dot after the object name | object.method(value);|||
| Concatenate | to combine strings with other strings and/or variables | strings greeting = "hello" + "My name is " + name ". "; |||


## Markdown Style Guide for Coding Notebooks

Follow this guide to keep your coding notebook **clear, consistent, and professional**.  
This ensures your notes are easy for you (and others) to read later.

---

## 🔹 Headings
**When to use:** Organize your notebook into sections (like days, topics, or projects).  
- `#` for the notebook title (use once at the top).  
- `##` for each day or major topic.  
- `###` for subsections (like "Notes", "Practice", "Reflections").  

✅ Example:


# My Coding Notebook
## Day 1
### Notes
### Practice
🔡 Text Formatting
When to use: Highlight important ideas or add emphasis.

Use bold for key terms or definitions.

Use italic for emphasis or side comments.

Use inline code for keywords, functions, or commands.

✅ Example:

**Class** = a blueprint for objects  
*Remember:* always test your code  
Use `System.out.println()` to print
💻 Code Blocks
When to use: Anytime you write multiple lines of code.

Inline code for short snippets.

Fenced code blocks with language for full examples.


✅ Example:


```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```
🧾 Lists
When to use: Organize steps, notes, or key points.

Numbered lists for sequences or steps.

Bulleted lists for unordered ideas.

✅ Example:

1. Define the class
2. Write the main method
3. Test your program

- Variables
- Loops
- Conditionals
✅ Checklists
When to use: Track progress on assignments or tasks.

✅ Example:

- [x] Complete coding warm-up
- [ ] Finish project draft
- [ ] Reflect on learning
➡️ Blockquotes
When to use: Call out notes, reminders, or teacher comments.

✅ Example:

> 💡 Remember: Loops repeat code until a condition is false.
📊 Tables
When to use: Compare values, track progress, or organize data neatly.

✅ Example:

| Task        | Status   | Notes          |
|-------------|----------|----------------|
| Homework 1  | Done ✅  | Submitted      |
| Homework 2  | Pending  | Needs review   |
🔗 Links & Images
When to use: Add references, resources, or visuals.

✅ Example:

[Java Docs](https://docs.oracle.com/javase/8/docs/api/)  
![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)
📂 Collapsible Sections
When to use: Hide solutions, extended notes, or extra details.

✅ Example:

<details>
  <summary>Click to reveal solution</summary>
  
System.out.println("Answer: 42");

</details>
📝 Footnotes
When to use: Add references or side notes without cluttering the page.

✅ Example:

This concept is related to object-oriented programming.[^1]

[^1]: See "Objects and Classes" in your textbook.
🎯 Style Rules
Consistency matters more than creativity

Always use headings to structure your notes.

Always use code blocks for multi-line code.

Clarity first

Bold key terms.

Use lists instead of long sentences when outlining steps.

Professional tone

Don’t mix casual notes with formal work in the same section.

Use blockquotes for reflections or teacher feedback.

Track your learning

Use checklists to mark what’s done.

Use collapsible sections if you want to hide answers until review time.

✅ Bottom Line:

Headings = Structure

Bold/Italic = Emphasis

Code blocks = Code

Lists = Steps/Ideas

Tables = Organization

Checklists = Progress

Blockquotes = Notes/Tips

Collapsible = Hide/Show detail

Keep it simple, consistent, and clear.
