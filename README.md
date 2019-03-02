# Technologiq

Technologiq is a robust Lektor theme designed for small business' with integrated blog functionality (if you want to use it), which is designed to fit the style of a small business or a SaaS landing page.  It could also be used as a template to blog about whatever it is you're developing/creating/supporting.

It uses Bootstrap 4, Jquery and Font-Awesome 4 out of the box. It also comes with integration to Google Analytics.

This comes with some example/dummy content just to give some idea of what goes where and how everything is laid out.

This theme is still under development and being adjusted here and there - so stay updated for changes.

# Configuration

Add params in the `.lektorproject file`

```ini
[theme_settings]
	first_name = "Roger"
	last_name = "Williams"
	name = "Roger Williams"
	street = "123 Somewhere Dr."
	city = "Chicago"
	state = "Illinois"
	zip = "60007"
	phone = "(312)555-4567"
	email = "your_email@yourdomain.com"
	about = "info_about_you"
	site = "rogerwilliams.com"
	googleanalytics = "your_google_analytics_id"
	facebookID = "your_facebook"
	twitterID = "your_twitter"
	instagramID = "your_instagram"
	githubID = "your_github"
	gitlabID = "your_gitlab"
	codepenID = "your_codepen"
	linkedInURL = "your_linkedin"
	googleplusID = "your_googleplus"
	profilepicture = "profile_picture_asset_url"
	googleanalytics = "your_google_analytics_id"
	slackURL = "https://join.slack.com/..."
	comments = "yes"
```

## Changing the layout

Currently this is designed to accomodate 2 different layouts (a homepage and a page layout) and is easily extended to fit your needs.

#### Default Layout

By default when a user lands on the homepage it uses the `homepage_layout.html` template to display the content in more of a SaaS landing-page-esque design. You can change which sections show in which order by simply editing that file and changing the order of the included sections.

#### Alternative Layout (Pages)
For individual pages the layout is different than the main page (as the content of the page is supposed to be the main focus of that particular page) - but the layout is designed in such a way that it's easy to include the additional sections from the main page where you want them in the page layout.

In your `contents.lr` for a page - you can include additional sections by adding a comma separated list of sections which you want included on that particular pages layout (they appear in order of the list provided) as seen below:

```
---
sections: features, about_us
---
```

## Editing the sections

To change the sections (text / formatting / layout) simply go into `templates/sections` and edit the appropriate `.html` file for the related section to display exactly as you would like.





Optionally turn on add Disqus Comments on the blog posts with lektor-disqus-comments plugin. Configure it with [this](https://github.com/lektor/lektor-disqus-comments#lektor-disqus-comments).

## License

Technologiq is licensed under the [MIT license](LICENSE.md)
