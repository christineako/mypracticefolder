1. htaccess Rewriting URL to include variables
RewriteRule ^office-spaces-for-rent/([0-9a-zA-Z]+) rental-office-details.php?u=$1 [NC,L]

QUESTION: URL could be successfully re-written but no data is passed



2. htaccess 301 Redirect
# FORCE https://www in URL
RewriteCond %{HTTP_HOST} ^eastwoodcondo.com
RewriteRule (.*) https://www.eastwoodcondo.com/$1 [R=301,L]

# Permanent URL redirect
Redirect 301 / https://www.eastwoodcondo.com
Redirect 301 /old-page.html https://www.eastwoodcondo.com

QUESTION: Which is the correct rewrite to use. What is the difference



3. Adding Whatsapp button with current URL

<a href="https://api.whatsapp.com/send?phone=639205202222&text=Hello%2C%20I'm%20in%20www.eastwoodcondo.com%20now.">Whatsapp</a>

QUESTION: How to capture and insert URL


4. Adding Twitter share button with current URL 
<a class="twitter-share-button"
  href="https://twitter.com/intent/tweet?text=https://www.eastwoodcondo.com"
  data-size="large">
Tweet</a>

QUESTION: How to capture and insert URL


5. Adding FB share button with current URL and Whatsapp
<!-- Load Facebook SDK for JavaScript -->
<div id="fb-root"></div>
<script>(function(d, s, id) {
var js, fjs = d.getElementsByTagName(s)[0];
if (d.getElementById(id)) return;
js = d.createElement(s); js.id = id;
js.src = "https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v3.0";
fjs.parentNode.insertBefore(js, fjs);
}(document, 'script', 'facebook-jssdk'));</script>

<!-- Your share button code -->
<div class="fb-share-button" 
  data-href="https://www.eastwoodcondo.com" data-layout="button_count">
</div>

QUESTION: How to capture and insert URL


6. Compressing files size before uploading image

file: imageupload.php

QUESTION: How to modify code to make it multiple files in one upload



