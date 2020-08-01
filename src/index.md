---
# Feel free to add content and custom Front Matter to this file.

layout: home
---

> Bridgetown Environment: **{{ bridgetown.environment }}**

This is what is being rendered in the head of this document:

```html
{% plausible %}
```

## Introduction

[Plausible](https://plausible.io) is a lightweight and open-source website analytics tool. It doesn’t use cookies and is fully compliant with GDPR, CCPA and PECR. This plugin is meant to remove all friction from adding your [Plausible Analytics tracking script code](https://docs.plausible.io/plausible-script) to your Bridgetown site.

The alternative to using this plugin is just pasting your Plausible tracking script code directly into the head of your document:

```html
<head>
  <!-- ... -->
  <script
    async
    defer
    data-domain="yourdomain.com"
    src="https://plausible.io/js/plausible.js"
  ></script>
  <!-- ... -->
</head>
```

[But if you use this plugin](https://github.com/andrewmcodes/bridgetown-plausible-tag), all you need to do is define your [Plausible domain](https://docs.plausible.io/add-website) in your Bridgetown config file and paste this into your document head:

{% raw %}

```html
<head>
  <!-- ... -->
  {% plausible %}
  <!-- ... -->
</head>
```

{% endraw %}
