# Zettelkasten

The German word Zettelkasten literally translates to "box of notes".
The idea is to build an interconnected database of notes that serves as a knowledge base.
The concept is rather old already (check [here](https://en.wikipedia.org/wiki/Zettelkasten)). An especially famous example of a Zettelkasten is the collection by the sociologist [Niklas Luhmann](https://en.wikipedia.org/wiki/Niklas_Luhmann).

# Concept
A Zettelkasten is a collection of short notes that explain concepts. This Zettelkasten is focused on, but not strictly limited to, quantum physiscs and adjacent fields.

## Major rules of the Zettelkasten
In order to make this repository as useful as possible to many people, please adhere to the following rules:

1. Keep notes short.
2. Keep notes simple.  
If the concept needs more explanation, consider splitting it in multiple (linked) notes.
The idea of a note is not to show that you know, but to explain it to others.
3. Be precise. 
4. Add references to relevant paper or reviews.
5. Use tags.
Add tags to your notes to add them to larger groups. If you add new tags, make sure that there is no almost identical tag.
6. Link notes.  
A Zettelkasten only works if notes are linked together such that other people may find them.
7. Reiterate over notes and correct them.  
As areas in the Zettelkasten grow, it might be worth to reorganize notes. This might result in splitting notes up, merging notes or creating summary notes to make other notes easier to reach.

# Tools and Setup
This Zettelkasten is based on [Obsidian](https://obsidian.md) and [git](https://www.git-scm.com).
Obisidan displays markdown notes, manages links between the notes and the tag network. 
It is the main tool to edit, add and manage notes.

We use git to synchronize the notes via github. 
It helps to track changes and make sure that involuntary edits do not propagate to others.

## Obsidian Setup
The folder `vault` is the actual Obsidian vault.
It can be opened in Obsidian to via the Obsidian GUI.
The vault is not chosen to be the main folder of the git repository in order to keep files like this README separate from the markdown notes in the Zettelkasten.

In order to make most of your Obsidian experience, here are some possibly helpful setup steps:

1. Set the template directory  
After opening the vault, you can navigate to the settings (gear symbol in the bottom left corner) and set the template directory.
Navigate to the `Core plugins` and search for `Templates`.
In the settings of the `Templates`, you select the directory `templates` for the template directory.
After closing, you can use `Ctrl+P->Insert Template` to insert the `Note` template for new notes.
It makes working with Obsidian faster and all notes start with the same structure.

2. Setting up the Zotero connection  
Zotero and Obsidian play nice together. 
After enabling community plugins in Obsidian, you can download the plugin `Zotero Integration`.
It needs a bit of setup:
    1. Navigate to the settings of the plugin `Zotero Integration`. 
    Under the section `Citation Formats`, create a new citation format by clicking `Add Citation Format`.
    2. Name it to something that you can remember, e.g. `Zettelkasten Bib`
    3. Choose `Output Format` as `Template`.
    4. Add the following template text
   ```
   {%- for creator in creators %} {%- if creator.name == null %} {{creator.firstName}} {{creator.lastName}} {%- endif -%}, {%- if creator.name %} {{creator.name}} {%- endif -%} {%- endfor %}; {{title}}; ({{date | format("YYYY")}}); {%- if DOI %} [{{DOI}}](https://www.doi.org/{{DOI}}); {%- else %} {%- if url %} [{{url}}]({{url}}); {%- endif %}  {%- endif %}  @{{citekey}} 

   ```
   5. With `Ctrl+P -> Zotero Integration: Zettelkasten Bib`, you can directly enter citations from your Zotero library. In order to adhere to current format of the citation key, it would be nice to set the `betterBibTex` citation key in Zotero to `zotero.clean`.

## Git rules of engagement
Using git with multiple people can lead to a lot of confusion.
To get a bit of structure and ensure a minimal quality of the notes, we have set up a couple of rules for the branches.

1. The `main` branch is protected 
You cannot push to `main`. It can be only changed via pull-requests. 
Please work in your own thematic branch.
If you start working on something, pull `main`, open a new branch with a topical name like `tensor-networks`, commit to it and push it.
If you feel like the notes have come to a good status, generate a pull-request to `main`.
You will have to assign at least one reviewer.
Once the review process is done, the pull request is accepted into the `main` branch.

2. Use reasonable commit messages
Please do not use `misc` or similar as commit messages.
Commit messages are vital to later understand how changes were made.
If all commit messages are the same it is hard to understand what changed.

3. Local branches can be modified
There is a difference between local and global commits.
While commits are local on your computer, you can easily undo and change commits.
Possible commands are `git reset --soft`, `git reset`  or `git rebase -i`.
You do not have to `git revert` local commits.
