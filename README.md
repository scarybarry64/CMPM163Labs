# CMPM163Labs
 
# Lab 2

Video: https://drive.google.com/file/d/1FH0aVV149_2M6mAkc414s7KPxrNHsHsl/view?usp=sharing

![](lab2/Lab2-Part2-Screenshot.PNG)

# Lab 3

Video: https://drive.google.com/file/d/1lCTCOwpgDgZ4DowcpvEWmLrhn2L8_4_x/view?usp=sharing

How: (From left to right) The first cube is made using shaders. I simply copied the code provided in the lab for making the other shader cube, though I made a separate fragment shader per the instructions. I then changed the color to lime, and had it rotate on the z-axis. The second cube is made using Three.js materials. It's the first cube made per the instructions. It has a grey phong material, with some specular and shininess. The lighting adds a greenish tint to the cube too. The third cube (my favorite) is also made using Three.js materials. For this, I used a toon material and colored it orange. I tweaked its specular, shininess, transparancy, and opacity to give it a shiny see-through look. The lighting makes it pulse magenta once it hits a certain angle as it rotates in the negative x direction. Lastly is the second cube mader per the instructions. It uses shaders, mixing colors to achieve a cyan sheen with hints of blue on its lower corners.

# Lab 4

Video: https://drive.google.com/open?id=1b7r3TuA5xE15Tofzve2w6at6cpShX7ZJ

How: 
- Cube 1 (Center): Using three.js built in texture functionality, I gave this cube a grassy-stone texture and its corresponding normal map to produce a fairly detailed centerpiece. Being in the center, you cannot see its sides.
- Cube 2 (Left): This is essentially the same as Cube 1, but without the normal map. It looks noticeably less detailed with the lighting, but you can see its right side due to it being 2 to the left.
- Cube 3 (Right): Again similar to Cube 1, but this time it uses a sandy-brick texture and corresponding normal map. It's also off to the right by 2, meaning you can see its left side.
- Cube 4 (Top): This uses shaders per the instructions. I gave it a pinkish texture, possibly old paint on metal or wood. It has no normal map, and so looks quite dull. It's up by 2, meaning you can see its bottom side.
- Cube 5 (Bottom): My favorite! This is similar to Cube 4, except I did some math magic to give it a 4x4 tiled wood texture. Basically, I took the varying vec2 "vUv" and modded it by 0.25, then I multiplied by 4.0. The result is a 4x4 cube, in which the original wood texture repeats itself in a 4x4 grid on each side. See line 61 for the magic. Cool! This cube is down by 2, meaning you can see its top.

Answers:
- a) To get the x coordinate from a given u value, multiply u by 8. Formula: x = 8 * u
- b) To get the y coordinate from a given v value, multiply v by 8. Formula: y = 8 * v
- c) White is the color sampled from the texture at uv coordinate (0.375, 0.25), which corresponds to (3, 2) on the texture.
