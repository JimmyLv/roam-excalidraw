# roam-excalidraw
The Roam Research Excalidraw plugin

If you are still using roam-excalidraw and find it is not working, it should be because the domain http://roam-excalidraw.com is expired 🤣 

Thanks @zsviczian for the awesome work, and I just forked and deployed it to @Vercel, you can change the js URL to https://roam-excalidraw.vercel.app/dist/loader.js

## Step 1 — Enable custom components.

![image](https://user-images.githubusercontent.com/4997466/208887197-ce54d469-5376-448e-b7f8-d4c1468cfe00.png)

## Step 2 — Add a new JavaScript block on the roam/js page & Enable the plugin.

{{[[roam/js]]}}

```js
{
  let s = document.createElement('script');
  s.type = 'text/javascript';
  s.src = 'https://roam-excalidraw.vercel.app/dist/loader.js';
  s.async = false;
  document.getElementsByTagName('head')[0].appendChild(s);  
}
```

## Step 3 - Use roam/templates to start drawing.

Enabling the plugin creates a Roam template for you automaticlly.

Simply type `;;excalidraw` and hit Enter to insert a new canvas anywhere you like:

![image](https://user-images.githubusercontent.com/4997466/208887812-54ad0c33-2dbe-44e2-bfc2-9fcaedaa6c2d.png)

ref: [Create Diagrams and Drawings in Roam Using Exalidraw](https://thinkstack.club/diagrams-and-drawings-in-roam-exalidraw/)
