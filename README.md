# Directory File Parsers #

## Requirements ##

* [Audio::Scan](http://search.cpan.org/~agrundma/Audio-Scan-0.87/lib/Audio/Scan.pm)
* Perl. I'm not going to explain how to get it.

## Usage ##

Invoke a file format script suitable for the media in your files, pipe to sort if necessary.

## Roadmap / Wishlist ##

* Suitable framework for detecting file-formats, both dumbly (by extension) and smartly (by file magic/mimetype), turning this into just a single script.
* Seemless `pbcopy` integration into OS X environments.
* Smart artist display, automatically when "Various Artists" is seen, or when differing artists are detected on tracks.

--------

# Bandcamp Parser #

## Requirements ##

* Perl >= 5.10. I'm not going to explain how to get it nor upgrade to it.
* [URI](http://search.cpan.org/~gaas/URI-1.59/URI.pm)
* [LWP::Simple](http://search.cpan.org/~gaas/libwww-perl-6.03/lib/LWP/Simple.pm)
* [JSON](http://search.cpan.org/~makamaka/JSON-2.53/lib/JSON.pm) >= 2.0 (JSON::XS generally recommended, additionally.)
* [DateTime](http://search.cpan.org/~drolsky/DateTime-0.70/lib/DateTime.pm)
* [DateTime::Format::Duration](http://search.cpan.org/~rickm/DateTime-Format-Duration-1.03a/lib/DateTime/Format/Duration.pm)

## Usage ##

Visit a bandcamp URL, a specific album or even track as part of an album. Copy the URL and paste it into a terminal as an argument to the bandcamp script.

Ex. `perl bandcamp.pl "http://rainbowdragoneyes.bandcamp.com/track/seize-my-day"`

Artists with only one Album/Track will have that information automatically printed. Otherwise a track will be resolved back to it's release, or printed as-is. An album will be printed as-is. And artist URL with multiple albums will list albums and URLs suitable for immediately copying back into execution.

## Roadmap / Wishlist ##

* Refactor
* Refactor
* Refactor
