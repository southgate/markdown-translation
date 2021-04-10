### 머리글

제목을 만들려면 제목 텍스트 앞에 기호를 1개에서 6개까지`#` 추가합니다. 사용하는 수의 `#`제목 크기가 결정됩니다.

```markdown
# The largest heading
## The second largest heading
###### The smallest heading
```

![렌더링된 H1, H2 및 H6 제목](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/headings-rendered.png)

### 텍스트 스타일링

굵은, 기울임꼴 또는 스트라이크스루 텍스트로 강조를 나타낼 수 있습니다.

| 스타일 | 통사론 | 키보드 바로 가기 | 본보기 | 출력 |
| --- | --- | --- | --- | --- |
| 대담한 |`** **` 또는 `__ __`| 명령/제어 + b | `**This is bold text**` |**이것은 굵은 텍스트입니다**|
| 이탤릭체 |`* *` 또는 `_ _`| 명령/제어 + i | `*This text is italicized*` |*이 텍스트는 기울어진 * /
| 스트라이크스루 | `~~ ~~` | | `~~This was mistaken text~~` |~~이것은 잘못된 텍스트였습니다.~~|
| 대담하고 중첩 된 기울임꼴 |`** **` 그리고 `_ _`| | `**This text is _extremely_ important**` |**이 텍스트는  _매우 _ 중요합니다.**|
| 모든 대담하고 기울임꼴 | `*** ***` | | `***All this text is important***` |***이 모든 텍스트는 중요합니다.***|

### 텍스트 인용

  `>`.

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

![렌더링된 인라인 코드 블록](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/inline-code-rendered.png)

코드 나 텍스트를 고유한 블록으로 포맷하려면 트리플 백틱을 사용합니다.

<pre>일부 기본 Git 명령은 다음과 같습니다.
```
git status
git add
git commit
```
</pre>

![렌더링된 코드 블록](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/code-block-rendered.png)

자세한 내용은 "를[코드 블록 만들기 및 강조 표시](/articles/creating-and-highlighting-code-blocks)참조하십시오."

### 링크

링크 텍스트를 괄호로 래핑한 다음 URL을 괄호로 래핑하여 인라인 링크를 만들 수  `[ ]`있습니다.  `( )` 키보드 바로 가기 키를 사용하여 링크를 만들 수도 `command + k`있습니다.

`This site was built using [GitHub Pages](https://pages.github.com/).`

![렌더링된 링크](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/link-rendered.png)

{% 팁 %}

**팁: ** {% 데이터 variables.product.product_name %} 유효한 URL이 주석에 기록될 때 자동으로 링크를 만듭니다. 자세한 내용은 "를[자동 연결 참조 및 URL](/articles/autolinked-references-and-urls)참조하십시오."

{% 끝팁 %}

### 섹션 링크

{% 데이터 재사용 가능.repositories.section-links %}

### 상대 링크

{% 데이터 재사용 가능.repositories.상대 링크 %}

### 목록

하나 이상의 텍스트 줄이 `-` 있거나 `*`.

```markdown
- George Washington
- 존 애덤스
- 토머스 제퍼슨
```

![Rendered unordered list](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/unordered-list-rendered.png)

To order your list, precede each line with a number.

```markdown
1. James Madison
2. 제임스 먼로
3. 존 퀸시 애덤스
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
- "[GitHub에서 쓰기 및 서식에 대해](/articles/about-writing-and-formatting-on-github)"
- "[고급 서식 으로 작업](/articles/working-with-advanced-formatting)"
- "[마스터링 마크다운](https://guides.github.com/features/mastering-markdown/)"

