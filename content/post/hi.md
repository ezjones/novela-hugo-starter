+++
authors = []
date = 2021-01-02T08:00:00Z
draft = true
excerpt = "Story"
hero = "/images/dsl_7714.jpg"
timeToRead = 0
title = "Hi"

+++
## [Instant Preview URLs](https://forestry.io/docs/previews/instant-previews/#instant-preview-urls)

When you click the preview button on a piece of content, Forestry will attempt to determine which URL to open by temporarily inserting a unique preview token in the markdown body. There are two situations where this won’t work:

### [If the Layout Doesn’t Use Markdown Body](https://forestry.io/docs/previews/instant-previews/#if-the-layout-doesn-t-use-markdown-body)

You may have some layouts that don’t utilize the body of the markdown file. This happens when you instead build the page entirely from front matter data, such as when you use [blocks](https://forestry.io/docs/settings/fields/blocks).

For these layouts, Forestry also inserts a special front matter value that you can include in these layouts to improve Forestry’s preview URL behavior. By outputting the contents of the `forestry_instant_preview_id` frot matter key our layout, Forestry will be able to identify the content being previewed. You can output this value anywhere between the opening and closing `<body>` tags of your HTML. It is recommended to add it as an HTML comment. If your HTML is being run through a minifier that strips comments, it’s fine to insert it differently, such as in a `<meta>` tag.

Be aware that `forestry_instant_preview_id` will only be inserted in one file at a time, and won’t be guaranteed to be there, so your code should check for it before outputting its value.

sd

as

da

sd

![](/images/dsl_7714.jpg)