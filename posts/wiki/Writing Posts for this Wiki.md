# Writing Posts for this Wiki
## So you want to contribute to the Drauger OS Wiki. But you have no idea where to start. You've come to the right place!

Contributing to the Drauger OS Wiki is designed to be as simple and easy as possible. All you need is knowledge of [Markdown](https://www.markdownguide.org/). And even then, online tools exist ([like this one](https://markdown-editor.github.io/)) that you can write your post in, then copy-paste the resulting text into a plain text file.

Of course, you still need to follow a few simple guidelines:

Post Files
---
A post file is the file which contains the actual text of your post. 

### Post File Name
Make sure the file post is in follows the following format:

> <post-title\>.md

All post files MUST have the `*.md` file extension. This is case-sensitive, and mandatory. Spaces are allowed in the name. Also, the actual name of the post file must be the same as the name of your post.

For example:

The title of this post is "**Writing Posts for this Wiki**". So, the name of this post's post file is:

> Writing Posts for this Wiki.md

### Post File Formatting
Post files must be formatted in Markdown. HTML is not allowed, except for in the case of the line-break element (`</br>`). Furthermore, the first line of the file must contain the title of the post, prepended with a hashtag (#). Like so:

> \# <post-title\>

The title of this post is "**Writing Posts for this Wiki**". So, the first line of this post's post file is:

> \# Writing Posts for this Wiki

Beyond this, feel free to format your Wiki post how you see fit.

### Post File Location
All post files must be stored in `posts/wiki`

Metadata files
---
Every post must have a metadata file. If submitting your post on [GitHub](https://github.com/drauger-os-development/website), you MUST have this file in your Pull Request, along with your post. If submitting it to another contributor, while strongly advised, it is not necessary to include a metadata file as one will be created for you.

### Metadata File Name
All metadata files must have the same name as the post they belong to. Spaces are allowed.

For example:

The title of this post is "**Writing Posts for this Wiki**". So, the name of this post's metadata file is the same.

### Metadata File Formatting
Metadata files support a very basic format. There are 4 mandatory fields, and 1 optional field. There is also support for a very basic comment syntax.

#### Mandatory Fields
Every metadata file **MUST** have the following fields:

 - SYNOPSIS
 - TAGS
 - AUTHOR
 - WRITTEN
 
All fields take 1 and only 1 line. The values for each tag are separated by a colon (:) and a single space.

##### SYNOPSIS
Your synopsis should be a short (140 character max) description of what your post is about. Longer synopses tend to do better with SEO. So if that is important to you, keep it in mind.

##### TAGS
This should be a comma-delimited list of tags that apply to your post. This list is case insensitive. More tags help users find your post easier. There is no limit to the number of tags you may have.

##### AUTHOR
Put your name, or the author's name, in this field. If multiple people wrote this post, they should be in a comma-delimited list.

##### WRITTEN
When you wrote your post. If it took you several days to write it, then opt for the day you finished it. The date format you must use is actually very specific:

> YYYY - MM - DD

That is, the full 4 digit year, the 2 digit month, and the 2 digit day.

#### Optional Fields
These fields are not necessary, but can provide more context to users.

##### EDITOR
This field works exactly like the AUTHOR field. However, it denotes who edited the post. 

#### Comments
Comments take up an entire line, with the first character on the line being a hashtag (#).

For example:

> \# These are comments in a metadata file. It looks the same as the title line on markdown files

> \# But, because they are in a metadata file, they have a different meaning.


#### Example Metadata file

> \# Metadata file for test wiki post </br>
> \# shell-script style comments are supported. But, only for entire lines </br>
> \# all keys and values MUST be seperated by a colon (:) and a SINGLE space. </br>
> </br>
> \# SYNOPSIS: the text to show to the user as a synopsis of a post. If this is not set, the first sentence of the post will be used. </br>
> SYNOPSIS: This is a test wiki post to ensure everything is showing up, working, and rendering correctly. </br>
> </br>
> \# TAGS: comma-delimited list of tags that apply to this post </br>
> TAGS: test </br>
> </br>
> \# AUTHOR: comma-delimited list of authors of the post </br>
> AUTHOR: Thomas Castleman </br>
> </br>
> \# EDITOR: comma-delimited list of editors of this post. This entry is optional. </br>
> EDITOR: Thomas Castleman </br>
> </br>
> \# WRITTEN: when the post was written, must be in the format YYYY - MM - DD </br>
> \# e.g.: </br>
> \# June 28th, 2022     ->  2022 - 06 - 28 </br>
> \# October 19th, 1978  ->  1978 - 10 - 19 </br>
> \# January 9th, 2145   ->  2145 - 01 - 09 </br>
> \# December 2nd, 2010  ->  2010 - 12 - 02 </br>
> WRITTEN: 2022 - 06 - 28 </br>

### Metadata File Location
All metadata files must be stored in `posts-meta/wiki`.