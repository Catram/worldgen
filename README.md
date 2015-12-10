## Fractal Worldmap Generator

Creator: John Olsson

Thanks to Carl Burke for interesting discussions and suggestions of how to speed up the generation! :)

This program is provided as is, and it's basically a "hack". So if you want a better userinterface, you will have to provide it by yourself!

For ideas about how to implement different projections, you can always look in WorldMapGenerator.c (the CGI program that generates the gifs on my www-page [http://www.lysator.liu.se/~johol/fwmg/fwmg.html].

Please visit my WWW-pages located at: [http://www.lysator.liu.se/~johol/]. You can send E-Mail to this adress: johol@lysator.liu.se

I compile this program with: ```gcc -O3 worldgen.c -lm -o gengif```

This program will write the GIF-file to a file which you are prompted to specify.

To change size of the generated picture, change the default values of the variables XRange och YRange.

You use this program at your own risk! :)

When you run the program you are prompted to input three values:

* Seed: This the "seed" used to initialize the random number generator. So if you use the same seed, you'll get the same sequence of random numbers...
* Number of faults: This is how many iterations the program will do. If you want to know how it works, just enter 1, 2, 3,... etc. number of iterations and compare the different GIF-files.
* PercentWater: This should be a value between 0 and 100 (you can input 1000 also, but I don't know what the program is up to then! :) The number tells the "ratio" between water and land. If you want a world with just a few islands, input a large value (EG. 80 or above), if you want a world with nearly no oceans, a value near 0 would do that.