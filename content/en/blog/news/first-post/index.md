---
date: 2018-10-06
title: "Easy documentation with Docsy"
linkTitle: "Announcing Docsy"
description: "The Docsy Hugo theme lets project maintainers and contributors focus on content, not on reinventing a website infrastructure from scratch"
author: Riona MacNamara ([@rionam](https://twitter.com/bepsays))
icon: fas fa-tools
resources:
- src: "**.{png,jpg}"
  title: "Image #:counter"
  params:
    byline: "Photo: Riona MacNamara / CC-BY-CA"
---

**This is a typical blog post that includes images.**

The front matter specifies the date of the blog post, its title, a short description that will be displayed on the blog landing page, and its author.

## Including images

Here's an image (`featured-sunset-get.png`) that includes a byline and a caption.

{{< imgproc featured-sunset-get.png Fill "600x300" >}}
Fetch and scale an image in the upcoming Hugo 0.43.
{{< /imgproc >}}

The front matter of this post specifies properties to be assigned to all image resources:

```
resources:
- src: "**.{png,jpg}"
  title: "Image #:counter"
  params:
    byline: "Photo: Riona MacNamara / CC-BY-CA"
```

To include the image in a page, specify its details like this:

```
{{< imgproc sunset Fill "600x300" >}}
Fetch and scale an image in the upcoming Hugo 0.43.
{{< /imgproc >}}
```

The image will be rendered at the size and byline specified in the front matter.

{{< tabpane >}}
  {{< tab header="MacOS" lang="shell" >}}

    brew install smartide

  {{< /tab >}}
  {{< tab header="Windows" lang="javascript">}}
    let var abc = "sab"
  {{< /tab >}}
  {{< tab header="Linux" >}}
    Karibu sana!
  {{< /tab >}}
{{< /tabpane >}}

{{< highlight go "linenos=table,hl_lines=8 15-17,linenostart=199" >}}
// ... code
{{< / highlight >}}

```go
func main(){
  fmt.printLn("hello world")
}
```


