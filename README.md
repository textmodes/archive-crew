# Artscene crews

The crews are saved in [YAML](http://yaml.org/) format.

## File names

The file name is the *slugified* version of the crew name and should be a
URL-safe name, so that:

-    The name is converted to lower case
-    All "unsafe" characters are converted to a space. Valid characters are
     `0..9`, `a..z`, `.!`
-    Multiple spaces are converted to a single space
-    Leading and trailing spaces are removed
-    Spaces are converted to dots `.`

## Data fields

### `name`

The `name` field contains the human-readable crew name and is free form.

### `site` (optional)

The `site` field is optional and contains the crew's website or main
social profile URL.

### `alias` (optional)

The `alias` field is optional and contains the human-readable crew name
aliases, which may contain abbreviations and alternate name spellings. The
field is a list of strings.

### `biography` (optional)

The `biography` field is optional and can be used to tell about a crew's
history, in [Markdown](https://daringfireball.net/projects/markdown) format. In
addition, you may use `@name` to link to artists and `#name` to link to crews
in the text.

The text should word-wrap at the 79th column, so that it would also display
properly on terminal devices, such as a BBS.

### `pack`

The `pack` field is a list of lower case pack names this crew has released or
the crew took part in. Please retain alphabetical order, because that is more
easy for humans when they are performing edits.
