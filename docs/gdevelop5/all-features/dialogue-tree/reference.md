# Dialogue Tree Reference

Handle dialogue trees, made using Yarn Spinner. Useful to make complex dialogues with multiple choices. The Yarn Spinner editor is embedded in GDevelop so you can edit your dialogues without leaving GDevelop. [Read more explanations about it.](/gdevelop5/all-features/dialogue-tree)

## Actions

**Clear dialogue state**  
Clear dialogue state. This resets all dialogue state accumulated by the player choices. Useful when the player is starting a new game.

**Complete clipped text scrolling**  
Complete the clipped text scrolling. Use this action whenever you want to skip scrolling.

**Confirm selected option**  
Set the selected option as confirmed, which will validate it and go forward to the next node. Use other actions to select options (see "select next option" and "Select previous option").

**Go to the next dialogue line**  
Go to the next dialogue line. Use this to advance to the next dialogue line when the player presses a button.

**Load dialogue tree from a JSON file**  
Load a dialogue data object - Yarn JSON format, stored in a JSON file. Use this command to load all the Dialogue data at the beginning of the game.

??? quote "See parameters"

    - Parameter 1 (jsonResource): JSON file that holds the Yarn JSON data

    > Technical note: parameter 0 are internal parameters handled by GDevelop.

**Load dialogue tree from a scene variable**  
Load a dialogue data object - Yarn JSON format, stored in a scene variable. Use this command to load all the Dialogue data at the beginning of the game.

??? quote "See parameters"

    - Parameter 0 (🗄️ Scene variable): Scene variable that holds the Yarn JSON data

**Load dialogue state**  
Load dialogue state. Use this to restore dialogue state, if you have stored in a variable before with the "Save state" action.

??? quote "See parameters"

    - Parameter 0 (🗄️ Global variable): Global Variable

**Save dialogue state**  
Save dialogue state. Use this to store the dialogue state into a variable, which can later be used for saving the game. That way player choices can become part of the game save.

??? quote "See parameters"

    - Parameter 0 (🗄️ Global variable): Global Variable

**Scroll clipped text**  
Scroll clipped text. Use this with a timer and "get clipped text" when you want to create a typewriter effect. Every time the action runs, a new character appears from the text.

**Select next option**  
Select next option (add 1 to selected option number). Use this when the dialogue line is of type "options" and the player has pressed a button to change selected option.

**Select option by number**  
Select option by number. Use this when the dialogue line is of type "options" and the player has pressed a button to change selected option.

??? quote "See parameters"

    - Parameter 0 (🔢 Number): Option index number

**Select previous option**  
Select previous option (subtract 1 from selected option number). Use this when the dialogue line is of type "options" and the player has pressed a button to change selected option.

**Set dialogue state boolean variable**  
Set dialogue state boolean variable. Use this to set a variable that the dialogue data is using.

??? quote "See parameters"

    - Parameter 0 (string): State variable name
    - Parameter 1 (❓ True or False): New value

**Set dialogue state number variable**  
Set dialogue state number variable. Use this to set a variable that the dialogue data is using.

??? quote "See parameters"

    - Parameter 0 (string): State variable name
    - Parameter 1 (🔢 Number): New value

**Set dialogue state string variable**  
Set dialogue state string variable. Use this to set a variable that the dialogue data is using.

??? quote "See parameters"

    - Parameter 0 (string): State variable name
    - Parameter 1 (string): New value

**Start dialogue from branch**  
Start dialogue from branch. Use this to initiate the dialogue from a specified branch.

??? quote "See parameters"

    - Parameter 0 (string): Dialogue branch

**Stop running dialogue**  
Stop the running dialogue. Use this to interrupt dialogue parsing.

## Conditions

**Compare dialogue state boolean variable**  
Compare dialogue state variable. Use this to trigger game events via dialogue variables.

??? quote "See parameters"

    - Parameter 0 (string): State variable
    - Parameter 1 (❓ True or False): Equal to

**Compare dialogue state number variable**  
Compare dialogue state number variable. Use this to trigger game events via dialogue variables.

??? quote "See parameters"

    - Parameter 0 (string): State variable
    - Parameter 1 (🔢 Number): Equal to

**Compare dialogue state string variable**  
Compare dialogue state string variable. Use this to trigger game events via dialogue variables.

??? quote "See parameters"

    - Parameter 0 (string): State variable
    - Parameter 1 (string): Equal to

