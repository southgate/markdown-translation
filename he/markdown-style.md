### כותרות

כדי ליצור כותרת, הוסף סימן אחד עד שישה`#` סימנים לפני טקסט הכותרת. מספר הכותרות `#`שבו תשתמש יקבע את גודל הכותרת.

```markdown
# The largest heading
## The second largest heading
###### The smallest heading
```

![הכותרות המעובדות H1, H2 ו- H6](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/headings-rendered.png)

### עיצוב טקסט

באפשרותך לציין הדגשה באמצעות טקסט מודגש, נטוי או קו חוצה.

| סגנון | תחביר | קיצור מקשים | דוגמה | פלט |
| --- | --- | --- | --- | --- |
| מודגש |`** **` או `__ __`| פקודה/פקד + b | `**This is bold text**` |**זהו טקסט מודגש**|
| נטוי |`* *` או `_ _`| פקודה/פקד + i | `*This text is italicized*` |*טקסט זה הוא הטיה * /
| קו חוצה | `~~ ~~` | | `~~This was mistaken text~~` |~~זה היה טקסט שגוי~~|
| מודגש ונועז מקונן |`** **` ו `_ _`| | `**This text is _extremely_ important**` |**טקסט זה _ חשוב_ ביותר**|
| כולם נועזים ונועזים | `*** ***` | | `***All this text is important***` |***כל הטקסט הזה חשוב***|

### ציטוט טקסט

באפשרותך לצטט טקסט באמצעות  `>`.

```markdown
In the words of Abraham Lincoln:

> Pardon my French
```

![Rendered quoted text](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/quoted-text-rendered.png)

{% tip %}

**Tip:** When viewing a conversation, you can automatically quote text in a comment by highlighting the text, then typing `r`. You can quote an entire comment by clicking {% octicon "kebab-horizontal" aria-label="The horizontal kebab icon" %}, then **Quote reply**. For more information about keyboard shortcuts, see "[Keyboard shortcuts](/articles/keyboard-shortcuts/)."

{% endtip %}

### Quoting code

You can call out code or a command within a sentence with single backticks. The text within the backticks will not be formatted.

```markdown
Use `git status` to list all new or modified files that haven't yet been committed.
```

![בלוק קוד מוטבע מעובד](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/inline-code-rendered.png)

כדי לעצב קוד או טקסט לבלוק נפרד משלו, השתמש בקווים אחוריים משולשים.

<pre>חלק מהפקודות הבסיסיות של Git הן:
```
git status
git add
git commit
```
</pre>

![בלוק קוד מעובד](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/code-block-rendered.png)

לקבלת מידע נוסף, ראה "[יצירה והדגשה של גושי קוד](/articles/creating-and-highlighting-code-blocks)."

### קישורים

באפשרותך ליצור קישור מוטבע על-ידי גלישת טקסט קישור בסוגריים מרובעים  `[ ]`ולאחר מכן גלישת כתובת ה- URL בסוגריים  `( )`. באפשרותך גם להשתמש בקיצור המקשים `command + k`כדי ליצור קישור.

`This site was built using [GitHub Pages](https://pages.github.com/).`

![קישור מעובד](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/link-rendered.png)

{% עצה %}

**עצה: ** {% נתונים variables.product.product_name %} יוצרים קישורים באופן אוטומטי כאשר כתובות URL חוקיות נכתבות בהערה. לקבלת מידע נוסף, ראה "[הפניות וכתובות URL עם קישור אוטומטי](/articles/autolinked-references-and-urls)."

{% תיאור סיום %}

### קישורי מקטעים

{% נתונים הניתנים לשימוש חוזר.מאגרים.מקטע-קישורים %}

### קישורים יחסיים

{% נתונים הניתנים לשימוש חוזר.מאגרים.קישורים יחסיים %}

### רשימות

באפשרותך ליצור רשימה לא מסודרת על-ידי קדם לשורת טקסט אחת או יותר עם `-`או  `*`.

```markdown
- George Washington
- ג'ון אדמס
- תומאס ג'פרסון
```

![Rendered unordered list](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/unordered-list-rendered.png)

To order your list, precede each line with a number.

```markdown
1. James Madison
2. ג'יימס מונרו
3. ג'ון קווינסי אדמס
```

![Rendered ordered list](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/ordered-list-rendered.png)

#### Nested Lists

You can create a nested list by indenting one or more list items below another item.

