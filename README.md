# rust-voltorb-flip-solver

<p float="left">
  <img src="https://user-images.githubusercontent.com/63099057/129618132-7642ce71-a68b-41cb-852b-8ee9f10f6f06.png" width="400" />
  <img src="https://user-images.githubusercontent.com/63099057/129618351-7c640987-ff53-4360-9d2d-0f2dd872e077.png" width="400" /> 
</p>

An efficient tool for solving Voltorb Flip puzzles (https://bulbapedia.bulbagarden.net/wiki/Voltorb_Flip).

Features so far:  
<ul>
  <li>first correct Voltorb Flip solver (Popular ones didn't even ask for the level :D). </li>
  <li>uses all cores</li>
  <li>very performant (given the difficulty of the task)</li>
  <li>nice colorful graphic user interface, missclick-proof, worst you can do is restart the calculation</li>
  <li>optimal and correct, assuming perfect randomness (someone provided me with Nintendo's level generation algorithm)</li>
  <li>displays the actualy win chance and, if you're curious, the chances of being a bomb/1/2/3 for each square when hovering over it</li>
</ul> 

System requirements:  
<ul>
  <li>tested on > 200.000 puzzles sampled from the actual game</li>
  <li>needs less than 30 seconds and 3 GB RAM for each puzzle tested (i7-8750H: 6 cores, hyperthreading)</li>
  <li>usually solves puzzles within a second or less </li>
</ul> 

Control:  
<ul>
  <li>click on buttons to advance their number</li>
  <li>pressing a number while doing so advances to that number straight away</li>
  <li>program starts calculating automatically</li>
  <li>choose the yellow squares (=free coins)</li>
  <li>if there are none wait for the dark blue ones (=highest chance to win, but possibly a bomb)</li>
  <li>grey means "useless" e.g. can't be a 2 or 3</li>
  <li>the windows title tells you about ongoing calculations, whether the constraints are consistent and so on</li>
</ul> 

Note:
<ul>
  <li>Starts out with puzzle 1 of examples.txt (extremely easy puzzle)</li>
  <li>Entering the level is just as crucial as the other constraints!</li>
  <li>Maximizes the chance of winning the ENTIRE puzzle, doesn't care whether it dies in one or three moves (yet)</li>
  <li>I'm still working on it, those problems will be solved, there will be suitable modes</li>
</ul>

Download: https://github.com/Tobs40/rust-voltorb-flip-solver/releases
