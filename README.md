# Montogue Bridge Widget
Widget to embed into websites tracking https://howmanydayssincemontaguestreetbridgehasbeenhit.com/

Website is not mine, it is a Melbourne classic and everyone should be aware of it. All love and gratitude to the creator of the website. I use their work/api to make this widget work.

Place the below code into any website or download the widget above and update the code below to reflect the new URL where the widget is

<iframe
  src="https://acetaylor.dev/scripts/widget.html"
  title="Days since Montague St Bridge was last hit"
  width="320"
  height="230"
  style="border: none; max-width: 100%;"
  loading="lazy"
></iframe>

The iframe's fetch() calls to /api/chumps/ are relative to acetaylor.dev, NOT the embedding page's domain — so they stay
same-origin and work with zero CORS configuration. This is the main reason to use an iframe instead of injecting the widget's HTML/JS directly into a foreign page.

Resize the iframe's width/height to taste; the widget itself is responsive up to a max-width of 320px.

If you'd rather NOT use an iframe (e.g. you want the widget to inherit the host page's fonts/theme), you'll need a script-tag version instead, which requires enabling CORS on /api/chumps/ (Access-Control-Allow-Origin header) since that fetch would then run from the embedding page's own origin.

I haven't currently built that but if people want it, I'm happy to do so.
