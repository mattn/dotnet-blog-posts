---
title: DotNetBlog - Blog Engine Written in Microsoft .NET Core
---

# Summary

This is blog engine that is markdown friendly inspired with Jekyll.

You can write new markdown for the entry. And you can use Liquid language in template. The directory structure is below.

# Directory Structure

```
+- _posts
|   +- 2017-07-12-blog-entry.md
|   +- 2017-07-13-todays-dinner.md
|
+- _layout
|   +- default.html (template for entries)
|   +- post.html    (tempalte for entry)
|
+- _site (public directory)
    +- index.html (default index file)
```

# Configuration

```
title: "Your Blog Title"
base-url: "http://your-blog.example.com"
clone-url: http://your-blog-entry-repository.example.com/repository.git
```

# Update

The blog entry files is managed in external git repository pointed `clone-url`. To update sites, run curl command below.

```
curl -X POST -d test http://your-blog.example.com/pull
```
