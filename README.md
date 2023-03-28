# off-paper-dev-challenge-public

Welcome to Off-Paper's development challenge! This assessment is designed to test your skills in Shopify theme development and give us an insight into your problem-solving abilities.

In this assessment, you will be tasked with adding a few small features to a custom section for our imaginary client's Shopify theme. Your task will involve using your knowledge of Liquid, HTML, CSS, and JavaScript to create a dynamic and responsive section that can be easily customized by our client.

We understand that this may be your first time working with Shopify, but we encourage you to approach this task with an open mind and a willingness to learn. We value creativity, attention to detail, and the ability to work efficiently under tight deadlines, so we're excited to see what you can come up with.

This assessment was not designed to be crazy intesive or overly difficult -- it's merely a way for us to see how your brain works. Try not to stress out too much! We've provided pointers and resources to help you along the way.

This assessment is due at 11:59PM on the day it is assigned. Good luck - well, you don't need luck -- you got this! 

## Before you begin 

This assessment requires that you have installed Shopify's CLI in order to configure the development server. 
Here's a link to the documentation with installation instructions and a list of commands: https://shopify.dev/docs/themes/tools/cli

You'll need to fork this repository in order to work on the assessment.

## Getting started 

Use the following command to spin up your development server:

```
shopify theme dev --store=off-paper-dev-challenge.myshopify.com
```

If this is your first time, you'll be prompted to log into Shopify Partners. You can log in with the credentials that were given to you in our introductory Zoom call. 

Once you successfilly log in, you can return to your terminal. 

When your develepment server is up, the CLI will provide you three links:

1. A link to your development theme at http://127.0.0.1:9292. This URL can hot reload local changes to CSS and sections, or refresh the entire page when a file changes, enabling you to preview changes in real time using the store's data. You can specify a different network interface and port using --host and --port.

2. A link to the customizer for the theme in the Shopify admin. (You'll be needing this)

3. A sharable preview link. (You probably won't be needing this one)

If you make any changes via the development customizer, you can pull them using the following command: 

```
shopify theme pull
```

You'll be working in the file **featured-in-logos.liquid**. You can find this file in the **sections** directory.
Don't forget to commit your changes when you've finished. :)

## And now, onto the task at hand.

Imagine the following scenario: a client has asked us to create a custom section for their Shopify store. This purpose of section is to showcase the logos of the various publications that their products have been featured in. So far, we've set it up as a dynamic image multicolumn, with each block containing one logo. 

![Screenshot of current Logos section](https://github.com/Off-Paper-Creative/offpaper-dev-challenge-public/blob/master/assets/Screen%20Shot%202023-03-24%20at%203.17.34%20PM.png)

Not bad so far, but our client has requested a few changes to the section. The required changes are listed as follows:

### TODO #1

![Animated screenshot depicting finished result of TODO #1](https://github.com/Off-Paper-Creative/offpaper-dev-challenge-public/blob/master/assets/Recording%202023-03-23%20at%2015.37.03.gif)

Our client has requested the ability to adjust the top and bottom padding of this section via the theme customizer. To fulfill this requirement, please add an input setting to the schema at the bottom of the file. Don't forget to add your dynamic styles inside of the style tags at the top of the file. 

### TODO #2

![Animated screenshot depicting finished result of TODO #2](https://github.com/Off-Paper-Creative/offpaper-dev-challenge-public/blob/master/assets/Recording%202023-03-23%20at%2015.46.56.gif)

Our client requires that each logo be clickable, with the capability to dynamically change each link within the customizer. To achieve this functionality, please add an input setting to the schema, along with the corresponding HTML and liquid tag required to render the link.

### TODO #3 

![Animated screenshot depicting finished result of TODO #3](https://github.com/Off-Paper-Creative/offpaper-dev-challenge-public/blob/master/assets/Recording%202023-03-23%20at%2015.49.26.gif)

Our client has requested a subtle interactive animation, specifically to scale up each logo image on mouseover, but ONLY for those with an attached link (See TODO #2). Please write a script using JavaScript to achieve this effect. Although it's possible to accomplish this with pure CSS, for the purposes of this exercise, JavaScript is required. Please note that the client specifically requested this animation to be applied only to linked images.

## Resources and documentation 

Here are some handy resources to help you along:

https://www.shopify.com/au/partners/shopify-cheat-sheet
https://shopify.dev/docs/themes/architecture/settings/input-settings
https://shopify.dev/docs/themes/architecture/sections/section-schema
