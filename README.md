# cards-golang
A deck of playing cards, demo app written in Go 1.17.5 for practice.

## To Compile and/or Run
run `go build main.go deck.go`

that should produce an executable file called `main` or `main.exe` on Windows

or compile and run using `go run main.go deck.go`

## Type Details
the deck type currently has 7 functions associated
- `newDeck()` - creates a new deck with 52 "cards" (a slice of strings containing the card names)
- `print()` - prints the indexes and card names to the terminal 
- `shuffle()` - shuffles the cards in the current deck
- `deal(d deck, handSize int)` - returns 2 subsets of the current deck depending on the hand size to be dealt
- `toString()` - returns a single comma separated string with all the cards
- `saveToFile(filename string)` - saves the current deck to a file
- `newDeckFromFile(filename string)` - loads a deck from a file

## Testing
run `go test deck*` to run available tests for the `deck` type
