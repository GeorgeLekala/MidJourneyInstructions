This page provides information about the Midjourney V4 model, which is an entirely new codebase and brand-new AI architecture designed by Midjourney and trained on the new Midjourney AI supercluster. The latest Midjourney model has more knowledge of creatures, places, objects, and more. It’s much better at getting small details right and can handle complex prompts with multiple characters or objects. The Version 4 model supports advanced functionality like image prompting and multi-prompts. The Midjourney Model Version 4 has three slightly different “flavors” with slight tweaks to the stylistic tuning of the model. Experiment with these versions by adding --style 4a, --style 4b, or --style 4c to the end of a V4 prompt. --v 4 --style 4c is the current default and does not need to be added to the end of a prompt. --style 4a and --style 4b only support 1:1, 2:3, and 3:2 aspect ratios. --style 4c support aspect ratios up to 1:2 or 2:1. You can access earlier midjourney models by using the --version or --v parameter or by using the /settings command and selecting a model version. Different models excel at different types of images. The niji model is a collaboration between Midjourney and Spellbrush tuned to produce anime and illustrative styles. The --niji model has vastly more knowledge of anime, anime styles, and anime aesthetics. It’s excellent at dynamic and action shots and character-focused compositions in general. Niji does not support the --stylize parameter. Use the /settings command and select Style Med to reset to the default style setting for all --niji prompts. Niji supports multi-prompts or image-prompts. Occasionally new models are released temporarily for community testing and feedback. There are currently two available test models: --test and --testp, which can be combined with the --creative parameter for more varied compositions. Test models only support --stylize values between 1250–5000. Test models do not support multi-prompts or image-prompts Test models have a maximum aspect ratio of 3:2 or 2:3. Test models only generate two initial grid images when the aspect ratio is 1:1. Test models only generate one initial grid image when the aspect ratio is not 1:1. Words near the front of the prompt may matter more than words near the back. You can add --v 1, --v 2, --v 3, --v 4, --v 4 --style 4a, --v4 --style 4b --test, --testp, --test --creative, --testp --creative or --niji to the end of your prompt. You can also type /settings and select your preferred version from the menu. 1️⃣ MJ Version 1 2️⃣ MJ Version 2 3️⃣ MJ Version 3 4️⃣ MJ Version 4 Niji Mode MJ Test MJ Test Photo

This page provides information about Midjourney upscalers. Midjourney starts by generating a grid of low-resolution image options for each job. You can use a Midjourney upscaler on any grid image to increase the size and add additional details. There are multiple upscale models available for upscaling an image. The U1 U2 U3 U4 buttons under each image grid are used to upscale the selected image. The default Midjourney resolutions are 512×512 (image variations), 1024×1024 (upscale), 1664×1664 (upscale to max), and 2048×2048 (beta upscale redo). These default resolutions aren’t sufficient in most cases for production of apparel and merchandise beyond about 5×5 inches. Midjourney has five upscale models available each serving different purposes. The latest default upscaler increases image size while smoothing or refining details. Some small elements may change between the initial grid image and the finished upscale. The Light Upscaler creates a 1024px x 1024px image and adds a moderate amount of details and textures. The Detail Upscaler, creates a 1024px x 1024px image and adds many additional fine details to the image. The Beta Upscaler creates a 2048px x 2048px image without adding many additional details. The Anime Upscaler is the default upscaler for the --niji model. It upscales images to 1024px x 1024px and is optimized to work well with illustrated and anime styles. Remaster is an additional option for previously upscaled images made with the V1, V2, or V3 Model Versions. Remaster will upscale an image again using the --test and --creative parameters blending the composition of the original image and the coherency of the newer --test model. Remaster any previously upscaled job by clicking the Remaster button found beneath the original upscale. To Remaster very old jobs, use the /show command to refresh that job in Discord. You can access earlier midjourney models by using the --version or --v parameter or by using the /settings command and selecting a model version. Different models excel at different types of images. You can type /settings and select your preferred upscaler from the menu. 1️⃣ Default Upscaler 2️⃣ Light Upscaler 3️⃣ Detail Upscaler 4️⃣ Beta Upscaler 5️⃣ Anime Upscaler

Basic Midjourney commands

/imagine: The primary command to create an image.
/help: Provides helpful information about the Midjourney bot.
/info: Show information about your account and usage.
/subscribe: Subscribe to the bot.
/fast: Your jobs will be incrementally billed.
/relax: Your jobs do not cost, but takes longer to generate.
/show <jobid>: Revive any job.
/private: Your jobs are private.
  
 Here are some examples of multi prompts from the Midjourney Multi Prompts guide 1:

Adding a double colon :: to a prompt indicates to the Midjourney Bot that it should consider each part of the prompt separately. For example, for the prompt hot dog, all words are considered together, and the Midjourney Bot produces images of tasty hotdogs. If the prompt is separated into two parts, hot:: dog, both concepts are considered separately, creating a picture of a dog that is warm.
You can assign a number immediately after the double colon to assign the relative importance to that part of the prompt. For example, the prompt hot:: dog produced a dog that is hot. Changing the prompt to hot::2 dog makes the word hot twice as important as the word dog, producing an image of a dog that is very hot!
You can add parameters at the end of the prompt. For example, the prompt cup:: cake illustration is considered together, producing illustrated images of cupcakes. The prompt cup:: cake illustration::2 is the same as cup:: cake illustration::1, but with the parameter 2 added to the end, making the word cake twice as important as the other words in the prompt 1.
I hope that helps. Let me know if you have any other questions.

Here are some key detailed takeaways from the Midjourney Explore Prompting documentation:

