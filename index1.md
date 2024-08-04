# Markdown Added Features

Start an indented code block following a paragraph with a blank line and at least four spaces of indentation:

    This is a code block.

    Blank lines between indented lines do not end the code block.

    Here is some HTML:\
    
        <div class="footer">
            2009—2017 JetBrains · All rights reserved
        </div>
        <div class="Header">
            First  markdown Header's
        </div>
       
       
This line of text is not indented. It ends the code block and starts a new paragraph.

   Set multiple lines of code in fenced code blocks.

   ```hs
   -- Point-free style
   fib :: Integer -> Integer
fib = (fibs !!)
where fibs = 0 : scanl (+) 1 fibs

-- Explicit

fib :: Integer -> Integer
fib n = fibs !! n
where fibs = 0 : scanl (+) 1 fibs

```

## Lists in Markdown

Things I need to do today:

1. Fix usability problem
1. Clean up the page
   * Make the headings bigger
   * Make the Color blue of header
1. Push my changes
1. Create code review
   - Describe my changes   
   - Assign reviewers
     - Ask for feedback 

## Tables in Markdown

| Month    | Assignee | Backup |
| ---:| :---:| --- |
| **January** | Dave     | _Steve_  |
| **February** | Gregg    | _Karen_  |
| **March**    | Diane    | _Jorge_  |


### Links in Markdown

[inline Link](https://www.jetbrains.com)

[Inline Link](https://www.jetbrains.com "JetBrains: Development Tools for Professionals and Teams")

[Reference Link][1]

[1]: https://www.jetbrains.com

---

## Auto Links

Both of these URLs are parsed as links:

<https://yourtrack.jetbrains.com/issues>

https://yourtrack.jetbrains.com/issues

Email addresses are also converted into "mailto" links when set in angle brackets:


Email me at: [Rafeeq]

[Rafeeq]: mrafeeq290@gmail.com


***

## Images 

The syntax for images is similar to the syntax for links. To insert an inline image:

- Start the line with an exclamation point ( ! ).
- Wrap the alt text with brackets ( [ ] ).
- Set the image URL and tooltip in parentheses ( ( ) ).

You can also use the reference style for images. To insert an image reference:

- Start the line with an exclamation point ( ! ).
- Wrap the alt text with brackets ( [ ] ).
- Set the image reference in brackets ( [ ] ).
- Define the image reference in another location with the format [ tag ]: image URL "tooltip".

---




    Here's an image link to the Markdown logo on Wikipedia:

    Inline :

![Markdown logo](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/208px-Markdown-mark.svg.png "Markdown")


Reference style:

![Markdown logo][logo]

[logo]: https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/208px-Markdown-mark.svg.png "Markdown"

## Markdown also supports images as links.

Just wrap the entire image reference in brackets then add the target URL in parenthesis after the image reference.
People use this syntax to insert a thumbnail image that links to a video on a video sharing platform.

Here's a reference to the latest video promotion for YouTrack:

[![YouTrack — Maintain Order In A World of Chaos](https://img.youtube.com/vi/rhAunB7UQFQ/sddefault.jpg)](https://www.youtube.com/watch?v=rhAunB7UQFQ)


---

## Backslash Spaces

When you have characters that are parsed as Markdown that you want to show as written, you can escape the character with the backslash (\).

- Backslashes before non-markup characters are shown as backslash characters.
- Escaped characters are treated as regular characters. Their usual meaning in Markdown syntax is ignored.
- Backslash escapes do not work in fenced code blocks, inline code spans, or autolinks.

Here are a few examples of backslash escapes for your referernce.

\**not emphasis**

\`not an inline code span`

\1. not an ordered list

\* not an unordered list

\# not a heading

\This is not a backslash escape - the escaped character is not a markup character.









