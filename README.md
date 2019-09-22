# Optimizing Your Gatsby.js Website for Production

![gatsby-site-production](https://on.ahmda.ws/275123/c)

<br>

Building static sites with `React.js` using **Gatsby** provides an **easy to deploy setup**, **blazing fast speed**, and **smooth developer experience**. We are all aware of the three fundamentals of website development i.e.,

- Development
- Staging
- Production

**JAMstack (JavaScript APIs Markup)** is awesome and being the recent trend I am going to explain some of the best ways through which you can optimize your `Gatsby.js` website before production.

Before we start make sure you have configured a basic Gatsby project setup.

## Optimizing Gatsby.js Site

 <details>
 <summary> <strong><code> Step #0</code></strong>: Don't have a Gatsby site setup? Read this. (CLICK TO EXPAND!) </summary>

In case you are an absolute beginner and this is your first time with Gatsby.js, all you need to do is follow these steps mentioned below. These will help you set up a basic Gatsby project.

- Install the Gatsby CLI by typing the following command in your terminal

```sh
npm install -g gatsby-cli
```

- Next, create a new Gatsby.js site through the following.

```sh
gatsby new site-name
```

- To access your site folder contents type the following.

```sh
cd site-name
```

- Finally, start the development server to begin building your Gatsby.js site.

```sh
gatsby develop
```

</details>

To optimize a Gatsby site make sure you have the following functionalities set up and running:

- Sitemaps
- Markdown Pages
- Embed Videos
- RSS Feed

### 🔘Adding Custom Sitemaps

Sitemaps maintains a list of all pages to tell search engines like Google about the organization of your site content. These prompts information about an unindexed
page to get it appropriately indexed. They are equally important for new and old sites. But a new website needs sitemap since it is difficult for search engines to find posts and pages of a new site.

You can add custom sitemaps in Gatsby through the `[gatsby-plugin-sitemap]` plugin.

Inside your terminal type the following to install this plugin.

```sh
npm install -- save gatsby-plugin-sitemap
```

### 🔘 Adding Markdown Pages

Gatsby plugins can read folders/files with markdown and create pages from them. Is important since writing in markdown is always easy of eyes, user friendly with less errors. So, the process of adding and rendering markdown in Gatsby is ￼￼that the plugins read files from filesystem. Then it transforms  markdown to html and frontmatter to data. Finally, using the create page API you build page components.

All this is done via using the `gatsby-source-filesystem` plugin.

Inside your terminal type the following to install this plugin.

```sh
npm install -- save gatsby-file-sourcesystem
```
But to make this plugin work you need a pre-requisite plugin i.e., `gatsby-transformer-remark` which is installed via the following:

```sh
npm install -- save gatsby-transformer-remark
```

### 🔘 Embedding Videos in Gatsby.js

Different web applications render media files especially videos and GIFs  differently. With Gatsby, plugins helps you source videos from a variety of video hosts like YouTube, Vimeo, Dailymotion, etc.

The `gatsby-remark-embed-video` plugin is a great piece of software for this purpose.

In your terminal type the following for plugin installation:

```sh
npm i gatsby-remark-embed-video
```

Also, this plugin require some other plugins to be installed first. These are:

- `gatsby-remark-responsive-iframe`
- `gatsby-transformer-remark`
- `gatsby-remark-images`

Note that if you’re using the `gatsby-remark-responsive-iframe` plugin, you have to ensure that the `gatsby-remark-embed-video` plugin is defined first.

### 🔘 Adding RSS Feed

When developing a Gatsby.js, website it is important to optimize for RSS Feed since it makes your site content easy to subscribe through feed reader apps.

The `gatsby-plugin-feed` serves the purpose really well.

Install it via the following command:

```sh
npm install -- save gatsby-plugin-feed
```
It needs the following two plugins as a pre-reqs:

- `gatsby-transformer-remark`
- `gatsby-source-filesystem`

### 🔘 Final Build & Deploy

After you have optimized your Gatsby website for the aforementioned functionalities you can run the final build command and then deploy it to some live environment. I am a huge fan of **Netlify** and host all my JAMstack sites through it.

That's about it! I hope you find this learning material helpful. You can share your feedback by 🌟this repo. For any queries and suggestions PRs are welcomed.
> 👋 **[Follow @MaedahBatool on Twitter](https://twitter.com/MaedahBatool/) →**
