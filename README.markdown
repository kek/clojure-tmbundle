# Clojure.tmbundle

## Prerequisites

The Clojure bundle depends on the following external utilities to work:

* bash
* ruby
* osascript

If either of those aren't on your Textmate's PATH, these commands will fail in unknown and spectacular fashion.

Additionally, if clj is not found on your Textmate's PATH, then it will use the one included in this bundle. You can manually specify it with the TM_CLJ variable.

## Installation

Run this:
 
	$ cd ~/Library/Application\ Support/TextMate/Bundles
	$ git clone git://github.com/kek/clojure-tmbundle.git Clojure.tmbundle
	$ osascript -e 'tell app "TextMate" to reload bundles'

An update script will :

* Get Clojure and Clojure-contrib from Github.
* Get library for generating off-line documentation from Github.
* Build Clojure and documentation.

Run this :

	$ ./Clojure.tmbundle/Vendor/clj-update-and-build
