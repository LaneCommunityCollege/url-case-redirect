# url_case_redirect

If your server serves content regardless of url case, but you can't simply redirect case using Apache config, then you may be looking for this module.

This module watches for mixed case paths, checks to see if the url exists, and if it does, sends a 301 to the lowercase version.

It also checks the request_uri. If that ends in a trailing slash, it runs it through the same function, since redirecting to the request path automatically trims the trailing slash off.