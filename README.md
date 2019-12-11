# houdini-genetic-optimization
Optimization on [jhorikawa](https://github.com/jhorikawa/HoudiniHowtos/tree/master/0012%20Genetic%20Algorithm) genetic algorithm for 3d metaball reconstruction

1. Keeping the best of the previous generation on the current DNAs
2. Making the best of previous generation one of the parents of every individual of the current generation. The other partner continues to be selected ramdomly (with chances proportional to the fitness)
3. When not evolving more than 5 for more than 5 generations, double mutation rate for the next 5 generations
 
 Futher possible improvements:
 1. After stabilizing a general form, create a cloud of smaller metaballs atracted to the original model for fine-tuning
 2. If there's no improvement even with doubled mutation rate, create extinction event (save the best in separate pool)
 
 ![Final result](https://i.imgur.com/4wSRt0P.png)
