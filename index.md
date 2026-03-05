---
layout: default
title: Welcome
exclude: true
---

<div class="home">

  <h1 class="page-heading">Welcome!</h1>
  
  <p>Welcome to <em>V/LineCars.com</em> - the online resource for those interested in the day to day operations, carriages and railcars in service with V/Line - in the present, past and future!</p>
  
  <p><img src="/images/header.jpg" alt="V/Line fleet in the sidings at Southern Cross Station" /></p>
  
  <div id="on-this-day-content"></div>
  
  <h2>Recent articles</h2>

  <ul class="post-list">
    {% for post in site.posts offset: 0 limit: 3  %}
      <li>
        <span class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</span>

        <h3>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h3>
		<div class="article-content">
			{{ post.excerpt  | strip_html | truncatewords: 50 }}
		</div>
      </li>
    {% endfor %}
  </ul>
  
  <p><a href="{{ "/articles/" | prepend: site.baseurl }}">More articles</a></p>

  <p class="rss-subscribe">Subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>

<script>
	const FEED_URL = 'https://tracker.vlinecars.com/on-this-day-photo.php';

	async function fetchSingleItem() {
		const output = document.getElementById('on-this-day-content');

		try {
			const response = await fetch(FEED_URL);
			const xmlText = await response.text();
			
			const parser = new DOMParser();
			const xmlDoc = parser.parseFromString(xmlText, "text/xml");
			
			// Select the first (and only) item
			const item = xmlDoc.querySelector("item");

			// Only render if an item actually exists
			if (item) {
				const title = item.querySelector("title")?.textContent.replace("On this day ", "").trim() || "";
				
				// Handling the 'content' namespace for <content:encoded>
				const content = item.getElementsByTagNameNS("http://purl.org/rss/1.0/modules/content/", "encoded")[0]?.textContent || "";

				output.innerHTML = `
						<h2>On this day</h2>
						<p>${title}</p>
						<p style=" max-width: 702px;">${content}</p>
				`;
			}
		} catch (err) {
			console.error("Fetch error:", err);
		}
	}

	fetchSingleItem();
</script>
