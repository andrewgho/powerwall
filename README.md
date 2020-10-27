powerwall - monitor local Tesla Powerwall
=========================================

This program runs in the background to continuously poll the local JSON
endpoint exposed by a Tesla Powerwall. It collects the grid power status,
remaining battery capacity, and power wattage flows between grid, solar,
Powerwall battery, and home load; records the data as tab-separated
timeseries data values, and keeps a JSON file up to date with the most
recent state (that JSON file can be used in turn to answer REST API
requests for upstream systems).

Usage
-----

    % powerwall -o program.log -d data.txt -s /htdocs/data.json 1000000-00-X--XX10000000000X

References
----------

* [Connecting to Tesla Gateway](https://www.tesla.com/support/energy/powerwall/own/monitoring-from-home-network)
* [Tesla Powerwall 2 - Local Gateway API documentation](https://github.com/vloschiavo/powerwall2)

Author
------

Andrew Ho <andrew@zeuscat.com>

License
-------

Tesla and Powerwall are registered trademarks of Tesla, Inc.
Tesla, Inc. does not sponsor, authorize or endorse this codebase.
The files in this repository are authored by Andrew Ho, and are covered by
the following MIT license:

    Copyright 2020 Andrew Ho

    Permission is hereby granted, free of charge, to any person
    obtaining a copy of this software and associated documentation
    files (the "Software"), to deal in the Software without
    restriction, including without limitation the rights to use, copy,
    modify, merge, publish, distribute, sublicense, and/or sell copies
    of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be
    included in all copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
    EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
    MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
    NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
    HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
    WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
    DEALINGS IN THE SOFTWARE.
