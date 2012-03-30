Pontoon
=======
This is a proof-of-concept implementation of an in-place website localization tool, as [outlined by Austin King][outline]. Please note that Pontoon is in a very early alpha version, under heavy development, and unlikely to do much out of the box. If you are interested in the technology, feel free to step by `#pontoon` on <irc://irc.mozilla.org> or get more information from a [wiki][wiki].

Pontoon.jpg contains a schema of the application's components.

Dependencies
------------
* Apache
* PHP
* Django 

Usage
-----
Web client:

* Map /pontoon on a web server to the root of this project.
* Point your browser to /pontoon.
* Click on the Demo link.

Django server ([Django][django] is required):

* `cd server`
* `python manage.py runserver 0.0.0.0:8000`

To use Microsoft Translator API for machine translation, obtain a valid API key from the [Bing Developer Center][bdc] and store it in a variable Pontoon._app._mt in your local JS settings file client/lib/js/local-settings.js.

Store Pontoon client path in the $path variable in your local PHP settings file hook/php/local-settings.php.

Contributors
------------
* Matjaž Horvat <matjaz@mozilla.com>
* Frederic Wenzel <fwenzel@mozilla.com>
* Zbigniew Braniecki <gandalf@mozilla.com>
* Austin King <aking@mozilla.com>

License
-------
    ***** BEGIN LICENSE BLOCK *****
    Version: MPL 1.1/GPL 2.0/LGPL 2.1

    The contents of this file are subject to the Mozilla Public License Version 
    1.1 (the "License"); you may not use this file except in compliance with 
    the License. You may obtain a copy of the License at 
    http://www.mozilla.org/MPL/

    Software distributed under the License is distributed on an "AS IS" basis,
    WITHOUT WARRANTY OF ANY KIND, either express or implied. See the License
    for the specific language governing rights and limitations under the
    License.

    The Original Code is Pontoon.

    The Initial Developer of the Original Code is
    Frederic Wenzel <fwenzel at mozilla dot com>.
    Portions created by the Initial Developer are Copyright (C) 2009
    the Initial Developer. All Rights Reserved.

    Contributor(s):

    Alternatively, the contents of this file may be used under the terms of
    either the GNU General Public License Version 2 or later (the "GPL"), or
    the GNU Lesser General Public License Version 2.1 or later (the "LGPL"),
    in which case the provisions of the GPL or the LGPL are applicable instead
    of those above. If you wish to allow use of your version of this file only
    under the terms of either the GPL or the LGPL, and not to allow others to
    use your version of this file under the terms of the MPL, indicate your
    decision by deleting the provisions above and replace them with the notice
    and other provisions required by the GPL or the LGPL. If you do not delete
    the provisions above, a recipient may use your version of this file under
    the terms of any one of the MPL, the GPL or the LGPL.

    ***** END LICENSE BLOCK *****

[outline]:  http://ozten.com/psto/2009/08/14/a-sketch-of-po-liveedit/   "A Sketch of PO LiveEdit"
[wiki]:  https://wiki.mozilla.org/L10n:Pontoon   "L10n:Pontoon - MozillaWiki"
[bdc]: http://www.bing.com/developers/createapp.aspx   "Bing Developer Center"
[django]: https://www.djangoproject.com/   "Django"
