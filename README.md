Secured apache headers with Mod-headers
    
    Header always set Access-Control-Allow-Origin "https://website.com"
    Header always set Strict-Transport-Security "max-age=31536000; includeSubdomains;"
    Header set X-XSS-Protection "1; mode=block"
    Header set X-Content-Type-Options "nosniff"
    Header always set Access-Control-Expose-Headers "Content-Security-Policy, Location"
    Header always set Content-Security-Policy "default-src https: wss: data: 'unsafe-inline' 'unsafe-eval';frame-ancestors 'self';object-src 'self';script-src 'unsafe-inline' 'unsafe-eval' 'self' maps.googleapis.com stackpathcdn.com static.zdassets.com google.com api.eu-1.smooch.io static.zdassets.com cdn.ckeditor.com oss.maxcdn.com d3js.org gyrocode.github.io ws.sharethis.com netdna-ssl.com hotjar.com c64.assets-yammer.com unpkg.com ajax.googleapis.com googleapis.com www.google-analytics.com google-analytics.com code.jquery.com cdnjs.cloudflare.com cdn.jsdelivr.net gstatic.com vimeo.com stats.g.doubleclick.net googletagmanager.com cdn.tiny.cloud cdn.datatables.net maxcdn.bootstrapcdn.com momentjs.com stackpath.bootstrapcdn.com clubandalbrok.com www.clubandalbrok.com;img-src data: blob: 'self' *.googleapis.com *.gstatic.com *.googleusercontent.com static.zdassets.com *.tinymce.com *.eulen.com *.google.com *.google-analytics.com *.google.es code.jquery.com cdnjs.cloudflare.com cdnbigbuy.com"
    Header set X-Frame-Options SAMEORIGIN
    Header always set Referrer-Policy "strict-origin"
    Header always set Permissions-Policy "accelerometer=(),gyroscope=(),magnetometer=(),microphone=(),midi=(),payment=()"
