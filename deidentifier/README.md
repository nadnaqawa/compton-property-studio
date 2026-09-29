# UK Patient Text De-identifier

Two self-contained, offline HTML files that replace UK patient identifiers with labelled placeholders such as `[PERSON 1]` or `[NHS NUMBER 1]`.

| File | For | Layout |
|---|---|---|
| `deidentify-mac.html` | MacBook / any laptop | Original and output side by side, drag-and-drop files, table of findings |
| `deidentify-iphone.html` | iPhone | One column, large buttons, Output/Original tabs, “Redact” bar for selected text |

The detection rules and word lists (SECTION 1 at the top of each file's script) are identical in both files. If you edit one, copy SECTION 1 into the other.

## Opening them

* **Mac:** double-click the file. It opens in Safari or Chrome and works with no internet connection.
* **iPhone:** the Files app's preview cannot run the tool, because it switches JavaScript off. Open it in an app with a built-in browser that can open local HTML files with JavaScript. Alternatively, open it from a private web address that you control. After the page has loaded, nothing you paste leaves the phone.

## Privacy

* A Content-Security-Policy blocks every outgoing connection.
* No cookies or storage are used, and nothing is written to the console.
* Spell-check and grammar add-ons are switched off in the text boxes.
* The list of originals and placeholders is shown on screen only. It is never included in the copied or downloaded output.

Automated redaction can miss things. Always check the output before sharing.
