# Electoral System Visualization
### About
Electoral System Visualization is a visual simulation of four different electoral system consisting of first-past-the-post (FPTP), Borda, Condorcet, and IRV. This project is written entirely in HTML5, CSS, and JavaScript. This project was inspired by a [webpage](http://www.zesty.ca/voting/sim) authored by Ka-Ping Yee.

### How Does It Work?
The simulation assumes that each candidate and voter can be plotted on a 2D plane. Imagine two axes of "Fiscal Policy" and "Social Policy". The diagram on the right shows such a plane with four election candidates plotted on it (the circles).

A voter can also be plotted on it (the square). This voter's first choice candidate is presumed to be the closest one. So in a FPTP election, this voter would vote for the green candidate.

Other voting systems use a "ranked ballot" -- a ballot where the voter can rank the candidates in order of preference. In our simulation, the candidates will be ranked by their Euclidian distance. This voter would rank green as their first choice (closest), blue as second, red as third, and finally yellow (farthest) as their fourth choice.

Now add more voters, all clustered around a "centre of opinion" (the cross). Most are close to the centre of opinion but others are far away, distributed in a normal distribution.

Now hold an election. Each of the voters casts a ballot with each candidate ranked by order of their distance from the voter. Count up the ballots to see who wins. Then colour the centre of opinion with the same colour as the winner.

Repeat the above for each point on the plane: move the "centre of opinion" to that point, scatter a large number of voters around that point, hold an election, and colour that point with the colour of the winner. Thus, each point on the plane represents an election with that point being the centre of public opinion. The result are images like those at the top of the page.

Obviously this is a simplification of real elections. But they do give us insights into the behaviour of each system. Real world behaviour would be more complex than these simulations show.

### Screenshots
![Electoral_System_Visualization_Screenshot](https://cloud.githubusercontent.com/assets/7763904/11633429/21973a00-9cd9-11e5-8fff-fcb47cc08aa1.png)

### Web Service Initialization
```Bash
./start
```

### License
* Electoral System Visualization is licensed under the [MIT license](https://www.github.com/elailai94/Electoral-System-Visualization/blob/master/LICENSE.md).
