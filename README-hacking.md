-*- outline -*-

These notes intend to help people working on the checked-out sources.
These requirements do not apply when building from a distribution tarball.

While building from a just-cloned source tree may require installing a
few prerequisites, later, a plain 'git pull && make' should be sufficient.

* First GIT checkout

You can get a copy of the source repository like this:

    $ git clone https://github.com/Boskovits/neon4j-test.git
    $ cd neon4j-test

The next step is to get and check other files needed to build,
which are extracted from other source packages:

    $ ./bootstrap
    
And there you are! Just

    $ make
    $ make check

At this point, there should be no difference between your local copy,
and the GIT master copy:

        $ git diff

should output no difference.

Enjoy!

-----

Copyright (C) 2017 Gábor Boskovits

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU Affero General Public License as
    published by the Free Software Foundation, either version 3 of the
    License, or (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU Affero General Public License for more details.

    You should have received a copy of the GNU Affero General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.