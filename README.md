#embedTwitchCSS

## Synopsis

Embedding a twitch stream on an external site with the tiwtch provided code leaves a lot to be desired. This is a simple style sheet that let's you easily drop in a responsive twitch stream & chat while maintaining a proper 16:9 video ratio. In the example I've put the stream and chat next to each other and set the width to be 75% and 25% respectfully. Obviously you should adjust those to your liking, the stream will maintain 16:9 regardless of it's width. I also included a default media query that hides the chat if the screen gets too small. You should adjust that trigger to your needs as well.

an example is up and running here: http://jcrastelli.com/projects/embedTwitchCSS/

## Code Example

To use as is, **download embedTwitchCSS.css** and link the style sheet to your page 

'''
<link rel="stylesheet" href="**YOUR-FILE-STRUCTURE**/embedTwitchCSS.css" />
'''

then put two divs **twitchStream** and **twitchChat** inside the **twitchWrapper** on your page.

'''
<div class='twitchWrapper'>
	<div class='twitchStream'>
		<iframe src="https://player.twitch.tv/?channel=**YOUR-CHANNEL-NAME**" frameborder="0" scrolling="no"></iframe>
	</div>
	<div class='twitchChat'>
		<iframe frameborder="0" scrolling="no" src="https://www.twitch.tv/**YOUR-CHANNEL-NAME**/chat"></iframe>
	</div>
</div>
'''

and you should be ready to rock!

I'd suggest you edit the width ratio between twitchStream and twitchChat and the media query trigger as per your needs. And if you're using another library to handle widths just drop the width property from those two elements entirely.

## Installation

Either download the whole project to get the implementation example index.html file or simple just download the embedTwitchCSS.css file within the css folder

## Contributors

If anyone notices anything wonky or has any suggestions I'm all ears

Big thanks to http://www.mademyday.de/css-height-equals-width-with-pure-css.html for the help with the 16:9 calculations and set up. This borrows heavily from them

## License
MIT License

Copyright (c) 2016 Gregle

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.