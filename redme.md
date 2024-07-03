Want i learn form this project

1) "sticky header" or "sticky navigation."
parent - relative 
child - sticky top-0 left-0 

See, I set the parent element to relative and the child element to sticky with top-0 and left-0. When we scroll, it will stay stuck at the top and won't move upwards

Example:-
<div class="relative"> 
    <div class="sticky top-0 left-0"></div>
</div>



2) condition second 

If you have two parts, left and right, and you want only the left part to stick, you can do this:
<div class="flex justify-center items-start relative">
    <div class="sticky top-0 left-0"></div>
</div>

When you apply the flex property to the parent, it occupies the full height of the container. So, to ensure that only the parent's height and width are considered, you should use items-start. This allows the sticky positioning to work as intended." 




3) image fiting in circle form

<div class="w-[22rem] h-[22rem] overflow-hidden rounded-full">
    <img class="w-full h-full object-cover" src="" alt=""></div>
</div>

The overflow-hidden class is applied to the parent <div> element. This class is used to specify that any content overflowing the bounds of the container should be hidden from view

Inside the container, there's an <img> element with the classes "w-full h-full object-cover." This image is set to occupy the entire width and height of its parent container while maintaining its aspect ratio. The object-cover class ensures that the image covers the entire container area, cropping it if necessary to fit.

4) for working of justify-center items-center u must give them flex otherwise it will not working but if u give flex then your content align row wise u want it will be colume wise in that cinario u give them this property "flex-col"

in simple language - If you want to center content both horizontally and vertically within a container using flexbox, you typically use justify-center and items-center classes. But if you want the content to stack vertically instead of horizontally, you add the flex-col class.

ex:-
<div class="flex justify-center items-center flex-col">
    <!-- Your centered content here -->
</div>
