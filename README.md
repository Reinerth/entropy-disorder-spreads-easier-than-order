# Example about the universal problem of entropy.<br> 

### Things that make me hmm.<br>


![09](https://github.com/user-attachments/assets/78c3521f-fef7-46c8-8051-824a4bcdf494)



<br>
Some philosophical notes and an abstract experiment about the universal problem of entropy.<br>
<br>
<br>
I am neither a physicist nor a mathematician, but it is clear and easy to understand,<br>
that building a house of cards, is much harder than destroying it.<br>
That requires no explanation. Or the same with the famous Rubik's Cube,<br>
which I still haven't figured out how to put those damn colors back in place.<br>
That ultimately seems to mean that disorder spreads easier than order.<br>
<br>
And even though I know there is no way out of it,<br>
I wanted to try it by myself if I could cheat at this universal law :-)<br>
I guess the main reason for the entropy-problem might be that we can't remember the way back.<br>
Means, all the footsteps we have walked till the reached point of disorder,<br>
are gone with the wind. It seems to be too expensive to remember them.<br>
<br>
So if I could remember the path I walked to disorder them,<br>
(in a script I could do that, by saving the steps somehow in a list)<br>
I could reorder them, with the "same" amount of steps that I needed to disorder them.<br>
But still the problem of "costs" is there, because remembering the path costs extra moves.<br>
At least on a binary level.<br>
<br>
<br>
<br>
<br>
Just for fun, I wanted to verify the theory by myself<br>
by trying to find a way, to order numbers,<br>
with fewer or the same amount of action moves, than I needed to disorder them.<br>
<br>
For that, I made a list of numbers that initially are sorted.<br>
Then I mix them and count the moves I needed for that.<br>
I count as a move, one step in a loop (I know on a binary level it would be much more).<br>
Finally, I applied different ways of sorting the numbers back.<br>
And again I counted the moves that I needed, to put them back in the place they belong.<br>
<br>
Initially the entropy convinced me to cheat,<br>
so that entropy would have an even greater advantage than it already has,<br>
on counting the amount of moves to disorder,<br>
by directly changing 2 numbers in one loop-step.<br>
This worked out, and I could reduce numbers to half of the length of the array,<br>
and I even could have reduced it to more if I had tried,<br>
but then I found, to be fair, I should have changed the sorting too,<br>
by trying to reposition two numbers in one loop-step.<br>
And this would work only in some rare cases (like explained in "My simple sort").<br>
So I corrected my hack to count the amount of steps in each loop-step.<br>
For both. The order and the disorder.<br>
<br>
So the number of steps for mixing could be reduced more,<br>
but I actually wanted the opposite.<br>
In the end it's just a matter of showing that the number for sorting<br>
cannot be smaller than the number for mixing.<br>
<br>
<br>
<br>
<br>
In reality my experiment could look something like this:<br>
I have an amount of number-cards in my hand (sorted) and I mix them (or simply throw them on the floor).<br>
Then I place them one by one, sorted, into my hand and count the moves for doing that.<br>
<br>
A philosophical difference I found between reality and script:<br>
In reality, we don't need to mix the cards with our hands.<br>
With one single move, we could let the cards fall down to get mixed.<br>
In the script, we need to take every number one by one to put it somewhere else.<br>
In the script there is no gravity or wind that would do the action moves instead.<br>
Could be hard to count those fuzzy wind-moves.<br>
Just imagine the other way around: the cards in your hand are mixed,<br>
you let them fall down, and they fall sorted on a stack. Easy life.<br>
<br>
<br>
<br>
<br>

### This is what the html-page looks like: <br>
No webserver needed for the html-page (only tested in Edge-browser).<br>
<img width="710" height="1252" alt="this-is-what-it-looks-like" src="https://github.com/user-attachments/assets/324d28ad-04b7-466e-bdbe-b6bc5729e9cb" />


<br>
<br>
<br>
<br>

### Some additional excusing words<br>
<br>
1). Just to be mentioned: I know this abstract, simplified example<br>
works only because of the "clear line we walk", a gapless and clean list of numbers.<br>
It wouldn't work out that easily if we have an irregular order and gaps, letters, colors, or more complex objects.<br>
And I have not analyzed the problem at the depth that I previously called "binary level",<br>
where I would need to count the moves of shifting the bits on the RAM-memory.<br>
<br>
2). The "My simple sort"-algorithm is explained with these unsorted numbers: 3-5-9-6-2-0-1-4-7-8<br>
We loop through those unsorted numbers<br>
and then place each one in a new Array at the index-position where it belongs.<br>
In first place is the number 3<br>
this has to be placed in the new array at the position myArray[3] ==> myArray[_, _, _, 3]<br>
On second place is the number 5<br>
this has to be placed in the new array at the position myArray[5] ==> myArray[_, _, _, 3, _, 5]<br>
and so on ... that's it.<br>
<br>
I am sure not to be the inventor of the "My simple sort",<br>
that I have called "My simple sort" just because I have written it without looking and finding it on the net.<br>
It might already have a name that I don't know.<br>
<br>
"My simple sort" is a kind of cheating, because we don't <ins>find</ins> the place where they belong,<br>
we <ins>know</ins> it just because they are numbers in a straight line/list.<br>
It is the same like the idea to remember the walked path. <br>
Our knowledge about the straight line is pendant to the rememberd path.<br>
This "sorting" works only with a gapless list of numbers.<br>
If we had only three numbers to sort like a million, a million and one, and a million and two,<br>
the Array-length would be a million and three, only for those three numbers :-)<br>
<br>
3). All other sorting algorithms have their own strengths that I do not mention here.<br>
One is better at sorting float-numbers or numbers with gaps,<br>
the other is better at sorting alpha-numerical values and so on.<br>
Not of importance in this little experiment.<br>
<br>
4) The script-code is not well-written or well-structured, because it is just a "quick-and-dirty-try".<br>
The focus is on (the difference of) the amounts of action moves for ordering and disordering,<br>
displayed in red in the output.<br>
The goal: a better understanding of the problem I'm living in.<br>


<br><br><br><br><br><br><br><br><br><br>
<br><br><br><br><br><br><br><br><br><br>

