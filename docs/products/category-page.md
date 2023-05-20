---
layout: page
title: Category Page
subtitle: Products
menubar: docs_menu
show_sidebar: false
toc: true
---

## Category Page

To create a category page listing your products you will need to create a product category page. 

Create a page, for example `products.md`, with the `layout: product-category` in the front matter. You can set the sort order of the products using `sort: title` to sort by the title, or by any setting in your product pages, such as price, rating or any custom front matter tags you wish to set. 

```yaml
title: Products
subtitle: Check out our range of products
layout: product-category
collection: products
show_sidebar: false
sort: title
```

[View example Category page](/bulma-simple-theme/products/)

## Product Include

The product include allows you to include products anywhere.

The include needs only the products as argument, and an optional tag for filtering.

Below is an example for the include.

{% raw %}
<code>
&lt;div class="columns is-multiline"><br/>
{% include product-items.html products=site.products tag="Category1" %}<br/>
&lt;/div>
</code>
{% endraw %}

## Example Product Include

<div class="columns is-multiline">
{% include product-items.html products=site.products tag="Category1" %}
</div>
