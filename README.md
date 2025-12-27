# PICwatch
A wristwatch based on a PIC microcontroller.

# Description
<p>I was browsing Aliexpress and came across some retro looking 7 segment displays which combined with the fact that most PIC microcontrollers have a timer module with a dedicated independent 32.768kHz oscillator (which makes for a perfect RTC) inspired me to make my own wristwatch with the quirk being that the only integrated circuit will be a PIC mcu!</p>

# Work in progress
<p>Right now I'm testing on a breadboard while waiting for some parts to arrive and the only things implemented are the LED multiplexing and the once per second interrupt from the timer <del>using the main oscillator as I still need to get some appropriate crystals for the dedicated oscillator</del>. Added the external cystal for the dedicated oscillator and working on the UART time sync. Also did a little optimization on the interrupt routine (mainly because it was downright stupid before) so now it runs fast enough to not be noticeable when using the LFINTOSC at 31kHz.</p>
<p>I'm still working out the features but I plan for the final version be simmilar to the classic F91W but with some neat features like a rechargeable battery and time syncing through UART while it's charging (no more fiddling with buttons!) and anything else that comes to mind and seems like a good idea.</p>

# License
<p>This project is licensed under the MIT NON-AI License which can be found here: <br>
<a href="https://github.com/non-ai-licenses/non-ai-licenses"> https://github.com/non-ai-licenses/non-ai-licenses </a> <br>
Credit to <a href="https://github.com/axel22"> axel22</a>.</p>
