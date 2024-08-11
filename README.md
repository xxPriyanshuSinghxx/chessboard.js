
# Chessboard.js Documentation

## Properties

### 1. **sparePieces**
Controls whether spare pieces are available on the board. Default is `false`.

### 2. **legalMoveOnly**
Allows only legal moves if set to `true`. Default is `false`.

### 3. **moves**
An array that holds all the moves made on the board.

### 4. **turn**
Tracks the current turn, either "w" for white or "b" for black. Default is `"w"`.

### 5. **status**
Indicates the game status. Default is `"active"`.

### 6. **PGN**
Holds the Portable Game Notation (PGN) for the game.

### 7. **FENs**
Stores the history of board states in Forsyth-Edwards Notation (FEN).

### 8. **orientation**
Indicates the board's orientation. Default is `"white"`.

### 9. **draggable**
Allows pieces to be draggable if set to `true`. Default is `false`.

### 10. **showNotation**
Indicates whether the file and rank notation is shown. Default is `false`.

## Methods

### 1. **constructor(id, options = {})**
Initializes a new Chessboard object with an HTML element ID and options.

### 2. **enableDrag()**
Enables drag-and-drop functionality for pieces.

### 3. **disableDrag()**
Disables drag-and-drop functionality for pieces.

### 4. **start()**
Sets the board to the initial position and starts the game.

### 5. **flipBoard()**
Flips the board orientation between white and black.

### 6. **fen()**
Returns the current board state in FEN format.

### 7. **makeMove(start, end, method)**
Makes a move from the start square to the end square.

### 8. **sparePieces(permission)**
Controls the visibility and availability of spare pieces.
