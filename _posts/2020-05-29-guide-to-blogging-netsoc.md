---
layout: page
title: "Guide to adding posts to the Netsoc blog"
author: "Rajit Banerjee"
date: 2020-05-29
---

## Welcome to the Netsoc blog!

Here's how you can add your own article to the Netsoc website in 5 simple steps:

-   Fork the homepage [repository](https://github.com/ucdnetsoc/homepage).
-   Add your Markdown file under `./_posts` following the naming convention: `YYYY-MM-DD-post_name.md`
-   Your file should include the following front matter:

```
---
layout: page
title: <title in quotes>
author: <author in quotes>
date: <YYYY-MM-DD>
---
```

For instance, for this post:

```
---
layout: page
title: "Guide to adding posts to the Netsoc blog"
author: "Rajit Banerjee"
date: 2020-05-29
---
```

-   Add any required images/files (that may be linked in the post) under `./assets`
-   Commit changes, create a pull request, and wait for your post to be approved!
