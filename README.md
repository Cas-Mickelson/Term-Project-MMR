**How to Run:**
1. Ensure that Java JDK is installed on your computer
2. Save each of the program files respectively as:
MMRSystem.java Team.java Player.java & Leaderboard.java
3. Open a terminal
4. Navigate to the folder containing the file
5. Compile the program by typing "javac" followed by each of the following:
MMRSystem.java Team.java Player.java & Leaderboard.java
6. Run the program by typing: java MMRSystem
7. The Results tab displays the last match results, and the Leaderboard tab displays the leaderboard/MMR database. Click Import to modify Players’ MMRs based on the match results, the Leaderboard tab and file will update in real time. Click Reset to reset all Players’ MMRs. Click Exit to close the application. You can update the results.csv file manually to test different results.
> [!CAUTION]
> In a practical application no one would have access to results.csv, so there is no validation on the data.

**Project Description:**
MMRSystem Class:
  Abstract. Computes: How much MMR to give or take from each player on all teams from a match based on their contribution, whether their team won or lost, how many players were on the enemy team, and a predetermined total MMR “gambled” by each team based on it's size.
  Reads the results.csv file.

Team Class:
  Concrete. Stores: a group of Players, each of their contributions to how the Team performed, if the Team won, & a Color representing the Team.
  Computes: The percentage a player contributed to the team's performance or lack thereof, and the Team’s overall KDA.

Player Class:
  Concrete. Stores: assists, deaths, id, kills, username.
  Computes: a Player’s KDA.

Leaderboard Class:
  Concrete. Stores: All active and inactive players, their ID’s, & MMR’s.
  Performs all read and write operations to the leaderboard.csv file.

Record Class (inside Leaderboard.java):
  Concrete. Stores: id, mmr, & username.

**Features:**
Displays last match results.
Displays player leaderboard.
Updates leaderboard based on last match results (on click).
Resets leaderboard.
