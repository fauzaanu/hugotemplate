---
title: "Config File"
date: 2019-01-15T16:18:12+01:00
publishDate: 2019-01-29T19:12:12+01:00
---

```
baseURL = "https://example.com/"
languageCode = "en-us"
title = "Edna West"
theme = "personal_web"
copyright="© Edna West"
googleAnalytics = ""
enableEmoji=true
enableRobotsTXT=true

[params.intro]
  main = "Hi, I'm Edna :wave:"
  sub = "I'm a Web Developer and Entrepreneur"

[taxonomies]
  design = "designs"
  tech = "techs"

[blackfriday]
  hrefTargetBlank = true

[params]
  breadcrumb = true
  accentColor = "#FD3519"

[params.notFound]
  gopher = "/images/gopher.png" # checkout https://gopherize.me/
  h1 = 'Bummer!'
  p = "It seems that this page doesn't exist."
  mainSection = 'portfolio' # values: [post, portfolio] only accept one section, to be displayed bellow 404

[params.sections]
  # Define how your sections will be called
  # when automatically pulled. For instance in the 404 page
  post = "article"
  portfolio = "project"

[params.sidebar]
  backgroundImage = '' # header background image - default "/images/default_sidebar.jpg" - Photo by Tim Marshall on Unsplash
  gradientOverlay = '' # default: rgba(0,0,0,0.4),rgba(0,0,0,0.4)
  logo = "" # - default "/images/edna-west.jpg"
[params.assets]
  favicon = ""
  customCSS = ""

[params.social]
  github = "https://github.com/bjacquemet"
  twitter = "https://twitter.com/jacquemetb"
  linkedin = "https://www.linkedin.com/in/baptistej"

[params.contact]
  email = ""
  text= "" # text of the contact link in the sidebar. If email params.contact.email is defined


[menu]

[[menu.main]]
  identifier = "about"
  name = "About"
  title = "About section"
  url = "/about/"
  weight = -120

[[menu.main]]
  identifier = "portfolio"
  name = "Portfolio"
  title = "Portfolio"
  url = "/portfolio/"
  weight = -110

[[menu.main]]
  identifier = "blog"
  name = "Post"
  title = "Blog section"
  url = "/post/"
  weight = -100

[sitemap]
  changefreq = "monthly"
  filename = "sitemap.xml"
  priority = 0.5

[privacy]
  [privacy.googleAnalytics]
    anonymizeIP = true
    disable = true
    respectDoNotTrack = true
    useSessionStorage = false
  [privacy.twitter]
    disable = false
    enableDNT = true
    simple = false
```