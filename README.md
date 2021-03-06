# TOOLING - SASS

I created a simple website :avocado:, do not take the content _seriously, it is for fun._ I had great time creating it, just to practice :point_right: SASS, :point_right: flexbox :point_right: and add few javascript lines(really basic for a beginner - when you click on the circle of Mr. Avocado) and there is spin animation on hover with the emojis. My project is responsive, there are is basically one breakpoint, but yes, there should be more, but as this is very simple design It does not apply for that many breakpoints. I used flexbox, but from now on I plan to apply grid. The project serve as an exercise like design for our course.

- Live site links to my project:
  - https://liadensam.github.io/tooling-sass/
  - https://late-trees.surge.sh/

## SASS :avocado:

It is the first time I used SASS and I am so grateful for its existence as I like to be organized and this tool enables me to organize my projects in an excellent way into different folders. I use three folders and within those folders I placed separte files.

### Structure of my project with sass organization :point_down:

- base
  - \_base-index.sass
  - \_base.sass
  - \_mixins.sass
  - \_typography.sass
  - \_variables.sass
- components
  - \_components-index.sass
  - \_content.sass
  - \_header.sass
- layout
  - \_layout-index.sass
  - \_flexbox.sass

As you can see, It is already clear where comes what part. Each folder has its _\_name-index.sass_ file so all the code from the particular folder with index can be imported there and then just the import from that index to the main _style.sass._ It is very important to have the _ before tha name of your connecting files to the main sass file, it means it will be imported to the main sass stylesheet and when you import it you do not need to write _ in front of it as you can see here :point_down:
![2021-09-12](https://user-images.githubusercontent.com/80709364/132992729-b1232c32-300e-4f16-9f67-8b03294fe06d.png)

At first, what is a great feature in VS code, you can have live compilation of SASS or SCSS to CSS. It is an extension, so you can just download it there and you do not need to watch that through your terminal :point_down:
![2021-09-12 (1)](https://user-images.githubusercontent.com/80709364/132992968-6da84ae3-66d8-44ec-a8ce-2807f38563af.png)

Then I jumped into the SASS and its magic. I used **variables** for my colors, linear gradient and font as if I decide to change anything and it would change for the whole file for the spots where the variable is and I do not need to go to the specific parts and change it there. I used mixins and some variables within those mixins as the linear gradient one. I created mixins for repetitive same parts where one or more styles are changed otherwise is the same code. You have to use @include when you insert mixin. For example here :point_down: I wrote mixin for profile-img where the code is the same for the elements, just I need to change background-color.

![2021-09-12 (2)](https://user-images.githubusercontent.com/80709364/132993181-4b83474b-a6a7-47c4-9060-d00bccdddefd.png)

I used nesting for example here in the content.sass file :point_down: where the paragraph belongs to the class content-boxes so it could be written as that to save some lines.
![2021-09-12 (3)](https://user-images.githubusercontent.com/80709364/132993265-1a892094-4a22-4334-9fdc-efacfc19173c.png)

It will appear in CSS as this :point_down:
![2021-09-12 (4)](https://user-images.githubusercontent.com/80709364/132993336-0bb229d9-84be-4253-97b8-fd43c5d9ca70.png)

These were the most useful points of SASS and for beginner enough to start and get more into that. I really :green_heart: the organization of the file so I can imagine working in a team is much easier then. :avocado:
