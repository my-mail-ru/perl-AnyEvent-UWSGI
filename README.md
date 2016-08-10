# NAME

AnyEvent::UWSGI - non-blocking UWSGI client (based on [AnyEvent::HTTP](https://metacpan.org/pod/AnyEvent::HTTP))

# SYNOPSIS

    use AnyEvent::UWSGI;
    uwsgi_get "uwsgi://example.com:3044/", headers => {Host => "example.com"}, sub { print $_[0] };

# DESCRIPTION

This module is an adaptation of AnyEvent::HTTP module for uwsgi protocol.
Subroutines prefixed by `http_*` (like request, get, post, head) replaced by appropriate subrountines with the prefix `uwsgi_*`.

# METHODS

- uwsgi\_request

    Like `AnyEvent::HTTP::http_request`

- uwsgi\_get

    Like `AnyEvent::HTTP::http_get`

- uwsgi\_head

    Like `AnyEvent::HTTP::http_head`

- uwsgi\_post

    Like `AnyEvent::HTTP::http_post`

# SEE ALSO

[AnyEvent::HTTP](https://metacpan.org/pod/AnyEvent::HTTP)

# COPYRIGHT

Copyright 2016 Alexander Kazakov.

This library is free software; you can redistribute it and/or
modify it under the same terms as Perl itself.