Even short single-word prompts will produce beautiful images in Midjourney’s default style, but you can create more interesting personalized results by combining concepts like artistic medium, historical periods, location, and more.
Pick A Medium: In the example below, the prompt is “painting of a cat in the style of Van Gogh”. The Midjourney Bot produces an image of a cat in the style of Van Gogh.

  Parameters are options added to a prompt that change how an image generates. Parameters can change an image's Aspect Ratios, switch between Midjourney Model Versions, change which Upscaler is used, and lots more.
Parameters are always added to the end of a prompt. You can add multiple parameters to each prompt.

Example of how Midjourney parameters are used.



Using an Apple device?
Many apple devices automatically change double hyphens (--) to an em-dash (—). Midjourney accepts both!

Basic Parameters
Aspect Ratios
--aspect, or --ar Change the aspect ratio of a generation.

Chaos
--chaos <number 0–100> Change how varied the results will be. Higher values produce more unusual and unexpected generations.

No
--no Negative prompting, --no plants would try to remove plants from the image.

Quality
--quality <.25, .5, 1, or 2>, or --q <.25, .5, 1, or 2> How much rendering quality time you want to spend. The default value is 1. Higher values cost more and lower values cost less.

Seed
--seed <integer between 0–4294967295> The Midjourney bot uses a seed number to create a field of visual noise, like television static, as a starting point to generate the initial image grids. Seed numbers are generated randomly for each image but can be specified with the --seed or --sameseed parameter. Using the same seed number and prompt will produce similar ending images.

Stop
--stop <integer between 10–100> Use the --stop parameter to finish a Job partway through the process. Stopping a Job at an earlier percentage can create blurrier, less detailed results.

Style
--style <4a, 4b or 4c> Switch between versions of the Midjourney Model Version 4

Stylize
--stylize <number>, or --s <number> parameter influences how strongly Midjourney's default aesthetic style is applied to Jobs.

Uplight
--uplight Use an alternative "light" upscaler when selecting the U buttons. The results are closer to the original grid image. The upscaled image is less detailed and smoother.

Upbeta
--upbeta Use an alternative beta upscaler when selecting the U buttons. The results are closer to the original grid image. The upscaled image has significantly fewer added details.

Default Values (Model Version 4)
Aspect Ratio	Chaos	Quality	Seed	Stop	Style	Stylize
Default Value
1:1	0	1	Random	100	4c	100
Range
1:2–2:1	0–100	.25 .5 or 1	whole numbers 0–4294967295	10–100	4a, 4b, or 4c	0–1000


Default Values (Model Version 5)
Aspect Ratio	Chaos	Quality	Seed	Stop	Stylize
Default Value
1:1	0	1	Random	100	100
Range
any	0–100	.25 .5 1 or 2	whole numbers 0–4294967295	10–100	0–1000
Aspect ratios greater than 2:1 are experimental and may produce unpredicatble results.


Model Version Parameters
Midjourney routinely releases new model versions to improve efficiency, coherency, and quality. Different models excel at different types of images.

Niji
--niji An alternative model focused on anime style images.

High Definition
--hd Use an early alternative Model that produces larger, less consistent images. This algorithm may be suitable for abstract and landscape images.

Test
--test Use the Midjourney special test model.

Testp
--testp Use the Midjourney special photography-focused test model.

Version
--version <1, 2, 3, 4, or 5> or --v <1, 2, 3, 4, or 5> Use a different version of the Midjourney algorithm. The current algorithm (V4) is the default setting.



Upscaler Parameters
Midjourney starts by generating a grid of low-resolution image options for each Job. You can use a Midjourney upscaler on any grid image to increase the size and add additional details. There are multiple upscale models available for upscaling an image.

Uplight
--uplight Use an alternative "light" upscaler when selecting the U buttons. The results are closer to the original grid image. The upscaled image is less detailed and smoother.

Upbeta
--upbeta Use an alternative beta upscaler when selecting the U buttons. The results are closer to the original grid image. The upscaled image has significantly fewer added details.

Upanime
Use an alternative upscaler trained to work with the when selecting the U buttons. This upscaler was specifically created to work with the --niji Midjourney Model.


Other Parameters
These parameters only work with specific earlier Midjourney Models

Creative
--creative Modify the test and testp models to be more varied and creative.

Image Weight
--iw Sets image prompt weight relative to text weight. The default value is --iw 0.25.

Sameseed
--sameseed Seed values create a single large random noise field applied across all images in the initial grid. When --sameseed is specified, all images in the initial grid use the same starting noise and will produce very similar generated images.

Video
--video Saves a progress video of the initial image grid being generated. Emoji react to the completed image grid with ✉️ to trigger the video being sent to your direct messages. --video does not work when upscaling an image.

Compatibility
Model Version & Parameter Compatability
Affects initial generation	Affects variations + remix	Version 5	Version 4	Version 3	Test / Testp	Niji
Max Aspect Ratio	✓	✓	any	1:2 or 2:1	5:2 or 2:5	3:2 or 2:3	1:2 or 2:1
Chaos	✓		✓	✓	✓	✓	✓
Image Weight	✓		✓		✓	✓	
No	✓	✓	✓	✓	✓	✓	✓
Quality	✓		✓	✓	✓		✓
Seed	✓		✓	✓	✓	✓	✓
Sameseed	✓				✓		
Stop	✓	✓	✓	✓	✓	✓	✓
Style				4a and 4b			
Stylize	✓		0–1000
default=100	0–1000
default=100	625–60000
default=2500)	1250–5000
default=2500)	
Tile	✓	✓	✓		✓		
Video	✓				✓		
Number of Grid Images	-	-	4	4	4	2 (1 when aspect ratio≠1:1)	


Deprecated Parameters
--width and --w (replaced with --aspect)
--height and --h (replaced with --aspect)
--fast (replaced with --quality)
--vibe (now known as V1)
--hq
--newclip
--nostretch
--old
--beta