To create a nested list using the web editor on {% data variables.product.product_name %} or a text editor that uses a monospaced font, like [Atom](https://atom.io/), you can align your list visually. Type space characters in front of your nested list item, until the list marker character (`-` or `*`) lies directly below the first character of the text in the item above it.

```markdown
1. First list item
   - First nested list item
     - Second nested list item
```

![Nested list with alignment highlighted](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/nested-list-alignment.png)

![List with two levels of nested items](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/nested-list-example-1.png)

To create a nested list in the comment editor on {% data variables.product.product_name %}, which doesn't use a monospaced font, you can look at the list item immediately above the nested list and count the number of characters that appear before the content of the item. Then type that number of space characters in front of the nested list item.

In this example, you could add a nested list item under the list item `100. First list item` by indenting the nested list item a minimum of five spaces, since there are five characters (`100. `) before `First list item`.

```markdown
100. First list item
     - First nested list item
```

![List with a nested list item](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/nested-list-example-3.png)   

You can create multiple levels of nested lists using the same method. For example, because the first nested list item has seven spaces (`␣␣␣␣␣-␣`) before the nested list content `First nested list item`, you would need to indent the second nested list item by seven spaces.

```markdown
100. First list item
     - First nested list item
       - Second nested list item
```

![List with two levels of nested items](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/nested-list-example-2.png)    

For more examples, see the [GitHub Flavored Markdown Spec](https://github.github.com/gfm/#example-265).

### Task lists

{% data reusables.repositories.task-list-markdown %}

If a task list item description begins with a parenthesis, you'll need to escape it with `\`:

`- [ ] \(Optional) Open a followup issue`

For more information, see "[About task lists](/articles/about-task-lists)."

### Mentioning people and teams

You can mention a person or [team](/articles/setting-up-teams/) on {% data variables.product.product_name %} by typing `@` plus their username or team name. This will trigger a notification and bring their attention to the conversation. People will also receive a notification if you edit a comment to mention their username or team name. For more information about notifications, see {% if currentVersion == "free-pro-team@latest" or currentVersion ver_gt "enterprise-server@2.20" or currentVersion == "github-ae@latest" %}"[About notifications](/github/managing-subscriptions-and-notifications-on-github/about-notifications){% else %}"[About notifications](/github/receiving-notifications-about-activity-on-github/about-notifications){% endif %}."

`@github/support What do you think about these updates?`

![Rendered @mention](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/mention-rendered.png)

When you mention a parent team, members of its child teams also receive notifications, simplifying communication with multiple groups of people. For more information, see "[About teams](/articles/about-teams)."

Typing an `@` symbol will bring up a list of people or teams on a project. The list filters as you type, so once you find the name of the person or team you are looking for, you can use the arrow keys to select it and press either tab or enter to complete the name. For teams, enter the @organization/team-name and all members of that team will get subscribed to the conversation.

The autocomplete results are restricted to repository collaborators and any other participants on the thread.

### Referencing issues and pull requests

You can bring up a list of suggested issues and pull requests within the repository by typing `#`. Type the issue or pull request number or title to filter the list, and then press either tab or enter to complete the highlighted result.

For more information, see "[Autolinked references and URLs](/articles/autolinked-references-and-urls)."

### Referencing external resources

{% data reusables.repositories.autolink-references %}

### Content attachments

Some {% data variables.product.prodname_github_app %}s provide information in {% data variables.product.product_name %} for URLs that link to their registered domains. {% data variables.product.product_name %} renders the information provided by the app under the URL in the body or comment of an issue or pull request.

![Content attachment](https://raw.githubusercontent.com/github/docs/main/assets/images/github-apps/content_reference_attachment.png)

To see content attachments, you must have a {% data variables.product.prodname_github_app %} that uses the Content Attachments API installed on the repository.{% if currentVersion == "free-pro-team@latest" %} For more information, see "[Installing an app in your personal account](/articles/installing-an-app-in-your-personal-account)" and "[Installing an app in your organization](/articles/installing-an-app-in-your-organization)."{% endif %}

Content attachments will not be displayed for URLs that are part of a markdown link.

For more information about building a {% data variables.product.prodname_github_app %} that uses content attachments, see "[Using Content Attachments](/apps/using-content-attachments)."

### Using emoji

You can add emoji to your writing by typing `:EMOJICODE:`.

`@octocat :+1: This PR looks great - it's ready to merge! :shipit:`

![Rendered emoji](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/emoji-rendered.png)

Typing `:` will bring up a list of suggested emoji. The list will filter as you type, so once you find the emoji you're looking for, press **Tab** or **Enter** to complete the highlighted result.

For a full list of available emoji and codes, check out [the Emoji-Cheat-Sheet](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md).

### Paragraphs

You can create a new paragraph by leaving a blank line between lines of text.

### Ignoring Markdown formatting

You can tell {% data variables.product.product_name %} to ignore (or escape) Markdown formatting by using `\` before the Markdown character.

`Let's rename \*our-new-project\* to \*our-old-project\*.`

![Rendered escaped character](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/escaped-character-rendered.png)

For more information, see Daring Fireball's "[Markdown Syntax](https://daringfireball.net/projects/markdown/syntax#backslash)."

### Further reading

- [{% data variables.product.prodname_dotcom %} Flavored Markdown Spec](https://github.github.com/gfm/)
- "[אודות כתיבה ועיצוב ב- GitHub](/articles/about-writing-and-formatting-on-github)"
- "[עבודה עם עיצוב מתקדם](/articles/working-with-advanced-formatting)"
- "[שליטה בסימון](https://guides.github.com/features/mastering-markdown/)"

