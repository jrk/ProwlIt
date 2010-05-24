Prowl! bookmarklet
==================
This simple Javascript pushes a message containing the title and URL of the currently displayed web page to your iPhone OS devices via the [Prowl](http://prowl.weks.net) service. It is meant to be compiled into a bookmarklet like:

> <a href="javascript:var%20http%20=%20new%20XMLHttpRequest();var%20url%20=%20%22https://prowl.weks.net/publicapi/add%22;var%20apikey%20=%20%XXXX%22;var%20application%20=%20%22the%20web%22;var%20evt%20=%20%22Browser!%22;var%20description%20=%20encodeURIComponent(document.title.replace(/^\s*|\s*/g,%27%27))+%20escape(%22\n%22)%20+%20encodeURIComponent(location.href);var%20params%20=%20%22apikey=%22+apikey+%22&application=%22+escape(application)+%22&event=%22+escape(evt)+%22&description=%22+description;http.open(%22POST%22,%20url,%20true);http.setRequestHeader(%22Content-type%22,%20%22application/x-www-form-urlencoded%22);http.send(params);">Prowl!</a>

It is meant for quickly pushing items from a PC browsing session to a mobile device like an iPhone or iPad.

To use, replace the API key "XXXX" in the bookmarklet string with your Prowl [API Key](https://prowl.weks.net/settings.php) before using.