# Developing and Evaluating a Chess AI using Mini-max and Alpha-Beta Pruning

## Short description of the project
For our project, we plan to develop a chess-playing artificial intelligence capable of selecting the best move from a given chess position. The primary goal will be to implement the Mini-Max algorithm with Alpha-Beta pruning and evaluate our best move while utilizing pruning to improve efficiency of searching through the chess game tree.
Our Chess AI will generate legal moves from the current board position and game state and possibly attempt to search ahead to determine which move produces the best expected outcome. Since completely searching a game tree of chess is computationally infeasible, Alpha-Beta pruning will be used alongside a depth limit to eliminate branches that cannot influence the final decision.
The program will use a heuristic evaluation function to estimate the strength of board positions when the search reaches its depth limit. A basic evaluation function based primarily on material value will first be implemented, with the goal of creating an enhanced version that considers additional chess concepts such as piece position, king safety, mobility and pawn structure.
Our intention is not to recreate the stockfish engine one to one, but rather to investigate and study how a classical AI search algorithm performs on chess and how its decisions compare with those of a modern chess engine as a benchmark.

## Programming language to be used
The project will primarily be implemented using Python. If a front-end is needed for any future deployment case we may utilize HTML/CSS/Javascript, and if we have enough time we can incorporate the React library, for any potential user interfaces so that users can view the board and play a game of chess.
We plan to use the python-chess library to help us represent the chess board, detect checks/checkmates, generate legal moves and to help us benchmark our AI with Stockfish for evaluation.

## Algorithms to be used
The primary algorithms and techniques to be used in the project will be:
  - Max Algorithm: To search possible future moves while assuming that both players attempt to make the optimal decision.
  - Alpha-Beta Pruning: To improve our search algorithm by eliminating branches from the search tree that will not affect the final decision.
  - Depth-Limited Search: Limits how far the AI searches because the chess game tree will be too large to evaluate.
  - Heuristic Evaluation Function: Estimate the value of a chess piece and position when the search depth limit is reached.
  - Move ordering: Potential best moves may be sorted to the top to be searched first so that alpha-beta pruning can begin on those trees instead of the possible worst.
Our evaluation function may consider factors including material advantage, piece-square positioning, king safety, mobility, pawn structure, and checkmate/stalemate.
## Datasets, if used
We may use the open-source datasets of chess evaluations and games from Lichess that are hosted on Hugging Face (chess-position-evaluation and standard-chess-games) that is in Forsyth-Edwards notation to help with our benchmarks if we feel it is needed.

## If you’re using open-source code or other codes available online, list which ones
We will be planning to use the following open-source libraries:
  - python-chess: An open-source Python chess library that will handle all of the chess game logic such as board representation, legal move generation, and chess rules. This will allow us to primarily focus on the chess AI aspect.
  - Stockfish: An open-source chess engine that will be used only as a benchmark for comparison with our AI.
The Mini-max algorithm, Alpha-beta pruning implementation, heuristic evaluation function, and performance analysis will be implemented by our group.
