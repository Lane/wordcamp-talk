title: What everyone ought to know about responsive design
author: Lane Olson

!SLIDE slide x=0 y=0

## What everyone ought to know about responsive design.

- Presented by Lane Olson
- Web designer with University Digital Strategy
- Design Since 2001, made some good sites and some bad sites
  - Images of past work.
- My last year has been devoted to responsive design

## What is responsive design?

- I assume you have a pretty good idea of what responsive design is, so I'll cover this quick.
- Responsive design is all about building a website that "responds" to whichever device the website is used on.
- Goal is to provide a usable experience to the user no matter how they choose to view the site.
- Process is much different to do this, then to design for one standard resolution.

## Why should you be building sites to target all devices?

- Usage of different devices, not just mobile phone
  - Televisions, e-readers, phones, mp3 players, etc.
- People are using there phones all the time, when they're watching TV, when they're in line at the store, event when they're in the bathroom.
- Mobile phone usage stats

  
## What are your options?

- Separate sites
  - Content parity (use images)
  - managing two separate instances
- Responsive Design

## Is it the right approach?

- The first website I ever made, had to be designed for 640x480 resolution.  It used tables to position image slices together.  The markup was cluttered with font tags and style attributes. Looking back on that, it's horrible practice... but at the time it was all we had.  Who's to say in 5 years we're not looking back and laughing at what a bad approach responsive design was.  But right now it's the best we have.

  [ Thumbs up, inline on screen, 1999 ]
  [ Thumbs down, to that, 2012 ]


## Common properties of responsive design (elaborate on these points)

- No content hiding
- Mobile first
- 



!SLIDE slide x=0 y=0

## Media Queries

- Media queries are a feature introduced in CSS3 that allow you to style based on the type of media something is intended for and also maximum and minimum widths and height of the current viewport
- Very powerful (allows for print styling), showcase types of media types
- There are a ton of devices out there.  All which have different resolutions, so you might be wondering how you are supposed to support so many devices?
  
    Image showing overlay of viewports (Android fragmentation) and sad jack
    
- Use the meta tag! (use the source)

    <meta name="viewport" content="width=device-width">
    
    http://blog.javierusobiaga.com/stop-using-the-viewport-tag-until-you-know-ho
    http://www.quirksmode.org/blog/archives/2010/04/a_pixel_is_not.html
    
  This is telling to the browser "my website adapts to your width".  IE. A the browser on a mobile device, regardless of its resolution, will zoom in to match a standard mobile resolution. 
  
  If you were to view a website without this meta tag, it would be extremely zoomed out. This also turns our earlier situation of designing for thousands of devices, to designing for a few.
  

(So this turns into this, switch slides between android fragmentation and viewports)  

- Show most common viewports
    - Mobile (Portrait) 320x480
    - Mobile (Landscape) 480x320
    - Tablet (Portrait) 768x1024
    - Tablet (Landscape) 1024x768
    - Desktop+
    - Retina Displays
    
    HOWEVER, do not design for content, design for viewports.  Best approach is a fluid design where you fix the design at breakpoints.
    - http://www.netmagazine.com/opinions/stop-designing-fixed-viewports
    
## Wireframing / Prototyping
- Best practice is to build mobile first.  It keeps everything simple, and helps establish content prioritization on the page.  I'm not going to go in depth on design processes for implementing a responsive design, but there are some important changes to the standard process.
  - Photoshop mockups, too time consuming.  Use a quick wireframing tool and use style tiles if clients need deliverables
  - Content and priortization, facilitate the user.  Important in standard web design, but crucial in responsive (might want to prove that)
  - Design in the browser: http://daneden.me/2011/09/design-in-the-browser/
  - OR DONT! http://www.andybudd.com/archives/2012/03/designing_in_the_browser_is_not_the_answ/
  
  Android touch guidelines (http://developer.android.com/design/style/metrics-grids.html)
  iPhone Touch guidelines
  - How loading time effects shopping: http://blog.kissmetrics.com/wp-content/uploads/2011/04/loading-time-lrg.jpg

## Page Layout

- Sample
  - I want to show my logo, my navigation, my latest blog post, my 5 most recent blog posts, archives.  In mobile, this is easy.  1 column, no problem. 
  - Tablet we have more real estate.  Let's bring the latest blog posts and archives up post up and move navigation to the right.
  - Desktop has much more space, lets do three columns.
  
  There are some common patterns that have emerged for common page elements.

## Navigation

- Dropdowns
- Show / Hide
- Select
- Slider

## Media

- Image serving and re-sizing techniques
- Bringing images into the design
- Embedding videos

## Content

- Mobile First approach
- Design considerations (paragraph length, modules/paragraph exceeding height, keep everything within the viewport.)
- Determine through analytics
- Hiding content

## Vector Icons!
http://www.awwwards.com/thousands-of-free-vector-icons-and-icon-webfonts-for-interfaces-and-responsive-web-design.html#vectoricons


!SLIDE slide x=0 y=0

## Grid Systems
- Skeleton
- Bootstrap Grid
- Golden Grid System

## Implementation
- You've wireframed out the different devices, now how do you build it?

## The World's Simplest Responsive Website

- I'm going to present to you the world's simplest responsive site.  (Show them one sentence website)  Looks great on any device.  Not very useful though.
- With media queries you can target the text and style it differently on different viewports.
        <h1>Hello World.</h1>
        
        @media (min-width: 480px) {
          
        }
        
        @media (min-width: 768px) {
          
        }
        
        @media (min-width: 960px) {
          
        }
- That is the starting point for responsive design


1.	Introduction (5 min)
a.	What is responsive design
A responsive design is one that has been created so it displays in a usable manner at any resolution (320+)
Image of apple devices showing a website.
2.	Should you have a responsive website? (10 min)
a.	Stats on mobile usage
i.	2014 mobile browser use will exceed desktop
b.	Stats on bounce rate of non responsive sites
c.	Associated costs
d.	Responsive vs Device specific
3.	Implementing a responsive design (30 min)
a.	Redesign considerations
b.	Content
i.	Priortization
c.	Breakpoints
i.	Mobile Device Outlines
d.	Responsive images
i.	Max-width
e.	Grids
i.	Bootstrap / gridset / skeleton / etc
f.	Type
i.	Fit text
g.	Tools / Frameworks
i.	Bones
ii.	Grids / Bootstrap / jQuery Mobile


Sources:
Google trends on responsive design search: http://www.google.com/trends/explore#q=responsive%20web%20design

http://www.mediapost.com/publications/article/184226/three-reasons-why-responsive-web-design-is-respons.html

http://googlemobileads.blogspot.ca/2012/09/give-mobile-users-what-they-want.html

http://usability.com/2012/04/24/compromise-happens/

Higher ed, usage stats: http://collegewebeditor.com/blog/index.php/archives/2012/09/11/2-more-reasons-why-the-responsive-web-design-approach-makes-sense-for-highered/

http://bradfrostweb.com/blog/mobile/content-parity/

http://bradfrost.github.com/this-is-responsive/patterns.html



