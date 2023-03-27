---
title: Home
layout: home
---
		The project is called {{ site.title }}
		var repo_url;
		{% for repository in site.github.public_repositories %}
		* [{{ repository.name }}]({{ repository.html_url }})
		{% endfor %}
		if (site.github.GH_ENV == 'gh_pages') {
			repo_url = site.repository_nwo;
		} else {
			repo_url = 'jimting/AREEAnswer';
		};
		answer_url = "https://raw.githubusercontent.com/"+repo_url+"/master/answer.json";