**Current dialogue branch contains a tag**  
Check if the current dialogue branch contains a specific tag. Tags are an alternative useful way to <<commands>> to drive game logic with the dialogue data.

??? quote "See parameters"

    - Parameter 0 (string): tag name

**Current dialogue branch title**  
Check if the current dialogue branch title is equal to a string. Use this to trigger game events when the player has visited a specific dialogue branch.

??? quote "See parameters"

    - Parameter 0 (string): title name

**Dialogue has branch**  
Check if the dialogue has a branch with specified name. Use this to check if a dialogue branch exists in the loaded dialogue data.

??? quote "See parameters"

    - Parameter 0 (string): Branch name

**Clipped text has completed scrolling**  
Check if the clipped text scrolling has completed. Use this to prevent the player from going to the next dialogue line before the typing effect has revealed the entire text.

**Has selected option changed**  
Check if a selected option has changed when the current dialogue line type is options. Use this to detect when the player has selected another option, so you can re-draw where the selection arrow is.

**Command is called**  
Check if a specific Command is called. If it is a <<command withParameter>>, you can even get the parameter with the CommandParameter expression.

??? quote "See parameters"

    - Parameter 0 (string): Command String

**Dialogue line type**  
Check if the current dialogue line line is one of the three existing types. Use this to set what logic is executed for each type.  
The three types are as follows:
- text: when displaying dialogue text.
- options: when displaying [[branching/options]] for dialogue choices.
-command: when <<commands>> are triggered by the dialogue data.

??? quote "See parameters"

    - Parameter 0 (🔤 String): type (one of: "text", "options", "command")

**Dialogue is running**  
Check if the dialogue is running. Use this to for things like locking the player movement while speaking with a non player character.

**Branch title has been visited**  
Check if a branch has been visited

??? quote "See parameters"

    - Parameter 0 (string): branch title

## Expressions

| Expression | Description |  |
|-----|-----|-----|
| `DialogueTree::BranchTag(number)` | Get a tag of the current branch of the running dialogue via its index ||
| | _🔢 Number_ | Tag Index Number |
| `DialogueTree::BranchTags()` | Get the tags of the current branch of the running dialogue ||
| `DialogueTree::BranchText()` | Get the full raw text of the current branch ||
| `DialogueTree::BranchTitle()` | Get the title of the current branch of the running dialogue ||
| `DialogueTree::ClippedLineText()` | Get dialogue line text clipped by the typewriter effect. Use the "Scroll clipped text" action to control the typewriter effect. ||
| `DialogueTree::CommandParameter(number)` | Get the parameters of a command call - <<command withParameter anotherParameter>> ||
| | _🔢 Number_ | parameter Index Number _Optional_. |
| `DialogueTree::CommandParametersCount()` | Get the number of parameters in the currently passed command ||
| `DialogueTree::HorizontalOptionsList(string)` | Get the text of all available options from an options line type as a horizontal list. You can also pass the selected option's cursor string, which by default is -> ||
| | _string_ | Options Selection Cursor |
| `DialogueTree::LineText()` | Returns the current dialogue line text ||
| `DialogueTree::Option(number)` | Get the text of an option from an options line type, using the option's Number. The numbers start from 0. ||
| | _🔢 Number_ | Option Index Number |
| `DialogueTree::OptionsCount()` | Get the number of options in an options line type ||
| `DialogueTree::SelectedOptionIndex()` | Get the number of the currently selected option. Use this to help you render the option selection marker at the right place. ||
| `DialogueTree::TagParameter(number)` | Get parameter from a Tag found by the branch contains tag condition ||
| | _🔢 Number_ | parameter Index Number _Optional_. |
| `DialogueTree::Variable(string)` | Get the number stored in a dialogue state variable ||
| | _string_ | Dialogue state variable name |
| `DialogueTree::VariableString(string)` | Get the string stored in a dialogue state variable ||
| | _string_ | Dialogue state variable name |
| `DialogueTree::VerticalOptionsList(string)` | Get the text of all available options from an options line type as a vertical list. You can also pass the selected option's cursor string, which by default is -> ||
| | _string_ | Options Selection Cursor |
| `DialogueTree::VisitedBranchTitles()` | Get a list of all visited branches ||



---

The Dialogue Tree extension is always installed in all GDevelop projects: there is no need to add it from the Project Manager.

*This page is an auto-generated reference page about the **Dialogue Tree** feature of [GDevelop, the open-source, cross-platform game engine designed for everyone](https://gdevelop.io/).* Learn more about [all GDevelop features here](/gdevelop5/all-features).