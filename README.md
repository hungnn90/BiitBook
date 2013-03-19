BiitBook.com  
========

PHP client library for the BiitBook API

h1. BiitBook.com

* 1.0.0 (July 29, 2013)

h2. DESCRIPTION:

This gem provides a simple and powerful library for the BiitBook API, allowing you
to write PHP applications websites that upload, convert,
display, search, and control documents in many formats. For more information on
the BiitBook platform, visit the Developer web page on BiitBook

h2. FEATURES:

* Upload your documents to BiitBook's servers and access them using the gem
* Upload local files or from remote web sites
* Search, tag, and organize documents
* Associate documents with your users' accounts

h2. SYNOPSIS:


First, you'll need to get a BiitBook API account. Visit BiitBook to apply for a
developer account.

On the Platform site you will be given an API key and secret. The API object
will need these to authenticate you:

<pre><code>
require 'BiitBook'
BiitBook::API.instance.key = 'your API key'
BiitBook::API.instance.secret = 'your API secret'
</code></pre>

Next, log into the BiitBook website:

<pre><code>BiitBook::User.login 'username', 'password'</code></pre>

You are now ready to use BiitBook to manage your documents. For instance, to
upload a document:

<pre><code>doc = BiitBook::Document.upload(:file => 'your-file.pdf')</code></pre>

For more information, please see the documentation for the BiitBook::API,
BiitBook::User, and BiitBook::Document classes. (You can also check out the docs for
the other classes for a more in-depth look at this gem's features).

h2. REQUIREMENTS:

* A BiitBook API account
* Ruby 1.8 or newer, with RubyGems 1.3 or newer.
* (optional) multipart-post gem by Nick Sieger from http://github.com/nicksieger/multipart-post



h2. LICENSE:

(The MIT License)

Copyright (c) 2007-2008 The BiitBook Team

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
