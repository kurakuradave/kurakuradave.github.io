---
layout: default
---

# ChorusText

ChorusText is an assistive device that lets a blind/low-vision person do text-editing, simply by means of touch and hearing alone.

## Why ChorusText

Text-editing is a sight-led activity. To be able to do it well, one must be able to:
1. locate the cursor's position on the screen
2. read the text around the cursor to gain an understanding of where s/he is in the text

Both of these are done using eyesight, and if one has poor or no eyesight, it can be tough.

This project is trying to find a solution to text-editing that is completely independent of eyesight.
To achieve this, we're tapping on the senses of touch and hearing.

To read the text, instead of staring at a monitor, the user drags some sliders and listen to synthesized speech of the text.

When the user types, instead of characters appearing/disappearing on the monitor, the sliders reposition themselves to manifest a physical representation of the text.

[This video shows the device in action:](https://www.youtube.com/watch?v=rKKQ0PMU3hs)

## How It Works

On the surface of the device, there are three physical sliders that the user can reach out to at any time.

Changing the position of the slider would cause the system to pull out the corresponding part of the text and speaks the content out loud, using text-to-speech.

So changing the position of the line slider's knob from top to bottom will result in the system reading the text progressively line by line.

And changing the position of the word slider knob from left to right will result in the system reading the words in the current line, progressively word by word.

And likewise, changing the position of the character slider knob from left to right will result in the system spelling the letters of the current word, in the current line, progressively letter by letter.

This way, the user can read the text he's working on with ease, and can drill down to the level of characters effortlessly, which is critical when spell-checking.

Furthermore, as the user types, the sliders continuously reposition themselves to physically manifest the latest state of the text and where the user is in the text.

If he adds two more characters to the current word, the character slider would move two steps to the right.
If he adds three words to the line, the word slider would move three steps to the right.
Deleting the current line would make the line slider to move one step up, and so on.

The cursor is no longer an abstract blinking thing, that only lives inside the monitor, where the only way to locate its position is by means of eyesight.

It is now physically manifested by the three sliders.

Simply reach out to the sliders with your hand and listen, the text is immediately accessible and navigable – no eyesight required.

## What It's Made From

ChorusText is built from Arduino, Linux Single-board-computer motorized sliders push-buttons and some basic electronic components

### [The repository is here](http://www.github.com/kurakuradave/chorustext)
Contains hardware design files as well as software source codes

### [ChorusText on Hackaday.io](https://hackaday.io/project/6142-chorustext)
Listed as Quarterfinalist in the Hackady Prize 2015 competition

## What's Next?

There's another open source project called [emacSpeak](http://emacspeak.sourceforge.net/), which has integrated emacs with a text-to-speech system, such that, as the user types, the TTS picks up the text and speaks it out loud.
Next step for ChorusText is to explore how to integrate it with the emacSpeak software, such that ChorusText becomes the hardware / physical manifestation of the text in the emacs buffer.
[Emacs](https://www.gnu.org/software/emacs/) is a major Linux text-editor software originally developed by Richard M. Stallman.

