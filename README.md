# ChessBoard.js Documentation

## Overview
The `ChessBoard` class is a comprehensive JavaScript library for creating and managing a chessboard on a web page. It provides features such as drag-and-drop functionality, highlighting legal moves, handling castling, en passant, and more. This class is designed to be flexible and customizable, making it suitable for various chess-related applications.

## Features
- **Drag-and-drop pieces**
- **Highlight legal moves**
- **Support for castling and en passant**
- **Customizable board and piece themes**
- **Timer and increment functionality**
- **Coordinates display**
- **Sound effects for moves**

## Class: `ChessBoard`

### Properties
- `#board`: The DOM element for the chessboard.
- `#chessboard`: The main chessboard element.
- `sparePieces`: Boolean indicating if spare pieces are enabled.
- `#highlightSquare`: Class for highlighting squares.
- `#isDragging`: Boolean indicating if a piece is being dragged.
- `#onlyLegalMove`: Boolean for allowing only legal moves.
- `#highlightLegalMoves`: Boolean for highlighting legal moves.
- `pieceTheme`: The theme for the pieces.
- `#darkColor`: Color for dark squares.
- `#lightColor`: Color for light squares.
- `moves`: Array of moves made.
- `status`: The status of the game.
- `halfMoveCount`: Half move count for the game.
- `fullMoveCount`: Full move count for the game.
- `enPassantSquare`: The en passant square.
- `turn`: Whose turn it is to move ('w' or 'b').
- `PGN`: Array for storing the Portable Game Notation.
- `moveStack`: Stack of moves made.
- `FEN`: Current FEN (Forsyth-Edwards Notation).
- `FENs`: Array of FENs.
- `timeFormat`: Object for time control settings.
- `whiteTime`: Time left for white.
- `blackTime`: Time left for black.
- `increment`: Increment per move.
- `timerInterval`: Interval for the timer.
- `lastTimestamp`: Timestamp for the last timer update.
- `ID1`: ID for the white timer display element.
- `ID2`: ID for the black timer display element.
- `matchStarted`: Boolean indicating if the match has started.
- `enableSound`: Boolean for enabling sound effects.
- `isAnimating`: Boolean indicating if an animation is ongoing.
- `castlingRights`: Object for castling rights.
- `#promotingPiece`: Piece to promote to.
- `#width`: Width of the board.
- `#offsetX`: X offset for dragging.
- `#offsetY`: Y offset for dragging.
- `#firstClick`: First click timestamp.
- `#draggableDiv`: Draggable div element.
- `#originalParent`: Original parent element of the piece.
- `#startSquare`: Start square of the move.
- `#endSquare`: End square of the move.
- `#lastMove`: Object for the last move made.
- `#pieceMap`: Map of piece codes to class names.
- `#_pieceMap`: Reverse map of class names to piece codes.
- `#fenChar`: Map of FEN characters to piece codes.
- `#_fenChar`: Reverse map of piece codes to FEN characters.
- `everyMove`: Array of every move made.

### Constructor
#### `constructor(id, options = {})`
- **id**: The ID of the HTML element to attach the chessboard to.
- **options**: Configuration options for the chessboard.

### Methods
#### `addStyles()`
Adds CSS styles for the chessboard.

#### `startTimer()`
Starts the game timer.

#### `stopTimer()`
Stops the game timer.

#### `updateTimer()`
Updates the game timer.

#### `toggleTimer()`
Toggles the timer on and off.

#### `updateDisplay()`
Updates the display of the timer.

#### `formatTime(milliseconds)`
Formats time from milliseconds to a string.

#### `onScroll(event)`
Handles scroll events for undoing moves.

#### `handleKeyDown(event)`
Handles keydown events for navigating moves.

#### `handleRightArrow()`
Handles the right arrow key for navigating moves.

#### `handleLeftArrow()`
Handles the left arrow key for navigating moves.

#### `#initializeBoard(position)`
Initializes the chessboard with a given position.

#### `enableCoordinates()`
Enables coordinate notation on the board.

#### `disableCoordinates()`
Disables coordinate notation on the board.

#### `#createImage(pieceCode)`
Creates an image element for a piece.

#### `createCircle(square)`
Creates a circle on a square.

#### `createRing(square)`
Creates a ring on a square.

#### `showLegalMoves(moves, fen)`
Shows legal moves on the board.

#### `hideLegalMoves()`
Hides legal moves on the board.

#### `changeTurn()`
Changes the turn to the next player.

#### `nextTurn()`
Gets the next player's turn.

#### `#playSound(move)`
Plays a sound for a given move.

---

This documentation provides a detailed overview of the `ChessBoard` class, its properties, methods, and functionalities. For a complete understanding, refer to the code comments and inline documentation in the `chessBoard.js` file.
