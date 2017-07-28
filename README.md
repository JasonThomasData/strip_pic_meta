### CLI to strip data from images.

I made this one page CLI as an easy way to strip exif (and other) metadata from pics, because I'm sceptical of what
companies like Facebook and others are likely to do with it.

Most phone cameras will save metadata in pics when the pics are taken. Most JPG-PNG converters will
drop the metadata, and yet you can still add metadata to pics manually. I want an easy way to strip
metadata from pics.

Some cameras will save the GPS coords, the time taken, details about the phone, etc. If you've taken
a photo of your children with these details, then obviously that's scary right?

This issue is portrayed in a rather humorous example of how revealing metadata can be, called [I
know where your cat lives](http://iknowwhereyourcatlives.com/about/)

This program loads an image as a object of pixels, and then saves them again. Everything other than
the pixels is lost.

To make this easy to use, I saved my program in /usr/local/bin/

TO DO
- Make the program accept an -r arg, to process the entire folder.
- Make the program accept target output destination.
