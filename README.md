Download Link: https://assignmentchef.com/product/solved-virtual-think-a-dot-in-visual-basic
<br>
In my youth, long before personal computers, there was a company called E.S.R., Inc. that satisfied my desire to possess a computing device. They had three offerings: DR. NIM, DIGI-COMP I, and THINK-A-DOT. I owned them all, but my personal favorite was THINK-A-DOT. At the time it cost a mere $2.95, which was well within my monthly allowance. I recently saw one selling on eBay for $120. Since I no longer own my original machine, and cannot afford to replace it, I would like you to build me a virtual THINK-A-DOT in Visual Basic.

<img decoding="async" alt="" data-recalc-dims="1" data-src="https://i0.wp.com/d2vlcm61l7u1fs.cloudfront.net/media%2F5ca%2F5cae45b3-48d2-49e7-bbaf-663b10591515%2FphpNTDAlI.png?w=980" class="lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" src="https://i0.wp.com/d2vlcm61l7u1fs.cloudfront.net/media%2F5ca%2F5cae45b3-48d2-49e7-bbaf-663b10591515%2FphpNTDAlI.png?w=980" alt="" data-recalc-dims="1">

 </noscript>




As originally constructed, a marble could be dropped into one of three holes in the top of the machine. It would then percolate through the machine and come out a hole on the bottom left or right. This was to allow for two-person competition, and really was of no interest to me. As the marble percolated through the machine it caused any dot it passed to change color from yellow to blue, and from blue to yellow. The color of the dot also controlled whether the marble would fall to the left (yellow) or to the right (blue). This meant there were ten possible paths through the machine from top to bottom, flipping either two or three dots to their alternate colors along the way. The initial pattern could be reset at any time by tilting the machine to the left or right.

<strong>      ThinkaDot.exe</strong> provides a working example, if the following explanation is hard to understand. For your virtual machine, you will need some way to reset all the dots to yellow, some way to indicate the initial starting point of a virtual marble (left, middle, or right), and some way to represent the eight dots and change their color from yellow to blue or from blue to yellow. The logic is such that after changing a dot from yellow to blue, the next dot to be reversed is down and to the left. For a blue dot changing to yellow, the next dot to be reversed is down and to the right. A virtual marble dropping down the far left or far right side will only reverse two dots and not three. The folder, <strong>ThinkaDot</strong>, contains the start of a solution. It provides a picture of the machine, and a <strong>flipper</strong> control that can be dragged onto the picture just like any other control. The flipper control has a Boolean property, <strong>droppedLeft</strong>, that tells you the direction the ball fell; and two methods: <strong>flip</strong> that reverses the control, and <strong>reset</strong>.




A useful property of Think-a-Dot that can be used for testing, is that a marble dropped into any one of the three holes at the top, eight times in a row, will return the machine to the original pattern. Also, dropping a marble into each of the holes twice will return the machine to the original pattern.