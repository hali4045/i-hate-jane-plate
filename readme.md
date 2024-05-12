# i hate jane plate

https://janeplate.hali.studio

## what is it 
jane plate files that i made from scratch for people to use for cad. also functional for production 

## why did i do this 
the version of the jane plate in the [v2 ce's geekhack comments](https://geekhack.org/index.php?topic=100415.msg2785585#msg2785585) SUCKS and has a lot of dumb numbers in it that don't line up 
![image](https://github.com/hali4045/i-hate-jane-plate/assets/66137164/7881b309-d957-4dbb-9130-527e79ef1b0d)
![image](https://github.com/hali4045/i-hate-jane-plate/assets/66137164/754e5c46-a0e1-4f15-87c5-a6ea05b05195)

i just wanted a version that would work without me yelling at it every 2 seconds because two allegedly parallel lines are at an angle that has to be expressed in scientific notation or an entire row is 0.05 mm below where it should be or some other dumb reason that has to exist in this 5 year old keyboard 

## patch notes 
- no more infinitesimally small angles
- 0.5 mm radius internal fillets instead of 1 mm
- added compatibility for both north and south facing stabs on spacebar
- bottom row is ACTUALLY the same height as the bottom arrow keys now (how was this ever a problem) 
- separated ansi and iso into their own plates
- claw mounting point holes do not extend towards switch cutouts as far
- convex fillet radii on mounting points changed to 1.5 mm instead of 1 mm to allow for 3 mm tools during case machining
- usb cutout fillets at f12/f13/prt sc changed to 0.5 mm from 1 mm because i think they look nicer
- corner chamfers filleted over 0.5 mm just to be nice 

## how did i do this 
first step was to create a layout to throw in a plate gen 
![image](https://github.com/hali4045/i-hate-jane-plate/assets/66137164/9321e3ca-6d7c-4f0b-9bbc-c8e2d2656bf0)

i used [plate.keeb.io](https://plate.keeb.io) for this project, although in hindsight, [ai03's](https://kbplate.ai03.com/) might have been better because of the stab cutouts i wanted 
![image](https://github.com/hali4045/i-hate-jane-plate/assets/66137164/b9e33e32-694a-4a2a-b9eb-470698d479af)

_whatever, it's in autocad now_

keebio plate gen doesn't handle collinear lines where keys overlap very cleanly so i spent a bit of time replacing those with solid lines instead 
another thing keebio plate gen does weird are the stab cutouts being 1 mm higher than ai03's. functionally this doesn't change anything but i think the non coplanar ones look better so i used those 

i measured the perimeter of the og jane plate in fusion and the numbers were nice so i used the same ones on my recreated plate. 
from the regular 19.05 mm grid, jane is 1 mm longer on the bottom, 0.5 mm longer on the left, 0.5 mm longer on the right, and 0.5 mm shorter on top 
![image](https://github.com/hali4045/i-hate-jane-plate/assets/66137164/8675ceeb-3f74-488a-b711-26efb727186c)
![image](https://github.com/hali4045/i-hate-jane-plate/assets/66137164/4d23278c-1bbd-454e-a5a0-754a17cc38c9)
![image](https://github.com/hali4045/i-hate-jane-plate/assets/66137164/2d092d40-0206-4782-af1a-385371dd5feb)

og jane has some ridiculous mounting point tech (that doesn't work) where the hole will extend wayyy farther into the plate than necessary as opposed to being concentric. in theory this allows for more give but i think it's dumb 
on the v2 ce (f13) these are all different lengths because the mounting points were designed with f12 in mind and didn't expect switch cutouts to interfere with the holes. i made the personal decision to make all of these as short as possible 
![image](https://github.com/hali4045/i-hate-jane-plate/assets/66137164/641c6027-48e0-43c4-9223-7d23e7721f59)
![image](https://github.com/hali4045/i-hate-jane-plate/assets/66137164/ceb254eb-786b-4c89-9d90-7ebeab4c3836)

_og jane v2 ce vs. my remake. keep in mind og is f13 and the screenshot of the remake is f12_ 

apart from that and the fact that the sizes on top vs. bottom are different, the mounting points were actually fairly normal to make 
![image](https://github.com/hali4045/i-hate-jane-plate/assets/66137164/c078da6c-c999-43d6-b662-99638f41ea2b)

_theorized anchor locations for mounting points_ 

from here i just measured numbers and drew them since they were all nice 
however during filleting i changed the radius of the convex fillets to 1.5 mm up from 1 mm. this reduces material but also allows for a 3 mm tool to be used in machining the case while maintaining tight tolerances 

after this all that was left was the usb cutout and corner chamfers and the jane plate is now normal 

end rant 

these files have not been prototyped, and i am not responsible for reimbursement if they do not work. 
