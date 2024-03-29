# Wiki-Game-Solver
A real-time navigation program over Wikipedia's articles’ graph. Implementing a bi- directional extension for the classic A* search and a variety of heuristics based on  different domains, including NLP and Graph Theory, in order to defeat a human on the popular Wiki-Game.<br>
<ul>
<li>WikiProblem.py - this module implements the WikiProblem which serves the problem interface using the online wikipedia API. it gives more data (text, categories etc.) but is slower than the offline interface. </li>
<li>WikiSolver.py - this module implements all solving mechanisms it includes a node class (used for tracking depth and path of search) a "base search" that is used for running all A* variations and all heuristics used in our project.</li>
<li>OnlineGamer.py - this script uses selenium in order to play online on https://thewikigame.com. It only executes code from WikiSolver. to see the agent competes with others online just run the script with no arguments.</li>
<li>executor.py - this file runs the code. it allows to run a single search with a single heuristic or run a full test that writes results to a tsv file. to see the correct usage run this script with no arguments.</li>
<li>sql_offline_queries.py - this module implements the OfflineWikiProblem which serves the problem interface using an <a href="https://drive.google.com/open?id=1kf_FEVSy6z_ACcL7kqop9a6LCXAP8jKB"> offline DB</a>. Extract the file and save it near this repository, in a parent directory, under the name "sdow.sqlite".</li>
<li>utils.py - data structures useful for implementing SearchAgents, from Pacman AI projects that were developed at UC Berkeley, and are used here for educational purposes.</li>
<li>index.html - the website from this project, describing it in hebrew. </li>
<li>improved_wikipedia (package) - an improvement for the popular wikipedia package, allowing quering more pages and info about pages with less requests.</li>
</ul>   

# requirements:
<ul>
  <li>wikipedia</li>
  <li>sqlite3</li>
  <li>BeautifulSoup</li>
  <li>requests</li>
  <li>sklearn</li>
  <li>scipy</li>
  <li>selenium (for the OnlineGamer)</li>
</ul>  





