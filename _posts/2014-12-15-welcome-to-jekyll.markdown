---
layout: post
title:  "My First Post: Here We Go"
date:   2014-12-15 20:16:53
categories: jekyll update
---

You'll find this post in your `_posts` directory - edit this post and re-build (or run with the `-w` switch) to see your changes!
To add new posts, simply add a file in the `_posts` directory that follows the convention: YYYY-MM-DD-name-of-post.ext.

Jekyll also offers powerful support for code snippets:

{% highlight javascript %}
function insertNodeAt(root, node, atIndex) {
  var childNodes = root.childNodes;
  // Remove from parent so that if node is already child of root,
  // `childNodes[atIndex]` already takes into account the removal.
  var curAtIndex = root.childNodes[atIndex];
  if (curAtIndex === node) {
    return node;
  }
  if (node.parentNode) {
    node.parentNode.removeChild(node);
  }
  if (atIndex >= childNodes.length) {
    root.appendChild(node);
  } else {
    root.insertBefore(node, childNodes[atIndex]);
  }
  return node;
}

module.exports = insertNodeAt;
{% endhighlight %}

Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll's GitHub repo][jekyll-gh].

[jekyll-gh]: https://github.com/mojombo/jekyll
[jekyll]:    http://jekyllrb.com
