MonkeyMachine — Icon Pack

Files:
- favicon.ico                         # multi-size favicon (16/32/48/64/128/256)
- apple-touch-icon.png (180x180)      # iOS home screen
- site.webmanifest                    # PWA manifest
- maskable_icon-*.png                 # PWA icons (maskable)
- logo-*.svg                          # SVG variants with explicit sizes

How to integrate (HTML <head>):

<link rel="icon" href="/favicon.ico" sizes="any">
<link rel="apple-touch-icon" href="/apple-touch-icon.png" sizes="180x180">
<link rel="manifest" href="/site.webmanifest">

# Optional (if you want PNG fallbacks in addition to ICO):
<link rel="icon" type="image/png" sizes="48x48" href="/maskable_icon-48x48.png">
<link rel="icon" type="image/png" sizes="96x96" href="/maskable_icon-96x96.png">
<link rel="icon" type="image/png" sizes="192x192" href="/maskable_icon-192x192.png">
<link rel="icon" type="image/png" sizes="512x512" href="/maskable_icon-512x512.png">

Notes:
- Icons have transparent background and are centered on a square canvas.
- PWA icons include `purpose: "any maskable"` for 192 & 512 sizes.
- Adjust `theme_color` and `background_color` inside site.webmanifest if needed.


Safari pinned tab:
<link rel="mask-icon" href="/safari-pinned-tab.svg" color="#6C4DFF">

Windows tiles (old Edge/IE):
<meta name="msapplication-TileColor" content="#0B1220">
<meta name="msapplication-config" content="/browserconfig.xml">
