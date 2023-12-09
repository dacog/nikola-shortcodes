# nikola-shortcodes

My custom  shortcodes for Nikola Static Site Generator.

These are shortcuts I found useful to follow a DRY principle. 

# Shortcodes

## series-button

Template engine: Jinja2

**Usage**:

```jinja2
{{% series_buttons previous_url="/previous-article" previous_text="Previous Article Title" next_url="/next-article" next_text="Next Article Title" %}}
```
**Important**

- If there is no previous_url, it does not render the previous button.
- If there is no next_url, it does not render the next button.
- If there is no previous_text, it defaults to "Previous in series".
- If there is no next_text, it defaults to "Next in series".

You can use CSS to customize the look-and-feel. The buttons have an id `#series-buttons`

## infobox

Template engine: Jinja2

This shortcode is used to display a infobox with a specific type of content. There is also an _optional_ `disclaimer` shortcode I use when I want to add a disclaimer to an infobox.

**Usage**:

```
{{% infobox type="book" text="This is a book infobox"  disclaimer="true" %}}
```

It supports the following font-awesome icons':

- book
- video
- audio
- link
- quote
- image
- sticky-note

## disclaimer

A really small shortcode to add a disclaimer somewhere on the page.

**Usage:**

`{{% disclaimer %}}`

# License

Use them however you want. Is all under the MIT License.
