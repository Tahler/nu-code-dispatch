The front facing web server for [NU Code](http://code.neumont.edu), which serves as a proxy to all
of the needed services to run the site.

The Dispatch runs in an Nginx container utilizing the nginx.conf file to proxy between the
[Compilation API](https://github.com/Tahler/nu-code-compilation-api) (/api), the
[Submission API](https://github.com/Tahler/nu-code-submission-api) (/submit), and
[the front end website](https://github.com/Tahler/nu-code-web) (/**).

![diagram](https://raw.githubusercontent.com/Tahler/nu-code-dispatch/master/doc/flow-diagram.png)

The diagram above uses horribly scaled arrows to demonstrate the HTTP request flows of the
application.
