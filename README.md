# paper-clock 

Ultra low power E-paper clock that attaches to Quadlock bike mount.

### Motivation

These days, everyone has a smart phone to look at the clock so the clocks in the
"environment" have largely disappeared. Very understandable. However, when I'm
biking, I often need to know what time it is and I can't just pull my phone out
mid-pedal to check. I have a [Quadlock bike mount](https://www.quadlockcase.com/collections/shop-cycle/products/products-bike-kit-universal-fit)
that I use regularly if I'm navigating with the phone. If I'm not though, the
phone is in my pocket or a bag.

To fix this issue, I want a clock that I can attach "statically" (basically,
it's there whenever my phone isn't) to my Quadlock mount that draws as little
power as possible.

### Design

An E-paper screen that shows the current time. The screen is always off unless a
button is pressed. An ATTiny85 MCU keeps track of the time with an accuracy of 1
minute. When the button is pressed (i.e. held down), the ATTiny tells the screen
to render the current time.
