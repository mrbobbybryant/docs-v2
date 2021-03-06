---
page: introduction
title: WP REST API version 2.0 Introduction
include_title: No
---
WP-API is organized around [REST][]. Our API is designed to have predictable,
resource-oriented URLs and to use HTTP response codes to indicate API errors.
We use built-in HTTP features, like HTTP authentication and HTTP verbs, which
can be understood by off-the-shelf HTTP clients, and we support cross-origin
resource sharing to allow you to interact securely with our API from a
client-side web application. JSON will be returned in all responses from the
API, including errors.

[REST]: http://en.wikipedia.org/wiki/Representational_state_transfer

<div class="routes">
	{% capture posts %}{% include routes/posts.md %}{% endcapture %}
	{{ posts | markdownify }}
	{% capture pages %}{% include routes/pages.md %}{% endcapture %}
	{{ pages | markdownify }}
	{% capture media %}{% include routes/media.md %}{% endcapture %}
	{{ media | markdownify }}
	{% capture post_meta %}{% include routes/post_meta.md %}{% endcapture %}
	{{ post_meta | markdownify }}
	{% capture post_revisions %}{% include routes/post_revisions.md %}{% endcapture %}
	{{ post_revisions | markdownify }}
	{% capture comments %}{% include routes/comments.md %}{% endcapture %}
	{{ comments | markdownify }}
	{% capture taxonomies %}{% include routes/taxonomies.md %}{% endcapture %}
	{{ taxonomies | markdownify }}
	{% capture terms %}{% include routes/terms.md %}{% endcapture %}
	{{ terms | markdownify }}
	{% capture users %}{% include routes/users.md %}{% endcapture %}
	{{ users | markdownify }}
</div>
