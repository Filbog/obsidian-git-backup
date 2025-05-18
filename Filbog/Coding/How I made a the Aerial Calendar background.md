09-01-2025

AKA image with a transparent background that I combined with CSS background-color property

1. Generate the image from the Bootstrap Icon via ChatGPT and save it
2. I didn't specify it has to have transparent BG in ChatGPT, (it's capable of doing it) so I used this tool for transparent background: https://onlinepngtools.com/create-transparent-png
3. I set the image's opacity in Pixlr (or any other semi-advanced image editor)  - we can't set it in CSS for backgrounds, at least not in a straightforward way
4. I used those properties on my body:
   ```CSS
   background: url('/static/images/transparent-bg-even-more-opaque.png'), var(--background);

background-attachment: fixed;

background-position: center;

background-repeat: no-repeat;

background-size: contain;
```
 And voila, it worked! End result:
 https://github.com/Filbog/aerial-calendar/

### Hashtags:
#coding #webdev #styling #css #django


### References (source material, similar notes):
