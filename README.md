# blackfriday-text

A text renderer for the [blackfriday](https://github.com/russross/blackfriday) markdown processor.

### Usage

		import (
			"github.com/mschoch/blackfriday-text"
			"github.com/russross/blackfriday"
		)

		extensions := 0
		renderer := blackfridaytext.TextRenderer()
		output := blackfriday.Markdown(input, renderer, extensions)

### Why?

Why would you want to output markdown as text?  Isn't it already text?

Yes, but sometimes you want to remove the formatting.  For example, prior to feeding it into a text index, its helpful to remove the formatting characters.