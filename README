edcast_jack special edition!
===========================

It's just like the old edcast you know and love, only a bit leaner and 
supporting of streaming 24bit flac from jack!

If your going to stream oggflac, look out!

With my fixes, I reccomend mplayer as the client, with a small buffer..

mplayer -cache 500 http://xxxxxxxxxx

VLC also works however it can eventually run into some kind of buffer/stutter issue

Please be advised of this: http://lists.xiph.org/pipermail/flac-dev/2010-December/002825.html

And then go here: https://github.com/oneman/libflac/commit/67e13364032404ebc1837af143fdd1cd81786c3a

features added
--------------

24 bit flac support   -b 24 on the command line

features to come: correct flushing of ogg packets to prevent buildup of silence in pages

Currently this is hackfixed and handled by flushing every packet, probably sending way to many out over
the network. this should be fixed by counting samples and flushing after X number of samples

minor changes: correct printing of server port number, removal of deprecated jack_new call



features removed
----------------

windows support, resampling support, metadata support


windows?      are you kidding me? did it even work ever?

resampling?   Did you not have jack set at the sample rate you really wanted?

metadata?     OggFLAC doesn't support any in the case of streams in anything Ive seen
              Most software doesn't support chained ogg ie. firefox/chrome/cortado
              if you want metadata, use a different program to talk to icecast2
              that makes the most sense, if you think about it for a moment.. 
              (also it never worked well anyway)



