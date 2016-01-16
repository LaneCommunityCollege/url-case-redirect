# url_case_redirect

If your server serves content regardless of url case, and due to a specific caching setup you can't just fix this via apache config, then you may be looking for this module.

This module watches for mixed case paths, checks to see if the url exists, and if it does, sends a 301 to the lowercase version.