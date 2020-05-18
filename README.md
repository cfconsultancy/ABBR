# ABBR
ABBR for tinymce 5

The abbr element is used along with a title attribute to associate a full-text explanation with an abbreviation or acronym. 
Website visitors do not see the text in the title attribute, but browsers, search engines, and assistive technologies do use this information.
You can also click or hover the abbr tag to see the explanation.

![Image abbr](https://github.com/cfconsultancy/ABBR/blob/master/abbr.jpg)

Install


Upload the map abbr to your tinymce/plugin directory

Now add abbr to your tinymce.init - plugins: and your toolbar

Since this ABBR html tag doesn't support touch devices you can add the following css snippet to you're default css file:

```
/* abbr */
abbr[title]:after
{
    content: " (" attr(title) ")";
}

@media screen and (min-width: 1025px)
{
    abbr[title]
    {
        border-bottom: 1px dashed #ADADAD;
        cursor:help;
    }

    abbr[title]:after
    {
        content: "";
    }
}
```

Code improvements are welcome

https://www.cfconsultancy.nl/free-tinymce-5-abbr-plugin.html

