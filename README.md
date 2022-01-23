pd-ffmplay~
=========
binaries of the ffmplay~ external for PureData by myQwil
https://github.com/myQwil/pdxtra

The FFmpeg (version 4.4.1) libraries are dynamically linked to the builds provided, which means that you'll need a local installation of these libraries in order for the external to work. A package manager is probably the ideal way to install them. Otherwise, they are available at ffmpeg.org/download.html, just be sure to get the "Shared" builds, and place them in a location where the external is able to find them.


Features:
====

* play/pause and seek functionality
* changing the speed of playback
* reading and iterating through m3u playlists
* opening files from http urls.
* retrieving metadata
* specifying additional channels as creation args for files with surround sound.
* In the help file, you'll notice ffplay~ has the creation arguments 1 2 5 6.
The 5 and 6 represent rear-left and rear-right channels.
A full list of available channels can be found here: github.com/FFmpeg/FFmpeg/blob/master/libavutil/channel_layout.h

Pd win64 dependencies:
====
Dependencies for Windows could be found here: https://www.gyan.dev/ffmpeg/builds/packages/ffmpeg-4.4.1-full_build-shared.7z

Put those files from the bin folder along with the ffplay~.m_amd64 file:  

avcodec-58.dll  
avformat-58.dll  
avutil-56.dll  
swresample-3.dll  

Pd macOS64 dependencies:
====
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew install ffmpeg

Linux dependencies:
====

apt-get install ffmpeg
