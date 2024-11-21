
# Grammar Tree Visualizer

This project allows you to generate and visualize grammar trees based on a set of grammar rules provided in a text file. The tree is constructed using the `networkx` library to represent the relationships between grammar symbols, and it is visualized using `matplotlib`.

## Features
- Parse a grammar from a text file (formatted as grammar rules).
- Generate a derivation tree based on the grammar rules.
- Visualize the resulting tree using `matplotlib` and `networkx`.

## Project Structure

- `main.py`: Contains the main code for reading the grammar, generating the tree, and visualizing it.
- `grammar.txt`: A sample grammar file that contains the rules of the grammar.
- `requirements.txt`: Lists the Python dependencies required to run the project.

## Getting Started

### Prerequisites

Make sure you have Python 3.x installed on your machine. You can download it from [here](https://www.python.org/downloads/).

### Installation

1. **Clone the Repository**

    ```bash
    git clone https://github.com/yourusername/grammar-tree-visualizer.git
    cd grammar-tree-visualizer
    ```

2. **Install the required dependencies**

    Use the following command to install the necessary Python libraries from the `requirements.txt` file:

    ```bash
    pip install -r requirements.txt
    ```

    The required dependencies are:
    - `networkx`
    - `matplotlib`

3. **Prepare the Grammar File**

    The `grammar.txt` file should contain grammar rules in the following format:

    ```
    S -> A B
    A -> a
    B -> b
    ```

    Each rule has a non-terminal symbol on the left-hand side and a list of symbols (terminals or non-terminals) on the right-hand side, separated by `->`.

### Running the Project

To run the code and generate a grammar tree:

```bash
python main.py
```

### Example Grammar

Your `grammar.txt` file should follow this format:

```
S -> A B
A -> a
B -> b
```

This will generate a tree with the root node `S`, which expands into `A` and `B`, where `A` expands into terminal `a` and `B` expands into terminal `b`.

### Visualizing the Tree

The tree is visualized in a pop-up window using `matplotlib`. Each node in the tree represents a symbol in the grammar, and the edges represent the production rules.

### Customizing the Grammar

To use your own grammar, modify the `grammar.txt` file with the new rules. Be sure to maintain the format shown above.

## File Descriptions

- `main.py`: The core script that reads the grammar, generates the tree, and visualizes it.
- `grammar.txt`: Contains the grammar rules used to generate the tree.
- `requirements.txt`: Lists the dependencies needed to run the project.

## Future Enhancements
- Support for more complex grammars with multiple production rules for a non-terminal.
- Error handling for malformed grammar files.
- Command-line arguments for passing custom grammar files and visualization options.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
# TheOne
