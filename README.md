# Integration

There are three pieces of code you need to add to your web page.

## HTML Element

    <div id="fling_uploader"></div>

Put this in your page's HTML where you'd like it to show up.

## Script

    <script src="http://source/assets/uploader.js"></script>

## Config

    <script type="text/javascript">
      fling.config.announce = "http://localhost:9050/announce"
      fling.config.session_id = "identify_this_user_uploads"
    </script>

When an upload is complete, you'll be notified of it at the url you set
`fling.config.announce` to.

## Server

After a user's fully uploaded their file, you will be notified at the location
you've configured. This request will be a list of URLs that you can download
from.
