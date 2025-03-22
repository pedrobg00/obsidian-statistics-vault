<instruction>Generate a hierarchical index for the headings in the text of {activeNote}.
The index should be formatted as a bullet list, maintaining the correct hierarchy (H1, H2, H3, etc.).
Use indentation to reflect the structure of the headings.
IMPORTANT: Each index item **MUST** link to its corresponding heading using the format [[#HEADING]] - example: ## Intro will be - [[#Intro].
Preserve the order of appearance of the headings in the text.
Begin the index with an H2 heading: ## Index.
Index example: 
```
## Index
- [[#Intro]]
...
```
</instruction>

<text>{activeNote}</text>