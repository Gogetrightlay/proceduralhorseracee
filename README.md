# data
make a constant int NUM_HORSES

make a constant int TRACK_LENGTH

# main()
initialize an integer array horses with all values set to 0 (all horses start at the beginning).

initialize winnerFound = 0.

seed the random number generator with the current time.

repeat while no winner has been found:

for each horse, call printLane(horseNum, horses) to display the racetrack.;
for each horse, check with isWinner(horseNum, horses):

if true, print "Horse X WINS!!!" and set winnerFound = 1.

if winnerFound is still 0, prompt user: "Press enter for another turn", and wait for input.

end program

# advance()
generate a random number coin = rand() % 2 (value is either 0 or 1).

if coin == 1, increase the position of the current horse: horses[horseNum]++.

if coin == 0, do nothing (horse stays in place).

# printLane()
loop i from 0 to TRACK_LENGTH - 1.

if i == horses[horseNum], print the horse’s number (horseNum).

otherwise, print ".".

after the loop, print a newline so the next horse starts on the next row.

# isWinner()
if horses[horseNum] >= TRACK_LENGTH - 1, return true horse has reached the finish line.

otherwise, return false.
