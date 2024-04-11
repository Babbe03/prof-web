---
title: "Attention"
subtitle: "Gaining and maintaining the attention of your students"
excerpt: "Attention is the foundation of learning. Without ensuring attention from your students there can be no learning; no acquisition of knowledge. Attention is mainly determined by the framing of the information, rather than the information itself. Through the use of novelty, intensity, and movement/motion your students will pay and maintain their attention on you."
date: 2021-01-28
author: ""
draft: false
# layout options: single, single-sidebar
layout: single
categories:
- Attention
---

Attention is such a fundamental concept that it seems pointless to discuss what it actually means. However, any fundamental concept always carries with it misconceptions perpetuated through tradition. Thereby, it seems most fitting to start with these misconceptions, and the implications of their dispelling. 

## 1. Attention is not continuous.

An experiment done by Bunce et al. in the chemistry department at the Catholic University of America was designed to answer three questions regarding student attention: 

    1. How often do students report attention lapses during a 50-min lecture,
    2. how long are these attention lapses,
    3. and what possible pedagogical influences are there on the lapses?

For six weeks, students were asked to use a clicker anytime they noticed themselves being distracted and inattentive. The clicker had three buttons signifying varying lengths of time they were “gone” for 1 minute or less, 2-3 minutes, or 5 minutes and more. The clicker data was collected every 30 seconds throughout the lectures, allowing Bunce et al. to see when the lapses occurred for the students. So what did they find?

Firstly, attention is not kept for the entire 50 minutes. No student using the clicker was able to hold attention for even 10-20 minutes, let alone the entire 50 minutes. Some students even reported lapses in attention within the first 30 seconds of the lecture. 

Secondly, attention is a cyclical process. Students would be engaged in a state of attention, then switch to inattention, and then back to attention. These cycles occurred consistently throughout the lecture, but the length varied over the class duration. The time between inattentive periods would become shorter and shorter the more time that passed. Students would become less capable of holding their attention later in the class, being forced to abandon their longer periods of attention and instead be in a state of almost constant jumping between attention and inattention. 

Thirdly, using student-centered pedagogical techniques leads to less reported inattention and increases attention after. When teachers performed demonstrations or assigned questions for the students to answer with clickers, fewer students would indicate lapses of attention. Furthermore, fewer students reported lapses in attention for the lecture section following demonstrations, indicating that students were more focused on the student-centered techniques and were able to maintain that increased attention. 



## 2. Attention is not one thing 


## 3. Attention is not due to a lack of interest


Wherever you end up wanting to show your social icons, you'll need to start by setting up the links in your site `config.toml` file. Open that up and scroll down to the `[[params.social]]` section. The start of it looks like this:

```toml
[params]
  <!--snip snip-->
  
  # Social icons may appear on your site header, footer, and other pages
  # Add as many icons as you like below
  # Icon pack "fab" includes brand icons, see: https://fontawesome.com/icons?d=gallery&s=brands&m=free
  # Icon pack "fas" includes solid icons, see: https://fontawesome.com/icons?d=gallery&s=solid&m=free
  # Icon pack "far" includes regular icons, see: https://fontawesome.com/icons?d=gallery&s=regular&m=free
  [[params.social]]
      icon      = "github" # icon name without the 'fa-'
      icon_pack = "fab"
      url       = "https://github.com/apreshill/apero"
  [[params.social]] <!--lather, rinse, repeat-->
```

For each link, you'll need to start a new portion that begins with `[[params.social]]`. Then, pick your `icon` and `icon_pack` from the [Font Awesome](https://fontawesome.com/) free icon library:

+ Icon pack "fab" includes [brand icons](https://fontawesome.com/icons?d=gallery&s=brands&m=free)

+ Icon pack "fas" includes [solid icons](https://fontawesome.com/icons?d=gallery&s=solid&m=free)

+ Icon pack "far" includes [regular icons](https://fontawesome.com/icons?d=gallery&s=regular&m=free)

Finally, add the `url` that you would like users to go to when they click on that icon. All external links (i.e., those that start with `http`) will open in a new tab (that is, `target="_blank"`); relative links to pages within the site will open in the same window.

Now you should be all set to show/hide your social icons. Each of these will pull the social icons and urls from the settings you just created in your site configuration file.

## Show social in site header and footer

Let's start with the header and footer, as those are site-wide. Open up your site `config.toml` file again and scroll down to the `[params]` section (it is actually :up: from where you configured these icons):

```toml
[params]
  <!--snip snip-->
  
  # show/hide social icons in site header & footer
  # configure social icons and links below in [[params.social]]
  socialInHeader = false
  socialInFooter = true
```

That was easy!

## Show social in homepage

Open up `content/_index.md`. That file's YAML controls what you see on the homepage. Set `show_social_links` like so:

```yaml
show_social_links: true # specify social accounts in site config
```

If you set this to `true` to show the icons on the homepage, your social icons in the footer will not show up even when you set `socialInFooter = true`, so as not to litter your site with too many icons.

## Show social in about page sidebar

Open up `content/about/sidebar/index.md`. That file's YAML controls what you see in the sidebar on the about page. Set `show_social_links` like so:

```yaml
show_social_links: true # specify social accounts in site config
```

## Show social in contact page

You may use the YAML for your contact page (located in `content/form/contact.md`):

```yaml
---
show_social_links: true # specify social accounts in site config
---
```
