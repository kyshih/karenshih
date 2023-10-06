---
layout: post
title:  a post with custom blockquotes
date:   2023-09-05 16:40:16
description: This post shows how to add custom styles for blockquotes.
---

This post shows how to add custom styles for blockquotes. Based on [jekyll-gitbook](https://github.com/sighingnow/jekyll-gitbook) implementation.

We decided to support the same custom blockquotes as in [jekyll-gitbook](https://sighingnow.github.io/jekyll-gitbook/jekyll/2022-06-30-tips_warnings_dangers.html), which are also found in a lot of other sites' styles. The styles definitions can be found on the [_base.scss](https://github.com/imkaywu/minimal-folio/blob/master/_sass/_base.scss) file, more specifically:

```scss
/* Notes, warnings, and error */
.post .post-content blockquote {
  &.block-note {
    border-color: $bq-note-color;
    background-color: $bq-note-color-bg;

    p {
      color: $bq-note-color-text;
    }

    h1, h2, h3, h4, h5, h6 {
      color: $bq-note-color-title;
    }
  }

  &.block-warning {
    border-color: $bq-warning-color;
    background-color: $bq-warning-color-bg;

    p {
      color: $bq-warning-color-text;
    }

    h1, h2, h3, h4, h5, h6 {
      color: $bq-warning-color-title;
    }
  }

  &.block-error {
    border-color: $bq-error-color;
    background-color: $bq-error-color-bg;

    p {
      color: $bq-error-color-text;
    }

    h1, h2, h3, h4, h5, h6 {
      color: $bq-error-color-title;
    }
  }
}
```

A regular blockquote can be used as following:

```markdown
> This is a regular blockquote
> and it can be used as usual
```

> This is a regular blockquote
> and it can be used as usual

These custom styles can be used by adding the specific class to the blockquote, as follows:

```markdown
> ##### NOTE
>
> A note can be used when you want to give advice
> related to a certain content.
{: .block-note }
```

> ##### NOTE
>
> A note can be used when you want to give advice
> related to a certain content.
{: .block-note }

```markdown
> ##### WARNING
>
> This is a warning, and thus should
> be used when you want to warn the user
{: .block-warning }
```

> ##### WARNING
>
> This is a warning, and thus should
> be used when you want to warn the user
{: .block-warning }

```markdown
> ##### ERROR
>
> This is an error, and thus should
> be used carefully
{: .block-error }
```

> ##### ERROR
>
> This is an error, and thus should
> be used carefully
{: .block-error }
