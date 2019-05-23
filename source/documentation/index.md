# Doing a basic accessibility check if you can’t do a detailed one

The first step towards meeting [the new accessibility requirements](https://www.gov.uk/guidance/accessibility-requirements-for-public-sector-websites-and-apps) involves evaluating how accessible your website is.

This means checking whether or not it meets the [international WCAG 2.1 AA standard](https://www.gov.uk/service-manual/helping-people-to-use-your-service/understanding-wcag).

Checking this in detail requires a large amount of technical expertise and is best left to either:

+ an accessibility expert within your organisation
+ a third-party accessibility auditor

Some organisations won’t have the expertise to do a detailed check themselves and paying a third party would place a ‘disproportionate burden’ on them. This means a burden or cost that is too much for the organisation to reasonably bear.

If this applies to your organisation, you’ll have to do a basic check instead. This guide will help you to do that basic check.

The checks outlined in this guidance can be done by anyone with a basic knowledge of websites - any web officers in your organisation or volunteers, for example.

> Before you start, [check whether it’s reasonable for you to do a detailed accessibility check instead](https://www.gov.uk/guidance/make-your-website-or-app-accessible-and-publish-an-accessibility-statement#decide-how-to-check-your-website-or-app-for-accessibility-problems). If it is, then just doing a basic check won’t be enough for you to meet the requirements.

## Preparing to do a basic accessibility check

You don’t need to check every page of your website - just a sample. So start by working out which sample of content you’re going to check.

If you’ve got more than one website or app, you need to gather a sample from each website or app you have.

Your sample needs to include:

+ your site's homepage
+ content pages that are mostly text based     
+ images, video and audio content
+ interactive tools and transactions, like forms
+ pages including login functionality, if your website has them 
+ PDFs and other document types you have
+ dynamic content like pop-up windows
+ navigation pages, including your sitemap and pages with search functionality 

You should also include in your sample any pages or websites containing information about accessibility, how to contact you, how to use your site, legal information (for examples terms and conditions pages, or things like your privacy policy) and any settings or preferences pages.

Once you’ve got your sample, work through the checks outlined in this guidance one by one.

It’s likely the checks will take at least a few days, so make sure to give yourself enough time to work through them.

Some of the requirements might not apply to your website. For example, if you don’t have any videos then you won’t be able to carry out any of the tests relating to video content.

## 1. Text content

You’ll need to start by checking the text-based content pages (and any PDFs or other documents) you included in your sample.

### Check content is marked up properly

It’s important that your content is marked up correctly. This is because some users with visual impairments use tools called ‘screen readers’ that read out page content to them.

Things like lists and headings need to be marked up in a way that allows screen readers to tell what they are and how your content is structured.

You’ll be able to check some of these things in your content management system. For instance, you can check to see whether any headings are marked up with ```<h2>``` or ```<h3>``` tags, or ```##``` and ```###``` if you’re using markdown. Headings shouldn’t just be marked up in bold.

You might need to look at the page HTML to check things like tables or bullet lists. How you do this depends on which browser you’re using. If you’re using:

+ Google Chrome, right-click a table or bullet list and select ‘inspect’
+ Safari, right-click a table or bullet list and select ‘inspect element’ - you might need to [enable Safari developer tools](https://developer.apple.com/library/archive/documentation/NetworkingInternetWeb/Conceptual/Web_Inspector_Tutorial/EnableWebInspector/EnableWebInspector.html) first
+ Edge, click ‘F12’ to open the developer tab and then hold ‘Ctrl’ and ‘B’ - once you’ve done that, left-click on a table or bullet list to inspect the HTML
+ Firefox, right-click a table or bullet list and select ‘inspect element’ - you might need to [enable Firefox web developer](https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector/How_to/Open_the_Inspector) first

Once that’s done, look out for the following sorts of tags:

+ for tables, look out for ```<td>```, ```<th>``` and ```<tr>```
+ for bullet lists, look out for ```<ul>``` and ```<li>```

If you can see these tags, it’s likely your content is marked up properly.

To check PDFs or other documents, open them in the tool used to create them and check that:

+ headings are marked up properly, using the proper document structure settings like the [styles gallery in Microsoft Word](https://support.office.com/en-ie/article/add-a-heading-3eb8b917-56dc-4a17-891a-a026b2c790f2)
+ tables and bullet points are properly styled - for instance, you’re not just using hyphens for bullet lists

### Check pages are usable when stylesheets are disabled

A stylesheet defines the visual layout of a web page. Your content still needs to be usable even if stylesheets are disabled.

You can test this by copying a URL from your website and pasting it into the [WAVE tool](http://wave.webaim.org/). Once you’ve done that, select ‘no styles’ from the panel on the left-hand side of the tool. This should give you a much more basic view of the page.

Repeat this process with all your sample content pages and check whether they’re still usable. This means it’s still possible to complete any relevant tasks or find important information - for example, look for opening hours or contact details, or navigate your way to a form you need to fill out.

You won’t be able to do this test on PDFs or other document types.

### Check that instructions are styled properly

You need to make sure you’re not conveying instructions in a way that relies on a user’s ability to see the page.

For example, only sighted users will understand instructions like:

+ ‘click the round button’
+ ‘click the big button below’
+ ‘click the red button’

Users who can’t see the page won’t know what you’re referring to, because instructions like that rely on you being able to see the page.

So check your sample of pages and look out for these types of instructions.

### Check that links make sense

Check any links on your sample content pages to check that the link text you’re using clearly explains where any links will take the user.

This is important because screen reader users often scan through lists of links in isolation. This means they don’t have the surrounding context to help them understand what the link is for.

You can check your links by looking at your sample pages and just reading the link text - without paying attention to the surrounding content. If the links still make sense even in isolation and clearly explain where the links go, it’s likely the text you’re using is accessible.

If you’re using link text like ‘click here’ or ‘more information’ then you’re probably not meeting this requirement - link text like that doesn’t describe where the link will go or what it’s for.

There’s [guidance explaining what good link text looks like](https://www.gov.uk/guidance/content-design/links#writing-link-text) if you’re not sure.

### Check that pages have good titles

You need to check your pages are titled properly. If they’re not, users won’t understand what they’re for and will struggle to find what they need using search.

Your page title should appear in the page tab at the top of your browser. For instance, if you go to [the GOV.UK homepage](https://www.gov.uk/) you’ll see the text in the tab near the top of the browser is ‘Welcome to GOV.UK’. This is the page title.

Look at the equivalent text for your sample pages. You can hover over the tab to see the full text if it’s too long to fit on the tab itself.

Check whether your titles are descriptive. Ask yourself whether they clearly state - in simple language - what the pages are about and the tasks they’d help users complete.

For example, ‘Apply for a blue badge’ is a much more descriptive title than just ‘Blue badges’.

Also check that none of the titles are duplicated: if two pages have the same title, how is the user supposed to know which one to use?

There’s [guidance on writing good page titles](https://www.gov.uk/guidance/content-design/writing-for-gov-uk) if you need help.

### Check the language the content is written in

A screen reader needs to know what language a page is written in so it uses the correct speech libraries for accent and pronunciation. It only knows this if the language is specified in the page HTML.

You’ll need to check the HTML of your sample content pages to see whether your website does this. To inspect the page HTML, use the same method you used when checking whether your content was marked up appropriately.

Once you’ve opened the HTML, scroll to the top of the panel. You should see a ```<!doctype html>``` tag. Directly under that you should see an ‘<html lang=”’ tag. This is where the screen reader finds out the page language.

If the page is written in English, the tag should read ```<html lang=“en”``` or ```<html lang=en-gb```. If it’s empty, the screen reader won’t be able to tell what language the page is in.

If any of your sample pages contain content written in other languages, you’ll need to check that’s marked up properly too, using the [country code for the relevant language](https://www.sitepoint.com/iso-2-letter-language-codes/).

## 2.  Images, video and audio content

There are a series of things you’ll need to do to check that your sample of images and video content is accessible. You should also do the image checks on any PDFs or other documents you included in your sample.

### Check any images are described in the page copy

You’ll need to check that your sample of images either:

+ have appropriate alternative (or ‘alt’) text that explains the information the image conveys
+ are described in any surrounding body text, so anyone who can’t see the images can still access the information the image conveys

You might be able to check and edit any alt text using your content management system (CMS).

If that doesn’t work, you can check it by inspecting the page HTML. Use the same method you used when checking whether your content was marked up properly.

Once you’ve opened up the HTML panel, inspect one of the images for alt text. If there is any, it’ll appear after the ```<img alt=``` tag.

### Check any video or audio content is properly described
As you did with your images, you’ll need to check that any videos or audio content are clearly described.

This firstly means checking that videos have captions. You should also check your sample videos (maybe 2 or 3) to assess the quality of those captions.

Once you’ve done that, you’ll need to check for transcripts for any audio content you’ve got.

### Audio descriptions for video and audio content

When you check through the videos on your website, you might come across things that are covered in the video but not described in the audio track - something like the contents of a chart or graph, for example.

If you were only following the audio, you’d miss this information. So for your site to be fully accessible, you’d need to provide an extra audio description to describe anything not covered in the main audio track.

Check your sample of videos to see if an extra audio track is required and whether you’re providing one.

### Check any video players are accessible

You need to check that any video players are accessible. This means checking that the buttons you need to use to interact with the video player are marked up in a way that a screen reader would recognise.

You’ll need to inspect the page HTML to check whether you’re meeting this requirement. Do this using the same method you used to check whether your text content was marked up properly.

Once you’ve done that, right-click (or left-click if you’re using Edge) one of the video player buttons and select ‘inspect’ or ‘inspect element’, depending on the browser you’re using.

Check whether the button’s been given a name like ‘Play’ or ‘Pause’ - if it has, the name will likely appear as part of a ‘title’ or ‘aria label’ tag.

If there’s no text indicating what the button does then it probably hasn’t been marked up properly. This means a screen reader won’t know what the button’s for and that users need to be able to see and understand the button icon to work it out for themselves.

### Check for images containing text

You’ll need to check whether any of your sample images contain text. This doesn’t include logos and brand names - it’s okay for those to contain text.

## 3. Interactive tools and transactions

You’ll need to do a few checks relating to the forms on your website.

### Check form fields are marked up appropriately

You need to make sure any form fields are marked up correctly. If they aren’t, screen readers won’t be able to tell what a form field is for, or what information the user should enter into it.

You can check your form fields are marked up properly by going to a form and clicking on a field label (the text that explains what a particular form field is for). If the field is marked up correctly, clicking the field label should cause your cursor to appear inside the corresponding field.

You can see what this looks like using the [GOV.UK contact form](https://www.gov.uk/contact/govuk#do-you-want-a-reply). If you click on the ‘Your name’ field towards the bottom of the page, you’ll see the focus of your cursor switches to the field itself.

Do this test on a few of your forms and see what happens.

### Check it’s clear what information users need to provide

As you go through your sample forms, you’ll need to check you’re using field labels in a way that makes clear what information the user needs to enter.

As a general rule, these labels should be specific. Look at your forms and make an assessment as to whether they’re clear. Common mistakes include not labelling fields at all, or using vague labels like ‘Name’ in a way that doesn’t make clear whose name the user needs to enter (for example, it could be a partner or child’s name, rather than the user’s own name).

### Check form elements are consistent across your website

When you’re checking through your forms, you’ll need to check that form labels are used consistently. These are the labels that describe the information a user needs to enter into a particular field.

Check your sample to see how you’re labelling the navigational elements. For instance, are you using ‘Submit’ on one form and then using ‘Go’ or ‘Complete’ on another?

Are you asking for users’ names and addresses in a consistent manner, or does it vary from form to form?

### Check that users can autofill information where appropriate

You need to make sure users can autofill information in forms where possible. For example, they should be able to autofill their name and address if their browser has saved this information.

Test this by filling out a form elsewhere on the internet - sign up for or order something online, or do your online shop.

Now come back to a form on your website. If you get the chance to autofill some or all of your address or personal details, then your website is meeting this requirement.

### Check users get a warning before they’re timed out

Some websites time users out after a period of inactivity. This usually results in form data being lost, or the user being automatically logged out of an account.

You need to make sure to warn users if you’re going to time them out after a period of inactivity. You’ll also need to give them the chance to interact with the page to prevent the time out from happening.

Test whether you’re doing this by going to one of the forms on your website and remaining inactive for around 20 minutes. If you get timed out with no warning, then you’re not meeting the requirements.

If, after a while, you were given a timeout warning and a chance to prevent the timeout by interacting with the page, you’re likely meeting the requirements.

### Check that any error messages are helpful

When a user provides incorrect information in a form, you need to let them know they’ve made a mistake and help them correct that mistake.

You can check how well your website is doing this by going to your sample forms and entering some intentionally incorrect or invalid information.

For example, you could enter a future date into a date of birth field or a postcode with too few characters and try submitting the form. This should generate an error message.

Assess whether the error messages make clear what you need to do to correct the mistakes. Messages like ‘invalid date’ or ‘invalid postcode’ aren’t very helpful: they indicate that the user has made a mistake, but don’t explain why the information was wrong and how to correct the error.

Something like ‘You can’t enter a date in the future - please enter a past date’ is much more helpful.

Play around with a few form fields to see how helpful the error messages are.

### Check users can review their answers before submitting a form

Users need to be able to check their answers before submitting certain types of form, to confirm they’ve entered the correct information. This only applies to forms where there would be serious consequences to them making a mistake - for example, financial transactions or something that enters them into a legal contract.

You can test this by going to any of your sample forms that meet these criteria and working your way through them. See if you’re presented with [a page that lets you check your answers](https://design-system.service.gov.uk/patterns/check-answers/) before submitting the form.

### Check that form elements behave as expected

When you were working your way through some of your sample forms, you should have noticed whether interacting with any of the elements caused anything unexpected to happen.

This includes things like a dropdown menu or radio button (an element that lets you select just one of a few options) causing a new page to open when you click on it.

## 4. PDFs and other documents

If you’ve been checking your PDFs and other documents as you work your way through these tests, you don’t need to worry about this section.

If you’ve only come to this guide to check the accessibility of your PDFs and other documents, then focus on the following sections:

+ 1 Text content
+ 2 Images, video and audio content
+ 5.4 Colour contrast

## 5. Technology

You’ll need to do check that users don’t have trouble interacting with your website. This means checking for technological or frontend issues.

### 5.1 Tests using a mobile or tablet device

You’ll need to do some checks using a mobile or tablet device to check that your website is usable on these types of device.

#### Check the page orientation

You’ll need to take a few of your sample pages and check they respond properly when you try to change the page orientation.

You can do this by loading up a page and turning the screen from portrait to landscape a few times. If the page responds and changes to fit that view, then you’re meeting the requirement. If it stays locked in place, then you’re not.

#### Check you can navigate using just one finger

Some users have limited dexterity or range of movement, which means it’s important that they don’t have to use complex gestures that involve more than one finger to navigate your website. There needs to be a simple alternative that they can use that only requires one finger.

Go through your sample content pages and check whether it’s possible to navigate using just one finger. Try things like double-tapping to zoom in and out of the page and holding or hovering your finger over an element to highlight it.

It’s worth trying to complete a couple of forms using these techniques, too.

#### Check you’re not relying on complex motions

Some more interactive websites or apps require users to do things like shake or tilt their device to complete an action.

This won’t apply to most websites, but if it applies to yours then you need to make sure there’s an alternative for users who can’t move their device in these ways.

Check that none of your sample pages require any of these types of interactions - and if they do, that there’s another way of completing the task.

### 5.2 Navigating just using a keyboard

Some of your users won’t be using a mouse and will need to navigate just using a keyboard. You’ll need to do some checks to see how easy it is for them to do that.

The main keys you’ll be using to navigate are the ‘Tab’, ‘Enter’ and ‘Esc’ keys. ‘Tab’ is the key that lets you jump between page elements, while ‘Enter’ and ‘Esc’ let you interact with and dismiss those page elements.  

You might need to [enable the tabbing function if you’re using Safari](https://a11yproject.com/posts/safari-keyboard-navigation/).

#### Check you can tell where you are on the page

When you navigate just using a keyboard, you don’t have the mouse cursor to let you know where the focus is on the page. You need to make sure there’s another way for users to orientate themselves and understand which page element they’re focusing on.

For example, if you tab through the [GOV.UK homepage](https://www.gov.uk/) you’ll notice that the page element in focus is highlighted very clearly with a prominent orange block.

Spend a few minutes tabbing through a few of the sample pages you selected. Ask yourself whether it’s clear where on the page you’re focused - if it takes you a while to notice which element is in focus then you’re probably not meeting this requirement.

#### Check the order makes sense when tabbing

While you were tabbing through the page elements, you should have noticed whether the tabbing moved in a logical order. For instance, if you tab on to a navigation bar, you’d expect to be able to tab through the entire bar without the focus jumping off elsewhere on the page.

Spend a few minutes testing this on a few of your sample pages.

#### Check nothing unexpected happens when tabbing through a page

When you were tabbing through your sample pages, you should have noticed whether anything unexpected happened. For example, if tabbing onto an element triggered anything like:

+ a new web page to open
+ a navigation menu to open

Another thing to look out for is whether you can interact with all the page elements you’d expect to.

For example, some websites like the Service Manual feature [hide and reveal style navigation](https://www.gov.uk/service-manual/user-research). If these navigational elements are marked up properly, you can expand and close them with a keyboard as you would with a mouse.

But if they aren’t, you’ll likely tab straight past them using just a keyboard. Look out for things like this.

#### Check you don’t get stuck when navigating through content

While you’re tabbing through your sample pages, you should notice whether you get stuck at any point.

Getting stuck means ending up somewhere you can’t navigate away from using just your keyboard. For instance, you might activate a pop-up or interactive element that you can’t skip away from just by using the ‘Esc’ key.

Users who don’t use their mouse wouldn’t be able to move away from a page element like this, which could prove very frustrating.

#### Check forms are still usable without a mouse

Take your sample of forms and see if you can complete them without using a mouse. This means using ‘Tab’ to jump between the form elements and ‘Enter’ to interact with any navigation elements, like ‘next’ or ‘submit’ buttons.

#### Check users can skip to the main content on a page

Lots of websites contain several links and navigational elements in the header at the top of the page. Users need to be able to skip past these links straight to the main page content if they want to, so they don’t have to tab through each item individually every time they open a new page.

Some websites give users the chance to skip these header blocks. For instance, if you hit ‘Tab’ when you arrive at the [GOV.UK home page](https://www.gov.uk/), you’ll see the option to ‘Skip to main content’. If you hit ‘Enter’, the page will refocus past the header block down to where the actual page content begins.

See if the same thing happens when you hit ‘Tab’ after refreshing a page on your website.

### 5.3 Checking content is usable when zoomed in or magnified

Some users with visual impairments use screen magnification tools that zoom into the page content, or increase the size of the text. You’ll need to check your content is usable for people using these tools.

#### Checking content is usable when you enlarge the text

Take a couple of the forms and content pages from your sample and see what happens if you increase the font size.

You can usually do this by changing the settings in your browser. For example, in Chrome you do this by choosing “Settings”, and changing the “Font size” from “medium” to “very large”.

Once you’ve increased the font size, try to complete a few tasks using your sample pages. If the page resizes or restructures properly, it won’t obscure any of the important information or buttons you’d need to progress through a form.

#### Checking how the page behaves when users zoom in

You’ll need to check what happens to your pages when you adjust the page zoom in your browser. You can do this either through your browser’s settings or by using a keyboard shortcut - usually ‘Cmd’ or ‘Ctrl’ plus the ‘+’ key.

Use the same sample of pages you used when tweaking the size of the text. For each page, see what happens when you zoom progressively further in.

If your website is handling this in an accessible way, then you shouldn’t need to use horizontal scroll: the content should reformat in a way that means you only need to use vertical scrolling.

### 5.4 Colour contrast

Some users with visual impairments won’t be able to interact with your website if the colour contrast isn’t set properly.

So check the colour contrast on your sample pages, including any PDFs or other document types.

#### Check for text contrast

You’ll need to check that the contrast ratio between text and the background colour of your website is at least 4.5:1.

You can use the [WAVE tool to check colour contrast](http://wave.webaim.org/).

This involves copying one of your sample URLs and pasting it into the [WAVE tool](http://wave.webaim.org/). Once you’ve done that, select ‘contrast’ from the panel on the left-hand side of the tool. This should show you the colour contrast information for the page in question.

#### Check any buttons and navigational elements

Like you did for the text on your website, you’ll need to check that the colour contrast between any buttons or navigational elements (like ‘next’ or ‘continue’ buttons in forms) and the background of your website is set appropriately.

The contrast ratio needs to be at least 3:1 in these cases. Again, use the WAVE tool to check this.

### 5.5 Pop-ups and interactive or flashing content

Pop-ups or flashing images can be very distracting. Users need to be able to disable or dismiss these elements easily.


#### Check that users can disable animated or moving content

Things like scrolling carousels or blinking images can be very distracting for people with cognitive disabilities.

If your website contains these sorts of elements, you need to check whether users can disable them.

Go to any of your sample pages containing these items and see if there’s a way to stop them. Try clicking on them, or interacting with the surrounding content. Check to see if there’s a button to stop or pause the item.

#### Check for content that plays automatically

Some websites play audio or video content automatically when a user refreshes or opens a page.

If this applies to your website - and the content plays for more than 3 seconds - you’ll need to check users can either change the volume or stop it altogether. There’s likely to be a video or audio box somewhere on the page that you can interact with to do these things.

#### Check whether there’s an alternative for people who can’t see maps

It’s very hard to make maps accessible. Instead, you need to check there’s an alternative to using the map - or another way of finding out the information the map conveys for anyone who can’t see the map.

The Pension Wise website does this well. For instance, when you [search for your nearest contact centre](https://www.pensionwise.gov.uk/en/book-face-to-face), you’re presented not only with a map you could use to navigate, but also with a text address any user could access.

### 5.6 Search and other forms of navigation

You’ll need to do some checks to see how accessible your navigational elements are.

#### Check there are multiple ways to navigate your website

Different users have different preferences, which means you need to provide more than one way of accessing content.  

The most common ways of doing this include:

+ offering a search bar
+ publishing a [site map](https://en.wikipedia.org/wiki/Site_map)
+ offering navigation categories that break up the content by theme

Check that you’re offering more than one of these options.

#### Check your navigation behaves consistently

Things like search bars and breadcrumb trails (the list of links that appear at the top of the  page to show where in your website’s navigation you currently are) should behave in the same way wherever they appear on your website.

You can check for this by going to a few of your sample pages and checking whether the navigational elements are presented consistently. If things like search boxes or navigation menus appear in different places across the pages, you’re probably not meeting the requirements.

#### Check links aren’t triggered on the down-press of a mouse

To open a link, a user has to click their mouse (known as a ‘down event’) and release it (known as an ‘up event’).

You need to check that this is how your links behave. Check a sample of your content pages and interact with some of the links - specifically to see whether the links are opened on the down click of the mouse, or whether they only open once you release the mouse button.

If they’re triggered on the down event, you’re not meeting the accessibility requirements.

## Once you’ve finished the checks

Once you’ve finished these checks, you must start [making a plan to fix any accessibility problems you found](https://www.gov.uk/guidance/make-your-website-or-app-accessible-and-publish-an-accessibility-statement#make-a-plan-to-fix-any-accessibility-problems-you-find).
