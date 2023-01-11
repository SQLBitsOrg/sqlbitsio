# SQLBits.io short links

This repo will create sqlbits.io shortlinks

You can see the existing short links here https://sqlbits.io/whatdowehave

# How to create a new short link for sqlbits.io in the browser

To create a new short link, you need to create a new file in the root of this repository.

use the Add file button here

![image](https://user-images.githubusercontent.com/6729780/211768161-0363bc21-f685-4aad-b0e6-437211346d2b.png)

The name of the file needs to be the shortlink and the extension needs to be md.

So if you want to create  

sqlbits.io/darren  

you create a new file called `darren.md`, the picture below creates one called `meettheteam.md`

![image](https://user-images.githubusercontent.com/6729780/211768657-c7ec98c7-3d28-484d-bd62-c130d051054f.png)

IN that file you put the following including the `---` formatted exactly like this

````
---
layout: redirected
sitemap: false
redirect_to:
  -  # This is where it will be redirected  - must be a complete url and a space after the -
permalink: /darren # this is the shortlink that we will create the / is required - MUST MATCH the name of the file amd a space after the :
---
````

You then add the URL of the webpage you are redirecting to after the single `- ` and the name of the shortlink including the `/` after the `permalink: ` There is a single space required before the URL and before the /

The file will look like this

![image](https://user-images.githubusercontent.com/6729780/211769290-f1913086-6abf-4c1f-9d4d-eb084b1eba5a.png)

To save it you scroll down and click the commit new file button.

![image](https://user-images.githubusercontent.com/6729780/211770576-1064bbf7-bb96-4b68-91c6-7647cbe42a08.png)

Then you wait for hte action to do its thing

[/sqlbitsio/actions](/sqlbitsio/actions)

Once the top one is green

![image](https://user-images.githubusercontent.com/6729780/211775268-0afcf9c3-46fd-498a-87f8-93c5c2417f37.png)


Then you test it before sharing it!!

![image](https://user-images.githubusercontent.com/6729780/211770889-1e5d826f-b33c-4eee-87eb-3d94771d603d.png)

TADA

![image](https://user-images.githubusercontent.com/6729780/211770999-26b39072-7509-4f9b-b120-5ba1c33cb458.png)

