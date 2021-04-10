### 見出し

見出しを作成するには、見出しテキストの前に 1 ~ 6`#` 個の記号を追加します。使用する数によって`#`、見出しのサイズが決まります。

```markdown
# The largest heading
## The second largest heading
###### The smallest heading
```

![レンダリングされた H1、H2、および H6 の見出し](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/headings-rendered.png)

### テキストのスタイル設定

強調は、太字、斜体、または取り消し線で示すことができます。

| スタイル | 構文 | キーボード ショートカット | 例 | アウトプット |
| --- | --- | --- | --- | --- |
| ボールド |`** **` 又は `__ __`| コマンド/コントロール + b | `**This is bold text**` |**これは太字のテキストです**|
| イタリック |`* *` 又は `_ _`| コマンド/コントロール + i | `*This text is italicized*` |*このテキストは斜体* /
| 取り消し線 | `~~ ~~` | | `~~This was mistaken text~~` |~~これは間違ったテキストでした~~|
| 太字およびネストされた斜体 |`** **` そして `_ _`| | `**This text is _extremely_ important**` |**このテキストは _非常に_ 重要です**|
| すべての太字と斜体 | `*** ***` | | `***All this text is important***` |***このテキストはすべて重要です***|

### テキストの引用

テキストは、 で引用できます `>`。

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

![レンダリングインライン コード ブロック](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/inline-code-rendered.png)

コードまたはテキストを独自のブロックにフォーマットするには、三重バックティックを使用します。

<pre>基本的な Git コマンドの一部を次に示します。
```
git status
git add
git commit
```
</pre>

![レンダリングされたコード ブロック](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/code-block-rendered.png)

詳細については、「 」を参照[コード ブロックの作成と強調表示](/articles/creating-and-highlighting-code-blocks)してください。

### リンクス

インライン リンクを作成するには、 のリンク テキストを角かっこ で折り返 `[ ]`し、 かっこで囲んで URL を囲みます `( )`。また、キーボード ショートカットを使用 `command + k` してリンクを作成することもできます。

`This site was built using [GitHub Pages](https://pages.github.com/).`

![レンダリングされたリンク](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/link-rendered.png)

{% チップ %}

**ヒント: ** {% データ variables.product.product_name %} は、有効な URL がコメントに書き込まれると自動的にリンクを作成します。詳細については、「 」を参照[自動リンクされた参照と URL](/articles/autolinked-references-and-urls)してください。

{% エンドヒント %}

### セクションリンク

{% データ再利用可能.リポジトリ.セクションリンク %}

### 相対リンク

{% データ再利用可能.リポジトリ.相対リンク %}

### リスト

または を使用して 1 行以上のテキストの前に配置すると、順序なしのリストを作成できます`-``*`。

```markdown
- George Washington
- ジョン・アダムス
- トーマスジェファーソン
```

![Rendered unordered list](https://raw.githubusercontent.com/github/docs/main/assets/images/help/writing/unordered-list-rendered.png)

To order your list, precede each line with a number.

```markdown
1. James Madison
2. ジェームズ・モンロー
3. ジョン・クインシー・アダムス
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
- "[GitHub での書き込みと書式設定について](/articles/about-writing-and-formatting-on-github)"
- "[高度な書式設定の操作](/articles/working-with-advanced-formatting)"
- "[マスタリング マークダウン](https://guides.github.com/features/mastering-markdown/)"

